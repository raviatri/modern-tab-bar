# modern-tab-bar
To achieve synchronized scrolling in Flutter where both the parent widget and the child list inside TabBarView scroll together, you can use the NestedScrollView widget. This allows you to scroll a header (parent) and a body (TabBarView), where the header scrolls up and sticks to the top when the body (child) starts scrolling.

For detailed implementation check []

# Steps:
1. Use NestedScrollView: This widget allows you to scroll both the parent and child widgets in sync.
2. Set SliverAppBar for the Parent Scrollable Area: This widget will stick at the top once the parent is scrolled up.
3. Use TabBarView for the Children: The child widgets (lists) will be in a TabBarView.

# How It Works:
1. The parent widget is the SliverAppBar which contains an image and a title.
2. The TabBar sticks to the top once the SliverAppBar scrolls out of view.
3. Each tab contains a ListView, and when the child list scrolls, the parent also scrolls.


