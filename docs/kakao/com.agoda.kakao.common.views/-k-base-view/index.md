[kakao](../../index.md) / [com.agoda.kakao.common.views](../index.md) / [KBaseView](./index.md)

# KBaseView

`open class KBaseView<out T> : `[`BaseActions`](../../com.agoda.kakao.common.actions/-base-actions/index.md)`, `[`BaseAssertions`](../../com.agoda.kakao.common.assertions/-base-assertions/index.md)

Base class for all Kakao views

This base class allows create new custom view with ease. All you
have to do is to extend this class, implement all necessarily additional
actions/assertions interfaces and override necessary constructors

### Parameters

`T` - Type of your custom view. Needs to be defined to enable invoke() and perform() for descendants

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `KBaseView(function: `[`ViewBuilder`](../../com.agoda.kakao.common.builders/-view-builder/index.md)`.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`)`<br>Constructs view class with view interaction from given ViewBuilder`KBaseView(parent: Matcher<`[`View`](https://developer.android.com/reference/android/view/View.html)`>, function: `[`ViewBuilder`](../../com.agoda.kakao.common.builders/-view-builder/index.md)`.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`)`<br>`KBaseView(parent: DataInteraction, function: `[`ViewBuilder`](../../com.agoda.kakao.common.builders/-view-builder/index.md)`.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`)`<br>Constructs view class with parent and view interaction from given ViewBuilder |

### Properties

| Name | Summary |
|---|---|
| [root](root.md) | `open var root: Matcher<Root>` |
| [view](view.md) | `open val view: ViewInteraction` |

### Functions

| Name | Summary |
|---|---|
| [invoke](invoke.md) | `operator fun invoke(function: `[`T`](index.md#T)`.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Operator that allows usage of DSL style |
| [perform](perform.md) | `infix fun perform(function: `[`T`](index.md#T)`.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`T`](index.md#T)<br>Infix function for invoking lambda on your view |

### Inherited Functions

| Name | Summary |
|---|---|
| [act](../../com.agoda.kakao.common.actions/-base-actions/act.md) | `open fun act(function: () -> ViewAction): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Performs custom action on a view |
| [assert](../../com.agoda.kakao.common.assertions/-base-assertions/assert.md) | `open fun assert(function: () -> ViewAssertion): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Check the view with the given custom assertion |
| [click](../../com.agoda.kakao.common.actions/-base-actions/click.md) | `open fun click(location: GeneralLocation = GeneralLocation.VISIBLE_CENTER): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Performs click on view |
| [doesNotExist](../../com.agoda.kakao.common.assertions/-base-assertions/does-not-exist.md) | `open fun doesNotExist(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Checks if the matched view does not exist |
| [doubleClick](../../com.agoda.kakao.common.actions/-base-actions/double-click.md) | `open fun doubleClick(location: GeneralLocation = GeneralLocation.VISIBLE_CENTER): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Performs double click on view |
| [hasAnyTag](../../com.agoda.kakao.common.assertions/-base-assertions/has-any-tag.md) | `open fun hasAnyTag(vararg tags: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Checks if the view has at least one of the given tags |
| [hasBackgroundColor](../../com.agoda.kakao.common.assertions/-base-assertions/has-background-color.md) | `open fun hasBackgroundColor(resId: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>`open fun hasBackgroundColor(colorCode: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Checks if the view has given background color |
| [hasDescendant](../../com.agoda.kakao.common.assertions/-base-assertions/has-descendant.md) | `open fun hasDescendant(function: `[`ViewBuilder`](../../com.agoda.kakao.common.builders/-view-builder/index.md)`.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Checks if the view has given descendant |
| [hasNotDescendant](../../com.agoda.kakao.common.assertions/-base-assertions/has-not-descendant.md) | `open fun hasNotDescendant(function: `[`ViewBuilder`](../../com.agoda.kakao.common.builders/-view-builder/index.md)`.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Checks if the view has not given descendant |
| [hasNotSibling](../../com.agoda.kakao.common.assertions/-base-assertions/has-not-sibling.md) | `open fun hasNotSibling(function: `[`ViewBuilder`](../../com.agoda.kakao.common.builders/-view-builder/index.md)`.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Checks if the view has not given sibling |
| [hasSibling](../../com.agoda.kakao.common.assertions/-base-assertions/has-sibling.md) | `open fun hasSibling(function: `[`ViewBuilder`](../../com.agoda.kakao.common.builders/-view-builder/index.md)`.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Checks if the view has given sibling |
| [hasTag](../../com.agoda.kakao.common.assertions/-base-assertions/has-tag.md) | `open fun hasTag(tag: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Checks if the view has given tag |
| [inRoot](../../com.agoda.kakao.common.assertions/-base-assertions/in-root.md) | `open fun inRoot(function: `[`RootBuilder`](../../com.agoda.kakao.common.builders/-root-builder/index.md)`.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Check if the view is in given root |
| [isClickable](../../com.agoda.kakao.common.assertions/-base-assertions/is-clickable.md) | `open fun isClickable(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Checks if the view is clickable |
| [isCompletelyDisplayed](../../com.agoda.kakao.common.assertions/-base-assertions/is-completely-displayed.md) | `open fun isCompletelyDisplayed(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Checks if the view is completely displayed |
| [isDisabled](../../com.agoda.kakao.common.assertions/-base-assertions/is-disabled.md) | `open fun isDisabled(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Checks if the view is disabled |
| [isDisplayed](../../com.agoda.kakao.common.assertions/-base-assertions/is-displayed.md) | `open fun isDisplayed(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Checks if the view is displayed |
| [isEnabled](../../com.agoda.kakao.common.assertions/-base-assertions/is-enabled.md) | `open fun isEnabled(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Checks if the view is enabled |
| [isFocusable](../../com.agoda.kakao.common.assertions/-base-assertions/is-focusable.md) | `open fun isFocusable(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Checks if the view is focusable |
| [isFocused](../../com.agoda.kakao.common.assertions/-base-assertions/is-focused.md) | `open fun isFocused(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Checks if the view is focused |
| [isGone](../../com.agoda.kakao.common.assertions/-base-assertions/is-gone.md) | `open fun isGone(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Checks if the view has GONE visibility |
| [isInvisible](../../com.agoda.kakao.common.assertions/-base-assertions/is-invisible.md) | `open fun isInvisible(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Checks if the view has INVISIBLE visibility |
| [isNotClickable](../../com.agoda.kakao.common.assertions/-base-assertions/is-not-clickable.md) | `open fun isNotClickable(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Checks if the view is not clickable |
| [isNotCompletelyDisplayed](../../com.agoda.kakao.common.assertions/-base-assertions/is-not-completely-displayed.md) | `open fun isNotCompletelyDisplayed(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Checks if the view is not completely displayed |
| [isNotDisplayed](../../com.agoda.kakao.common.assertions/-base-assertions/is-not-displayed.md) | `open fun isNotDisplayed(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Checks if the view is not displayed |
| [isNotFocusable](../../com.agoda.kakao.common.assertions/-base-assertions/is-not-focusable.md) | `open fun isNotFocusable(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Checks if the view is not focusable |
| [isNotFocused](../../com.agoda.kakao.common.assertions/-base-assertions/is-not-focused.md) | `open fun isNotFocused(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Checks if the view is not focused |
| [isNotSelected](../../com.agoda.kakao.common.assertions/-base-assertions/is-not-selected.md) | `open fun isNotSelected(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Checks if the view is not selected |
| [isSelected](../../com.agoda.kakao.common.assertions/-base-assertions/is-selected.md) | `open fun isSelected(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Checks if the view is selected |
| [isVisible](../../com.agoda.kakao.common.assertions/-base-assertions/is-visible.md) | `open fun isVisible(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Checks if the view has VISIBLE visibility |
| [longClick](../../com.agoda.kakao.common.actions/-base-actions/long-click.md) | `open fun longClick(location: GeneralLocation = GeneralLocation.VISIBLE_CENTER): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Performs long click on view |
| [matches](../../com.agoda.kakao.common.assertions/-base-assertions/matches.md) | `open fun matches(function: `[`ViewBuilder`](../../com.agoda.kakao.common.builders/-view-builder/index.md)`.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Check if the view matches given matcher |
| [notMatches](../../com.agoda.kakao.common.assertions/-base-assertions/not-matches.md) | `open fun notMatches(function: `[`ViewBuilder`](../../com.agoda.kakao.common.builders/-view-builder/index.md)`.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Check if the view does not match given matcher |
| [onFailure](../../com.agoda.kakao.common.actions/-base-actions/on-failure.md) | `open fun onFailure(function: (error: `[`Throwable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-throwable/index.html)`, matcher: Matcher<`[`View`](https://developer.android.com/reference/android/view/View.html)`>) -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Adds failure handler to the view |
| [pressImeAction](../../com.agoda.kakao.common.actions/-base-actions/press-ime-action.md) | `open fun pressImeAction(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Presses IME action, if supported view is in focus |
| [repeatUntil](../../com.agoda.kakao.common.actions/-base-actions/repeat-until.md) | `open fun repeatUntil(maxAttempts: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)` = 1, action: () -> ViewAction, matcher: `[`ViewBuilder`](../../com.agoda.kakao.common.builders/-view-builder/index.md)`.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Repeats given action on the view until this view will match the given matcher |
| [scrollTo](../../com.agoda.kakao.common.actions/-base-actions/scroll-to.md) | `open fun scrollTo(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Scrolls to the view, if possible |

### Inheritors

| Name | Summary |
|---|---|
| [KBottomNavigationView](../../com.agoda.kakao.bottomnav/-k-bottom-navigation-view/index.md) | `class KBottomNavigationView : `[`KBaseView`](./index.md)`<`[`KBottomNavigationView`](../../com.agoda.kakao.bottomnav/-k-bottom-navigation-view/index.md)`>, `[`BottomNavigationViewActions`](../../com.agoda.kakao.bottomnav/-bottom-navigation-view-actions/index.md)`, `[`BottomNavigationViewAssertions`](../../com.agoda.kakao.bottomnav/-bottom-navigation-view-assertions/index.md)<br>View for acting and asserting on BottomNavigationView |
| [KButton](../../com.agoda.kakao.text/-k-button/index.md) | `class KButton : `[`KBaseView`](./index.md)`<`[`KButton`](../../com.agoda.kakao.text/-k-button/index.md)`>, `[`TextViewAssertions`](../../com.agoda.kakao.text/-text-view-assertions/index.md)<br>View with BaseActions and TextViewAssertions |
| [KCheckBox](../../com.agoda.kakao.check/-k-check-box/index.md) | `class KCheckBox : `[`KBaseView`](./index.md)`<`[`KCheckBox`](../../com.agoda.kakao.check/-k-check-box/index.md)`>, `[`CheckableActions`](../../com.agoda.kakao.check/-checkable-actions/index.md)`, `[`TextViewAssertions`](../../com.agoda.kakao.text/-text-view-assertions/index.md)`, `[`CheckableAssertions`](../../com.agoda.kakao.check/-checkable-assertions/index.md)<br>View with CheckableActions, CheckableAssertions and TextViewAssertions |
| [KDrawerView](../../com.agoda.kakao.drawer/-k-drawer-view/index.md) | `class KDrawerView : `[`KBaseView`](./index.md)`<`[`KDrawerView`](../../com.agoda.kakao.drawer/-k-drawer-view/index.md)`>, `[`DrawerActions`](../../com.agoda.kakao.drawer/-drawer-actions/index.md)<br>View with DrawerActions and BaseAssertions |
| [KEditText](../../com.agoda.kakao.edit/-k-edit-text/index.md) | `class KEditText : `[`KBaseView`](./index.md)`<`[`KEditText`](../../com.agoda.kakao.edit/-k-edit-text/index.md)`>, `[`EditableActions`](../../com.agoda.kakao.edit/-editable-actions/index.md)`, `[`EditableAssertions`](../../com.agoda.kakao.edit/-editable-assertions/index.md)<br>View with EditableActions and EditableAssertions |
| [KImageView](../../com.agoda.kakao.image/-k-image-view/index.md) | `class KImageView : `[`KBaseView`](./index.md)`<`[`KImageView`](../../com.agoda.kakao.image/-k-image-view/index.md)`>, `[`ImageViewAssertions`](../../com.agoda.kakao.image/-image-view-assertions/index.md)<br>View with BaseActions and ImageViewAssertions |
| [KNavigationView](../../com.agoda.kakao.navigation/-k-navigation-view/index.md) | `class KNavigationView : `[`KBaseView`](./index.md)`<`[`KNavigationView`](../../com.agoda.kakao.navigation/-k-navigation-view/index.md)`>, `[`NavigationViewActions`](../../com.agoda.kakao.navigation/-navigation-view-actions/index.md)`, `[`NavigationViewAssertions`](../../com.agoda.kakao.navigation/-navigation-view-assertions/index.md)<br>View with NavigationViewActions and NavigationViewAssertions |
| [KProgressBar](../../com.agoda.kakao.progress/-k-progress-bar/index.md) | `class KProgressBar : `[`KBaseView`](./index.md)`<`[`KProgressBar`](../../com.agoda.kakao.progress/-k-progress-bar/index.md)`>, `[`ProgressBarActions`](../../com.agoda.kakao.progress/-progress-bar-actions/index.md)`, `[`ProgressBarAssertions`](../../com.agoda.kakao.progress/-progress-bar-assertions/index.md)<br>View with ProgressBarActions and ProgressBarAssertions |
| [KRatingBar](../../com.agoda.kakao.rating/-k-rating-bar/index.md) | `class KRatingBar : `[`KBaseView`](./index.md)`<`[`KRatingBar`](../../com.agoda.kakao.rating/-k-rating-bar/index.md)`>, `[`RatingBarActions`](../../com.agoda.kakao.rating/-rating-bar-actions/index.md)`, `[`RatingBarAssertions`](../../com.agoda.kakao.rating/-rating-bar-assertions/index.md)<br>View with RatingBarActions and RatingBarAssertions |
| [KSeekBar](../../com.agoda.kakao.progress/-k-seek-bar/index.md) | `class KSeekBar : `[`KBaseView`](./index.md)`<`[`KSeekBar`](../../com.agoda.kakao.progress/-k-seek-bar/index.md)`>, `[`SeekBarActions`](../../com.agoda.kakao.progress/-seek-bar-actions/index.md)`, `[`ProgressBarAssertions`](../../com.agoda.kakao.progress/-progress-bar-assertions/index.md)<br>View with SeekBarActions and ProgressBarAssertions |
| [KSnackbar](../../com.agoda.kakao.text/-k-snackbar/index.md) | `class KSnackbar : `[`KBaseView`](./index.md)`<`[`KSnackbar`](../../com.agoda.kakao.text/-k-snackbar/index.md)`>`<br>View with internal TextView and a Button |
| [KSwipeRefreshLayout](../../com.agoda.kakao.swiperefresh/-k-swipe-refresh-layout/index.md) | `class KSwipeRefreshLayout : `[`KBaseView`](./index.md)`<`[`KSwipeRefreshLayout`](../../com.agoda.kakao.swiperefresh/-k-swipe-refresh-layout/index.md)`>, `[`SwipeRefreshLayoutActions`](../../com.agoda.kakao.swiperefresh/-swipe-refresh-layout-actions/index.md)`, `[`SwipeRefreshLayoutAssertions`](../../com.agoda.kakao.swiperefresh/-swipe-refresh-layout-assertions/index.md)<br>View with SwipeRefreshLayoutActions and SwipeRefreshLayoutAssertions |
| [KSwipeView](../-k-swipe-view/index.md) | `class KSwipeView : `[`KBaseView`](./index.md)`<`[`KSwipeView`](../-k-swipe-view/index.md)`>, `[`SwipeableActions`](../../com.agoda.kakao.common.actions/-swipeable-actions/index.md)<br>View with SwipeableActions and BaseAssertions |
| [KTabLayout](../../com.agoda.kakao.tabs/-k-tab-layout/index.md) | `class KTabLayout : `[`KBaseView`](./index.md)`<`[`KTabLayout`](../../com.agoda.kakao.tabs/-k-tab-layout/index.md)`>, `[`TabLayoutActions`](../../com.agoda.kakao.tabs/-tab-layout-actions/index.md)`, `[`TabLayoutAssertions`](../../com.agoda.kakao.tabs/-tab-layout-assertions/index.md)<br>View with TabLayoutActions and TabLayoutAssertions |
| [KTextInputLayout](../../com.agoda.kakao.edit/-k-text-input-layout/index.md) | `class KTextInputLayout : `[`KBaseView`](./index.md)`<`[`KTextInputLayout`](../../com.agoda.kakao.edit/-k-text-input-layout/index.md)`>, `[`TextInputLayoutAssertions`](../../com.agoda.kakao.edit/-text-input-layout-assertions/index.md)<br>View with TextInputLayoutAssertions |
| [KTextView](../../com.agoda.kakao.text/-k-text-view/index.md) | `class KTextView : `[`KBaseView`](./index.md)`<`[`KTextView`](../../com.agoda.kakao.text/-k-text-view/index.md)`>, `[`TextViewActions`](../../com.agoda.kakao.text/-text-view-actions/index.md)`, `[`TextViewAssertions`](../../com.agoda.kakao.text/-text-view-assertions/index.md)<br>View with BaseActions and TextViewAssertions |
| [KView](../-k-view/index.md) | `class KView : `[`KBaseView`](./index.md)`<`[`KView`](../-k-view/index.md)`>`<br>Simple view with BaseActions and BaseAssertions |
| [KViewPager](../../com.agoda.kakao.pager/-k-view-pager/index.md) | `class KViewPager : `[`KBaseView`](./index.md)`<`[`KViewPager`](../../com.agoda.kakao.pager/-k-view-pager/index.md)`>, `[`SwipeableActions`](../../com.agoda.kakao.common.actions/-swipeable-actions/index.md)`, `[`ViewPagerAssertions`](../../com.agoda.kakao.pager/-view-pager-assertions/index.md)<br>View with SwipeableActions and ViewPagerAssertions |