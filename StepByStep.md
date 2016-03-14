# How to use IDEM-IA. Step by step. #

The process of designing an Idemia‘s solution  is a complex process involving a set of steps where you start with the creation of the project structure and then model each of the elements of the problem and the relationship between them. To better understand this process it was decided to divide it into two main stages. In the first, called "generation", is defined and customized the project structure that will support the next stage.  In the second, are modeled graphically the components of the problem, among which are: agent, environment, states, actions, perceptions, etc.

To describe the complete process, it will use an academic example called “Pacman”.

> ![http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/1.PacmanSolutionSnapshot.png](http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/1.PacmanSolutionSnapshot.png)



## Stage 1: Generating a Solution ##

This stage defines the project structure and generates the empty model to design the solution.


  1. Select File > New > Java Project
> > ![http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/2.NewJavaProyectMenu.png](http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/2.NewJavaProyectMenu.png)
  1. In New Java Project dialog that appear, enter “Pacman” for the Project Name


> ![http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/3.NewJavaProyect.png](http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/3.NewJavaProyect.png)

  1. Click Finish
  1. Once project is created, select it.
  1. Select File > New > Folder
> > ![http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/4.NewFolderMenu.png](http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/4.NewFolderMenu.png)
  1. In New Folder dialog, enter o select “Pacman” for the parent folder
> > ![http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/5.NewFolder.png](http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/5.NewFolder.png)
  1. Enter “model” for folder name, then click Finish

The project structure is generated, now you have to generate the blank model.

  1. Select File > New > Other
> > ![http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/6.NewIdemiaDiagramMenu.png](http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/6.NewIdemiaDiagramMenu.png)
  1. In New dialog, you will see a list of tools to create. Select “Idemia Diagram” from “Examples” folder, and click Next
> > ![http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/7.NewIdemiaDiagram.png](http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/7.NewIdemiaDiagram.png)
  1. In New Idemia Diagram dialog (Create Idemia Diagram), enter or select “model” folder
  1. Enter “pacman.idemia\_diagram” for file name, and click Next
> > ![http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/8.NewIdemiaDiagram(modelo).png](http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/8.NewIdemiaDiagram(modelo).png)
  1. In New Idemia Diagram dialog (Create Idemia Model), enter or  select “model” folder

> ![http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/9.NewIdemiaDiagram(diagrama).png](http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/9.NewIdemiaDiagram(diagrama).png)
  1. Enter “pacman.idemia” for file name, and then click Finish.

**Done! You are ready to model your Idemia solution!**

> ![http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/10.BlankIdemiaSolutionSnapshot.png](http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/10.BlankIdemiaSolutionSnapshot.png)


## Stage 2: Modeling Solution ##

As you know, IDEMIA support a complete solution integrated with only one Agent and one Environment.  It doesn’t restrict the number of relations (Actions and Perception) between them.

**Note:** To create the relation is necessary that Agent and Environment exists.


_Step 1: Modeling Agent and its Goal, State and Strategy_
  1. Agent
    1. Click in Agent button in the toolbar
    1. Press, and hold down the left button. Drag the figure to enlarge it and then drop it
    1. Enter "PacmanAgent" and press Enter
> > ![http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/11.PacmanAgent.png](http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/11.PacmanAgent.png)
  1. Agent Goal
    1. Click in Goal button in the toolbar
    1. Click in Goal Compartment, enter “PacmanGoal” and press Enter
> > ![http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/12.GoalState.png](http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/12.GoalState.png)
    1. Right Click in the goal, and select Show Properties View
    1. In Properties Area that appear, enter “(knownWorld = True) & (emptyWorld = True)” in Value property  and press Enter
> > ![http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/13.DataStructPacmanGoal.png](http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/13.DataStructPacmanGoal.png)
  1. Agent State
    1. Click in State button in the toolbar.
    1. Click in State Compartment, enter “PacmanState” and press Enter
> > ![http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/14.PacmanState.png](http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/14.PacmanState.png)
    1. Click in DataStructure button in the toolbar
    1. Click in State Compartment, enter “world” and press Enter
> > ![http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/15.DataStructPacmanState.png](http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/15.DataStructPacmanState.png)
    1. Right Click in the goal, and select Show Properties View
    1. In Properties Area that appear, select “matrix” value in Type
    1. Repeat last four items to create others DataStructure following the Pacman Example (names and types of DataStructure)
> > ![http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/16.CompleteDataStructPacmanState.png](http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/16.CompleteDataStructPacmanState.png)
  1. Agent Strategy
    1. Select Search button in the toolbar
    1. Click in StrategyCompartment, and press Enter (default search strategy is DeptFirstSearch)
> > ![http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/17.PacmanStrategy.png](http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/17.PacmanStrategy.png)
**Agent Done!**


_Step 2: Modeling Environment and its State_

  1. Environment Figure
    1. Click in Environment button in the toolbar.
    1. Press, and hold down the left button. Drag the figure to enlarge it and then drop it
    1. Enter “PacmanEnvironment” and press Enter
> > ![http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/18.PacmanEnvironment.png](http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/18.PacmanEnvironment.png)
  1. Environment State
    1. Click in State button in the toolbar
    1. Click in State Compartment, enter “EnvironmentState” and press Enter
> > ![http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/19.PacmanEnvironmentState.png](http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/19.PacmanEnvironmentState.png)
    1. Click in DataStructure button in the toolbar
    1. Click in State Compartment, enter “World”
> > ![http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/20.DataStructurePacmanEnvironmentState.png](http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/20.DataStructurePacmanEnvironmentState.png)
    1. Right Click in the goal, and select Show Properties View
    1. In Properties Area that appear, select “matrix” value in Type
    1. Repeat last four items to create the others DataStructure following the Pacman Example (names and types of DataStructure)
> > ![http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/21.CompleteDataStructurePacmanEnvironmentState.png](http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/21.CompleteDataStructurePacmanEnvironmentState.png)
**Environment Done!**


_Step 3: Modeling Relations_
  1. Actions
    1. Click in Action button in the toolbar
    1. Click in Agent Header and hold down, and then drop in Environment Header
    1. Enter “Flight” in action name, and press Enter
> > ![http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/22.Action.png](http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/22.Action.png)


> Repeat last threeitems to create the others Actions following the Pacman Example (actions names, pre and post conditions)

  1. Perceptions
    1. Click in Action button in the toolbar
    1. Click in Environment Header and hold down, and then drop in Agent Header
    1. Enter “energy” in action name, and press Enter
> > ![http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/23.Perception.png](http://idemia.googlecode.com/svn/wiki/images/How_to_use_IDEM-IA_Step_by_Step/23.Perception.png)


> Repeat last three items to create the others Perceptions following the Pacman Example (perceptions names)

**Relations Done!**