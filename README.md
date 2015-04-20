# popups
jq plug popups

/* ========================================================================
 *  tc: popups 扩展
 *  
 *  弹窗
 * 
 *  author: candy
 *
 *  version 0.0.1
 *
 * 结构：.ui-popups 
 *          .ui-popups-dialog
 *          .close
 *          .ui-popups-head
 *              .ui-popups-title
 *          .ui-popups-body
 *              .ui-popups-content
 *          .ui-popups-foot
 *
 * 
 * <div class="ui-popups">
        <div class="ui-popups-dialog">
            <em class="close" data-dismiss="popups">x</em>
            <div class="ui-popups-head">
                <h3 class="ui-popups-title">弹窗标题</h3>
            </div>
            <div class="ui-popups-body">
                <p>弹窗内容</p>
            </div>
            <div class="ui-popups-foot">
                <button class="btn btn-success" data-dismiss="popups">取消</button>
            </div>
        </div>
    </div>
 *
 *  标记：
 *  data-dismiss="popups"的元素点击会关闭父级弹窗
 *  data-ui="popups" data-target="#xxx"的元素点击会弹出#xxx元素弹窗
 *  
 *  $('#xxx').popups({scope: '#popups_dialog'}); // 手动调用
 * backdrop：显示背景遮罩层 默认true
 * scope：背景层范围（嵌套弹窗时用） 选择器
 * 
 *
 *
 * 回调：分别指显示前后，隐藏前后的回调， e.preventDefault(); // 阻止后续事件运行
 * 
 * show.tc.popups 
 * shown.tc.popups
 * hide.tc.popups
 * hiden.tc.popups
 * 
 *  
 * ======================================================================== */
