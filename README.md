## ExpandableListView + RecylerView (for child items with Horizontal Scroll)

### Screenshots

<img src="https://raw.github.com/sivailango/ExpandableListView-RecylerChildItems/master/screenshots/Screenshot_2016-03-02-13-43-43.png" width="320" alt="Screen shot 1">

<img src="https://raw.github.com/sivailango/ExpandableListView-RecylerChildItems/master/screenshots/Screenshot_2016-03-02-13-43-53.png" width="320" alt="Screen shot 1">

#### item_parent.xml  

Group header with custom indicator at Right hand side

#### item_group_child.xml  

RecyclerView to hold the all childs of its parent in Horizontal way

#### item_child.xml  

Child item layout

### BrandAdapter.java

```
@Override
public int getChildrenCount(int groupPosition) {
    return 1;
}
```

since the parent element going to have only one RecyclerView, so `return 1` for `getChildrenCount`
