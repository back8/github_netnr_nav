# netnrnav
同步实现水平导航、垂直导航、侧滑导航，无限树形

> Demo: https://nav.netnr.com

### Html
```html
    <button type="button" class="MenuToggle show-in-mobile btn btn-primary">
        <span class="fa fa-align-justify fa-2x"></span>
    </button>
    <div id="netnrnav" class="netnrnav horizontal">
        <div class="netnrnav-wrapper">
            <ul>
            ...
            </ul>
        </div>
    </div>
```

### JavaScript
```javascript
<script type="text/javascript">
    var topbar = $('#netnrnav').netnrnav();
    $('.MenuToggle').click(topbar.toggle);
</script>
```

### 说明
- ` .netnrnav` 默认为垂直导航，为 `.netnrnav` 添加 `.horizontal` 后转为水平导航
    - 垂直导航、水平导航在分辨率<=768px时自动隐藏，转为侧滑导航
- `.hide-in-horizontal` 仅在垂直导航中显示，包括侧滑导航
- `.show-in-horizontal` 仅在水平导航中显示
- `.hide-in-mobile` 仅在>768px的屏幕显示
- `.show-in-mobile` 仅在<=768px的屏幕显示

### Fork
https://github.com/zhoufengjob/SuiNav