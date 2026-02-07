# Fork Changes Documentation

This document tracks all custom modifications, patches, and deviations from the upstream `serenader2014/flutter_carousel_slider` repository.

## Fork Information

- **Fork Repository**: `https://github.com/pieces-app/flutter_carousel_slider`
- **Upstream Repository**: `https://github.com/serenader2014/flutter_carousel_slider`
- **Current Branch**: `master`
- **Fork Version**: `4.1.1`
- **Commits Ahead**: 2
- **Commits Behind**: 37
- **Last Upstream Merge**: Fork created from upstream circa v4.1.1

## Custom Modifications

### 1. Carousel Controller Rename
- **Commit**: `63ed183`
- **Changes**:
  - Renamed carousel controller class to avoid naming conflicts
- **Files Modified**:
  - `lib/carousel_controller.dart` (62 lines changed)
  - `lib/carousel_options.dart` (26 lines changed)
  - `lib/carousel_slider.dart` (155 lines changed)
- **Reason**: The upstream controller name conflicted with another widget controller in the Pieces app

### 2. Dependency Updates
- **Commit**: `4e4c725`
- **Changes**: Updated dependencies for SDK compatibility

## Upstream Sync Status

- **Current Gap**: 37 commits behind upstream/master
- **Complexity**: MEDIUM -- controller rename needs to be re-applied after merge
- **Priority**: MEDIUM -- upstream has bug fixes and improvements

### Recommended Sync Approach
1. Fetch upstream master
2. Create merge branch
3. Resolve conflicts -- primarily re-apply controller rename
4. Test carousel functionality in Pieces app
5. Update this document

## Why This Fork Exists

1. **Controller Naming Conflict**: The upstream `CarouselController` name conflicts with another controller in the Pieces widget tree
2. **Historical**: Rename was necessary to avoid build errors

## Future Considerations

1. **Check Upstream**: Newer upstream versions may have renamed the controller or provide namespace options
2. **Upstream v2**: Monitor `feature/v2` branch on upstream for potential breaking changes
3. **Alternative Package**: Evaluate if other carousel packages avoid this naming issue

## Contact

For questions about this fork or to request changes, contact the Pieces development team.
