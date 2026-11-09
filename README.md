! uBlock Origin 自定义规则  2026/10/23
! uBlock origin 适用于chrome 140之前

! 【汽车之家】
! 右下角视频弹窗
autohome.com.cn##div[class^="style_video_player_container_"]
! 首页弹窗
autohome.com.cn##div.ant-modal[role="dialog"]
! 首页弹窗全屏遮罩 + 锁住鼠标滚动
autohome.com.cn##.ant-modal-root
autohome.com.cn##body:style(overflow: auto !important;)
autohome.com.cn##html:style(overflow: auto !important;)

! 【快科技】
! 新闻列表中的广告（关键词）
www.kkj.cn##li:has-text(/推荐|广告|广告|广告|广告|广告|广告/)
! 首页弹窗
www.kkj.cn##a[href*="jd.com"]
www.kkj.cn##div:has(> .jdong11_close)
www.kkj.cn##.HSsRgYjfNn
! 首页顶部
www.kkj.cn##.shidian
! 放久了的全屏弹窗
news.mydrivers.com###a_showhotnews_list
news.mydrivers.com###a_showhotnews_list_dia
news.mydrivers.com##.HSsRgYjfNn

! 【果核GHXI】
! 底部提示：
www.ghxi.com##div:has-text(网站上的恰饭广告)
! 置顶图片广告：
www.ghxi.com##div[class^="header-wrap"]
! 置顶推荐：
www.ghxi.com##div[class^="scroll-list"]
www.ghxi.com##div[class^="img-ad"]
www.ghxi.com##div[class^="card-list"]
www.ghxi.com##div[class^="img-ad"]
www.ghxi.com##div[class^="thematic-list"]
! 置顶文章广告：
www.ghxi.com##div.group:has(span:has-text(/置顶/))
! 关注微信的弹窗：
www.ghxi.com##div[class="gh-dialog gh-show"]
! 首页弹窗全屏遮罩 + 锁住鼠标滚动
ghxi.com###gh-container
!上面的如果不行，就用这个试试：ghxi.com##.gh-container.gh-show
ghxi.com##body:style(overflow: auto !important;)
ghxi.com##html:style(overflow: auto !important;)

! 【知乎】
! 知乎登录弹窗及右下角广告，并恢复鼠标上下滚动
zhihu.com##div[class^="Modal Modal--default signFlowModal"]
zhihu.com##html:style(overflow: auto !important)
zhihu.com##body:style(overflow: auto !important)
zhihu.com##.signFlowModal:style(display: none !important)
zhihu.com##div:has-text(登录即可查看)
zhuanlan.zhihu.com##.Modal-backdrop
zhuanlan.zhihu.com##.Modal-enter-done.undefined.Modal-wrapper

! 【小众软件】www.appinn.com
! 置顶图片广告：
appinn.com##div[style*="padding-top: 15px"][style*="width:600px"]
appinn.com##div[class="slider-container"]
! 文章列表的团购广告：
appinn.com##article:has(a[href*="group-get"])
