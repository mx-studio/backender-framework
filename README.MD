## INSTALL

Install framework in current directory:

```composer create-project adjai/backender-framework .```

## CREATE ENTITIES

### CREATE CONTROLLER

```composer run-script create-controller```

### CREATE MODEL

```composer run-script create-model```

### CREATE CRUD AND MODEL

Create CRUD controller and model:

```composer run-script create-entity```

Methods for created CRUD controller:
- ```items($where = [], $fields = '*', $count = null, $orderBy = [], $groupBy = [], $ifCalcTotalRows = false, $page = 1)``` - list all items
- ```remove($id)```
- ```update($model)```, $model - array for adding / updating single row in model

For modifying CRUD methods override it and use appropriate trait method inside ($this->traitActionItems, $this->traitActionRemove, $this->traitActionUpdate).
