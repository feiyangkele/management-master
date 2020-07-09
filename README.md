# management-master
本小区物业管理系统分成两种角色，分别是小区业主和小区物业管理员，小区业主登录系统后可以投诉、维修上报、查看账单、登录注册等；管理员登录系统后可以对用户进行管理，并且可以对车位、房屋、缴费、社区服务等进行管理。小区物业管理系统使用Java语言开发，使用IDEA的开发平台，通过Tomcat服务器发布项目，使用的架构为B/S架构。

#### 系统功能设计

##### 1、登录模块
小区物业管理系统面向两种角色：管理员、小区业主。两者都是经由一个登陆入口登陆系统，通过该登陆模块，用户输入账户密码且选择登陆角色后可以登录系统，根据用户的权限进行相应的管理操作。

<div align=center><img src="http://tiebapic.baidu.com/forum/w%3D580/sign=3fa880119cd4b31cf03c94b3b7d7276f/b0b91bdfa9ec8a131662ccb2e003918fa1ecc0fa.jpg"/></div>

##### 2、我的维修模块
我的维修模块面向业主的功能是维修信息提报，业主可以添加维修信息，并且可以查看相应的维修信息；管理员通过自己的社区服务的功能模块下的维修管理，可以查看业主所提交的维修信息，并且可以对维修信息进行维护、修改。

##### 3、用户系统模块
用户系统模块是面向管理员使用的模块，本模块的主要功能是用户管理，管理员可以通过本模块添加业主，添加的业主信息包括用户名、手机号、性别等；通过本模块管理员可以对用户的车位、房屋进行停用，并且可以管理房屋分配、车位分配、缴费管理等。管理员还可以修改业主信息，还可以删除业主信息。

<div align=center><img src="http://tiebapic.baidu.com/forum/w%3D580/sign=64463fedb7ec08fa260013af69ef3d4d/599c6163f6246b609f762926fcf81a4c500fa2fa.jpg"/></div>

##### 4、房屋系统模块
房屋系统模块是面向管理员使用的模块，本模块的主要功能是楼栋管理、单元管理、房屋管理三个子模块；楼栋管理包括对小区的楼栋进行添加、修改、删除等；单元管理是对小区内所有的单元信息进行管理的模块，管理员可以添加单元、修改单元信息、删除单元信息等；房屋管理是对小区内所有的房屋信息进行管理，包括添加房间名、房间面积、状态等信息。

<div align=center><img src="http://tiebapic.baidu.com/forum/w%3D580/sign=453f74d65ded2e73fce98624b700a16d/854cf8d3572c11dfdaa92471742762d0f603c2fa.jpg"/></div>

##### 5、车位系统模块
车位系统模块主要的功能是对车位信息进行管理，管理员可以添加所有的车位信息，并且可以条件查询车位信息。管理员也可以对车位信息进行分配，并且可以修改车位信息、删除车位信息。

<div align=center><img src="http://tiebapic.baidu.com/forum/w%3D580/sign=aef1e48f39738bd4c421b239918a876c/15465d2c11dfa9ecfe56cd4575d0f703908fc1fa.jpg"/></div>

##### 6、缴费系统模块
缴费系统模块也是面向管理员使用的模块，主要功能包括缴费类型、缴费管理。缴费类型包括对于物业收费的类型，包括水费、电费、物业费等；缴费管理包括查看业主本月是否缴费，并且可也确认业主缴费。

<div align=center><img src="http://tiebapic.baidu.com/forum/w%3D580/sign=f45d9818cdb44aed594ebeec831d876a/ed4468d9f2d3572c639a078e9d13632763d0c3fa.jpg"/></div>

##### 7、个人中心模块
个人中心模块是管理员及用户都有的模块，通过本模块无论是管理员还是用户都可以对个人信息进行管理，并且可以进行维护。

<div align=center><img src="http://tiebapic.baidu.com/forum/w%3D580/sign=583625b6a41c8701d6b6b2ee177e9e6e/f64aa3ec8a13632714955961868fa0ec09fac7fa.jpg"/></div>


<div class="repository-content ">

    
    

  <div class="d-none d-lg-block mt-6 mr-3 Popover top-0 right-0 box-shadow-medium col-3">
    
  </div>

  



  <div class="gutter-condensed gutter-lg d-flex flex-column flex-md-row">

  <div class="flex-shrink-0 col-12 col-md-9 mb-4 mb-md-0">
    



        

      <div class="file-navigation mb-3 d-flex flex-items-start">
  
<details class="details-reset details-overlay mr-0 mb-0 " id="branch-select-menu">
  <summary class="btn css-truncate" data-hotkey="w" title="Switch branches or tags" aria-haspopup="menu" role="button">
    <svg height="16" class="octicon octicon-git-branch text-gray" text="gray" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M11.75 2.5a.75.75 0 100 1.5.75.75 0 000-1.5zm-2.25.75a2.25 2.25 0 113 2.122V6A2.5 2.5 0 0110 8.5H6a1 1 0 00-1 1v1.128a2.251 2.251 0 11-1.5 0V5.372a2.25 2.25 0 111.5 0v1.836A2.492 2.492 0 016 7h4a1 1 0 001-1v-.628A2.25 2.25 0 019.5 3.25zM4.25 12a.75.75 0 100 1.5.75.75 0 000-1.5zM3.5 3.25a.75.75 0 111.5 0 .75.75 0 01-1.5 0z"></path></svg>

      <i class="d-none d-lg-inline">Branch:</i>
    <span class="css-truncate-target" data-menu-button="">master</span>
    <span class="dropdown-caret"></span>
  </summary>

  <details-menu class="SelectMenu SelectMenu--hasFilter" src="/fuzhengwei/CodeGuide/refs/master?source_action=disambiguate&amp;source_controller=files" preload="" role="menu">
    <div class="SelectMenu-modal">
      <include-fragment class="SelectMenu-loading" aria-label="Menu is loading">
        <svg class="octicon octicon-octoface anim-pulse" height="32" viewBox="0 0 16 16" version="1.1" width="32" aria-hidden="true"><path fill-rule="evenodd" d="M14.7 5.34c.13-.32.55-1.59-.13-3.31 0 0-1.05-.33-3.44 1.3-1-.28-2.07-.32-3.13-.32s-2.13.04-3.13.32c-2.39-1.64-3.44-1.3-3.44-1.3-.68 1.72-.26 2.99-.13 3.31C.49 6.21 0 7.33 0 8.69 0 13.84 3.33 15 7.98 15S16 13.84 16 8.69c0-1.36-.49-2.48-1.3-3.35zM8 14.02c-3.3 0-5.98-.15-5.98-3.35 0-.76.38-1.48 1.02-2.07 1.07-.98 2.9-.46 4.96-.46 2.07 0 3.88-.52 4.96.46.65.59 1.02 1.3 1.02 2.07 0 3.19-2.68 3.35-5.98 3.35zM5.49 9.01c-.66 0-1.2.8-1.2 1.78s.54 1.79 1.2 1.79c.66 0 1.2-.8 1.2-1.79s-.54-1.78-1.2-1.78zm5.02 0c-.66 0-1.2.79-1.2 1.78s.54 1.79 1.2 1.79c.66 0 1.2-.8 1.2-1.79s-.53-1.78-1.2-1.78z"></path></svg>
      </include-fragment>
    </div>
  </details-menu>
</details>



  <div class="flex-auto"></div>

  <a class="btn mr-2 d-none d-md-block" data-hydro-click="{&quot;event_type&quot;:&quot;repository.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;FIND_FILE_BUTTON&quot;,&quot;repository_id&quot;:255558345,&quot;originating_url&quot;:&quot;https://github.com/fuzhengwei/CodeGuide&quot;,&quot;user_id&quot;:67892538}}" data-hydro-click-hmac="56547359bc652e5012bb4719149762061c7ebaabbd82b566e246065af42fdeab" data-ga-click="Repository, find file, location:repo overview" data-hotkey="t" data-pjax="true" href="/fuzhengwei/CodeGuide/find/master">
    Go to file
</a>
    <details class="details-overlay details-reset position-relative">
  <summary role="button">
            <span class="btn d-none d-md-flex flex-items-center">
          Add file
          <span class="dropdown-caret ml-1"></span>
        </span>
        <span class="btn d-inline-block d-md-none">
          <svg height="16" class="octicon octicon-kebab-horizontal" aria-label="More options" viewBox="0 0 16 16" version="1.1" width="16" role="img"><path d="M8 9a1.5 1.5 0 100-3 1.5 1.5 0 000 3zM1.5 9a1.5 1.5 0 100-3 1.5 1.5 0 000 3zm13 0a1.5 1.5 0 100-3 1.5 1.5 0 000 3z"></path></svg>

        </span>

</summary>
          <ul class="dropdown-menu dropdown-menu-sw">
          <li class="d-block d-md-none">
            <a class="dropdown-item" data-hydro-click="{&quot;event_type&quot;:&quot;repository.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;FIND_FILE_BUTTON&quot;,&quot;repository_id&quot;:255558345,&quot;originating_url&quot;:&quot;https://github.com/fuzhengwei/CodeGuide&quot;,&quot;user_id&quot;:67892538}}" data-hydro-click-hmac="56547359bc652e5012bb4719149762061c7ebaabbd82b566e246065af42fdeab" data-ga-click="Repository, find file, location:repo overview" data-hotkey="t" data-pjax="true" href="/fuzhengwei/CodeGuide/find/master">
              Go to file
</a>          </li>
          <li class="d-block d-md-none dropdown-divider" role="none"></li>
          
  <li><!-- '"` --><!-- </textarea></xmp> --><form action="/fuzhengwei/CodeGuide/new/master" accept-charset="UTF-8" method="post"><input type="hidden" name="authenticity_token" value="6k0Cl5KEwZvSKhnliu+MdgIHOqUV6iFv5a75/sPQ2ECuxD0sXpOJbUHTUB2jmY4PM30bvi25T9yvaKwZvaEoqw==">
    <button class="dropdown-item btn-link" type="submit">
      Create new file
    </button>
  </form></li>


          
  <li><a href="/fuzhengwei/CodeGuide/upload/master" class="dropdown-item">
    Upload files
  </a></li>

        </ul>

</details>



    <span class="d-none d-md-flex">
        
<get-repo>
  <details class="position-relative details-overlay details-reset" data-action="toggle:get-repo#onDetailsToggle">
    <summary class="btn ml-2 btn-primary" data-hydro-click="{&quot;event_type&quot;:&quot;repository.click&quot;,&quot;payload&quot;:{&quot;repository_id&quot;:255558345,&quot;target&quot;:&quot;CLONE_OR_DOWNLOAD_BUTTON&quot;,&quot;originating_url&quot;:&quot;https://github.com/fuzhengwei/CodeGuide&quot;,&quot;user_id&quot;:67892538}}" data-hydro-click-hmac="5516214c0b96c2c389c4b9e40c69869e556d08c71c111fecdc1719b17957cc0a">
      <svg class="octicon octicon-download mr-1" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.47 10.78a.75.75 0 001.06 0l3.75-3.75a.75.75 0 00-1.06-1.06L8.75 8.44V1.75a.75.75 0 00-1.5 0v6.69L4.78 5.97a.75.75 0 00-1.06 1.06l3.75 3.75zM3.75 13a.75.75 0 000 1.5h8.5a.75.75 0 000-1.5h-8.5z"></path></svg>
      Code
      <span class="dropdown-caret"></span>
</summary>    <div class="position-relative">
      <div class="get-repo-modal dropdown-menu dropdown-menu-sw p-0 js-toggler-container " style="top:6px;width:352px;">
        <div data-target="get-repo.modal">
          <div class="border-bottom p-3">
              <div class="https-clone-options">
                  <!-- '"` --><!-- </textarea></xmp> --><form data-remote="true" action="/users/set_protocol?protocol_selector=ssh&amp;protocol_type=clone" accept-charset="UTF-8" method="post"><input type="hidden" name="authenticity_token" value="2BfqwMqZLhaDmfT6URSLjvJcrCffCTZuQVmN6663yysCzpVbhfu7HsGfYhy6/ZjHTWjKvx9f3pVtmI7UuE2xIA=="><button name="button" type="submit" data-hydro-click="{&quot;event_type&quot;:&quot;clone_or_download.click&quot;,&quot;payload&quot;:{&quot;feature_clicked&quot;:&quot;USE_SSH&quot;,&quot;git_repository_type&quot;:&quot;REPOSITORY&quot;,&quot;repository_id&quot;:255558345,&quot;originating_url&quot;:&quot;https://github.com/fuzhengwei/CodeGuide&quot;,&quot;user_id&quot;:67892538}}" data-hydro-click-hmac="b633c8af645dd2651561838bf0c626f345a00d61e61bb7a25dde2a810e381e1a" class="btn-link f6 js-toggler-target float-right">Use SSH</button></form>

                <h4 class="mb-1">
                  Clone with HTTPS
                  <a class="muted-link" href="https://help.github.com/articles/which-remote-url-should-i-use" target="_blank" title="Which remote URL should I use?">
                    <svg class="octicon octicon-question" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8 1.5a6.5 6.5 0 100 13 6.5 6.5 0 000-13zM0 8a8 8 0 1116 0A8 8 0 010 8zm9 3a1 1 0 11-2 0 1 1 0 012 0zM6.92 6.085c.081-.16.19-.299.34-.398.145-.097.371-.187.74-.187.28 0 .553.087.738.225A.613.613 0 019 6.25c0 .177-.04.264-.077.318a.956.956 0 01-.277.245c-.076.051-.158.1-.258.161l-.007.004a7.728 7.728 0 00-.313.195 2.416 2.416 0 00-.692.661.75.75 0 001.248.832.956.956 0 01.276-.245 6.3 6.3 0 01.26-.16l.006-.004c.093-.057.204-.123.313-.195.222-.149.487-.355.692-.662.214-.32.329-.702.329-1.15 0-.76-.36-1.348-.863-1.725A2.76 2.76 0 008 4c-.631 0-1.155.16-1.572.438-.413.276-.68.638-.849.977a.75.75 0 101.342.67z"></path></svg>
                  </a>
                </h4>
                <p class="mb-2 f5">
                  Use Git or checkout with SVN using the web URL.
                </p>

                <div class="input-group">
  <input type="text" class="form-control input-monospace input-sm" data-autoselect="" value="https://github.com/fuzhengwei/CodeGuide.git" aria-label="Clone this repository at https://github.com/fuzhengwei/CodeGuide.git" readonly="">
  <div class="input-group-button">
    <clipboard-copy value="https://github.com/fuzhengwei/CodeGuide.git" aria-label="Copy to clipboard" class="btn btn-sm" data-hydro-click="{&quot;event_type&quot;:&quot;clone_or_download.click&quot;,&quot;payload&quot;:{&quot;feature_clicked&quot;:&quot;COPY_URL&quot;,&quot;git_repository_type&quot;:&quot;REPOSITORY&quot;,&quot;repository_id&quot;:255558345,&quot;originating_url&quot;:&quot;https://github.com/fuzhengwei/CodeGuide&quot;,&quot;user_id&quot;:67892538}}" data-hydro-click-hmac="56dfa9440116868189da68804c89b2e6bb5ca6cda30a6a71e9a5d209c3a6e576" tabindex="0" role="button"><svg class="octicon octicon-clippy" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M5.75 1a.75.75 0 00-.75.75v3c0 .414.336.75.75.75h4.5a.75.75 0 00.75-.75v-3a.75.75 0 00-.75-.75h-4.5zm.75 3V2.5h3V4h-3zm-2.874-.467a.75.75 0 00-.752-1.298A1.75 1.75 0 002 3.75v9.5c0 .966.784 1.75 1.75 1.75h8.5A1.75 1.75 0 0014 13.25v-9.5a1.75 1.75 0 00-.874-1.515.75.75 0 10-.752 1.298.25.25 0 01.126.217v9.5a.25.25 0 01-.25.25h-8.5a.25.25 0 01-.25-.25v-9.5a.25.25 0 01.126-.217z"></path></svg></clipboard-copy>
  </div>
</div>

              </div>

              <div class="ssh-clone-options">
                  <!-- '"` --><!-- </textarea></xmp> --><form data-remote="true" action="/users/set_protocol?protocol_selector=https&amp;protocol_type=clone" accept-charset="UTF-8" method="post"><input type="hidden" name="authenticity_token" value="fdAEAIHe+uLbTPKB0qDDUW+a2gC4mSv6H3SpSz7L7J2nCXubzrxv6plKZGc5SdAY0K68mHjPwwEztap0KDGWlg=="><button name="button" type="submit" data-hydro-click="{&quot;event_type&quot;:&quot;clone_or_download.click&quot;,&quot;payload&quot;:{&quot;feature_clicked&quot;:&quot;USE_HTTPS&quot;,&quot;git_repository_type&quot;:&quot;REPOSITORY&quot;,&quot;repository_id&quot;:255558345,&quot;originating_url&quot;:&quot;https://github.com/fuzhengwei/CodeGuide&quot;,&quot;user_id&quot;:67892538}}" data-hydro-click-hmac="5b15172640cc5cafb87e00324b994429b1956b72a7f84d83036e937d343099be" class="btn-link f6 js-toggler-target float-right">Use HTTPS</button></form>
                  <h4 class="mb-1">
                    Clone with SSH
                    <a class="muted-link" href="https://help.github.com/articles/which-remote-url-should-i-use" target="_blank" title="Which remote URL should I use?">
                      <svg class="octicon octicon-question" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8 1.5a6.5 6.5 0 100 13 6.5 6.5 0 000-13zM0 8a8 8 0 1116 0A8 8 0 010 8zm9 3a1 1 0 11-2 0 1 1 0 012 0zM6.92 6.085c.081-.16.19-.299.34-.398.145-.097.371-.187.74-.187.28 0 .553.087.738.225A.613.613 0 019 6.25c0 .177-.04.264-.077.318a.956.956 0 01-.277.245c-.076.051-.158.1-.258.161l-.007.004a7.728 7.728 0 00-.313.195 2.416 2.416 0 00-.692.661.75.75 0 001.248.832.956.956 0 01.276-.245 6.3 6.3 0 01.26-.16l.006-.004c.093-.057.204-.123.313-.195.222-.149.487-.355.692-.662.214-.32.329-.702.329-1.15 0-.76-.36-1.348-.863-1.725A2.76 2.76 0 008 4c-.631 0-1.155.16-1.572.438-.413.276-.68.638-.849.977a.75.75 0 101.342.67z"></path></svg>
                    </a>
                  </h4>

                    <div class="flash flash-warn my-3">
                      You don't have any public SSH keys in your GitHub account.
                      You can <a href="/settings/ssh/new">add a new public key</a>, or try cloning this repository via <button type="button" class="btn-link js-toggler-target">HTTPS.</button>
                    </div>

                  <p class="mb-2 f5">
                      Use a password protected SSH key.
                  </p>

                  <div class="input-group">
  <input type="text" class="form-control input-monospace input-sm" data-autoselect="" value="git@github.com:fuzhengwei/CodeGuide.git" aria-label="Clone this repository at git@github.com:fuzhengwei/CodeGuide.git" readonly="">
  <div class="input-group-button">
    <clipboard-copy value="git@github.com:fuzhengwei/CodeGuide.git" aria-label="Copy to clipboard" class="btn btn-sm" data-hydro-click="{&quot;event_type&quot;:&quot;clone_or_download.click&quot;,&quot;payload&quot;:{&quot;feature_clicked&quot;:&quot;COPY_URL&quot;,&quot;git_repository_type&quot;:&quot;REPOSITORY&quot;,&quot;repository_id&quot;:255558345,&quot;originating_url&quot;:&quot;https://github.com/fuzhengwei/CodeGuide&quot;,&quot;user_id&quot;:67892538}}" data-hydro-click-hmac="56dfa9440116868189da68804c89b2e6bb5ca6cda30a6a71e9a5d209c3a6e576" tabindex="0" role="button"><svg class="octicon octicon-clippy" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M5.75 1a.75.75 0 00-.75.75v3c0 .414.336.75.75.75h4.5a.75.75 0 00.75-.75v-3a.75.75 0 00-.75-.75h-4.5zm.75 3V2.5h3V4h-3zm-2.874-.467a.75.75 0 00-.752-1.298A1.75 1.75 0 002 3.75v9.5c0 .966.784 1.75 1.75 1.75h8.5A1.75 1.75 0 0014 13.25v-9.5a1.75 1.75 0 00-.874-1.515.75.75 0 10-.752 1.298.25.25 0 01.126.217v9.5a.25.25 0 01-.25.25h-8.5a.25.25 0 01-.25-.25v-9.5a.25.25 0 01.126-.217z"></path></svg></clipboard-copy>
  </div>
</div>

              </div>
          </div>
          <ul class="list-style-none">
            <li data-platforms="windows,mac" class="Box-row Box-row--hover-gray p-0 rounded-0 mt-0 js-remove-unless-platform">
              <a class="d-flex flex-items-center text-gray-dark text-bold no-underline p-3" data-hydro-click="{&quot;event_type&quot;:&quot;clone_or_download.click&quot;,&quot;payload&quot;:{&quot;feature_clicked&quot;:&quot;OPEN_IN_DESKTOP&quot;,&quot;git_repository_type&quot;:&quot;REPOSITORY&quot;,&quot;repository_id&quot;:255558345,&quot;originating_url&quot;:&quot;https://github.com/fuzhengwei/CodeGuide&quot;,&quot;user_id&quot;:67892538}}" data-hydro-click-hmac="9b95852fa751faaa7e2b1ef02d5fbda62f1526076410855d8f01c6ab01df0026" data-action="click:get-repo#showDownloadMessage" href="x-github-client://openRepo/https://github.com/fuzhengwei/CodeGuide">
                <svg class="octicon octicon-desktop-download mr-3" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.75 5V.75a.75.75 0 00-1.5 0V5H5.104a.25.25 0 00-.177.427l2.896 2.896a.25.25 0 00.354 0l2.896-2.896A.25.25 0 0010.896 5H8.75zM1.5 2.75a.25.25 0 01.25-.25h3a.75.75 0 000-1.5h-3A1.75 1.75 0 000 2.75v7.5C0 11.216.784 12 1.75 12h3.727c-.1 1.041-.52 1.872-1.292 2.757A.75.75 0 004.75 16h6.5a.75.75 0 00.565-1.243c-.772-.885-1.193-1.716-1.292-2.757h3.727A1.75 1.75 0 0016 10.25v-7.5A1.75 1.75 0 0014.25 1h-3a.75.75 0 000 1.5h3a.25.25 0 01.25.25v7.5a.25.25 0 01-.25.25H1.75a.25.25 0 01-.25-.25v-7.5zM9.018 12H6.982a5.72 5.72 0 01-.765 2.5h3.566a5.72 5.72 0 01-.765-2.5z"></path></svg>
                Open with GitHub Desktop
</a>            </li>
            <li class="Box-row Box-row--hover-gray p-0">
              <a class="d-flex flex-items-center text-gray-dark text-bold no-underline p-3" rel="nofollow" data-hydro-click="{&quot;event_type&quot;:&quot;clone_or_download.click&quot;,&quot;payload&quot;:{&quot;feature_clicked&quot;:&quot;DOWNLOAD_ZIP&quot;,&quot;git_repository_type&quot;:&quot;REPOSITORY&quot;,&quot;repository_id&quot;:255558345,&quot;originating_url&quot;:&quot;https://github.com/fuzhengwei/CodeGuide&quot;,&quot;user_id&quot;:67892538}}" data-hydro-click-hmac="348be0cb71ca1b01f808b071999b052ba5c54d977e7c6820872c26bcbc668ab9" data-ga-click="Repository, download zip, location:repo overview" data-open-app="link" href="/fuzhengwei/CodeGuide/archive/master.zip">
                <svg class="octicon octicon-file-zip mr-3" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M3.5 1.75a.25.25 0 01.25-.25h3a.75.75 0 000 1.5h.5a.75.75 0 000-1.5h2.086a.25.25 0 01.177.073l2.914 2.914a.25.25 0 01.073.177v8.586a.25.25 0 01-.25.25h-.5a.75.75 0 000 1.5h.5A1.75 1.75 0 0014 13.25V4.664c0-.464-.184-.909-.513-1.237L10.573.513A1.75 1.75 0 009.336 0H3.75A1.75 1.75 0 002 1.75v11.5c0 .649.353 1.214.874 1.515a.75.75 0 10.752-1.298.25.25 0 01-.126-.217V1.75zM8.75 3a.75.75 0 000 1.5h.5a.75.75 0 000-1.5h-.5zM6 5.25a.75.75 0 01.75-.75h.5a.75.75 0 010 1.5h-.5A.75.75 0 016 5.25zm2 1.5A.75.75 0 018.75 6h.5a.75.75 0 010 1.5h-.5A.75.75 0 018 6.75zm-1.25.75a.75.75 0 000 1.5h.5a.75.75 0 000-1.5h-.5zM8 9.75A.75.75 0 018.75 9h.5a.75.75 0 010 1.5h-.5A.75.75 0 018 9.75zm-.75.75a1.75 1.75 0 00-1.75 1.75v3c0 .414.336.75.75.75h2.5a.75.75 0 00.75-.75v-3a1.75 1.75 0 00-1.75-1.75h-.5zM7 12.25a.25.25 0 01.25-.25h.5a.25.25 0 01.25.25v2.25H7v-2.25z"></path></svg>
                Download ZIP
</a>            </li>
          </ul>
        </div>

        <div class="p-3" data-targets="get-repo.platforms" data-platform="mac" hidden="">
          <h4 class="lh-condensed mb-3">Launching GitHub Desktop<span class="AnimatedEllipsis"></span></h4>
          <p class="text-gray">If nothing happens, <a href="https://desktop.github.com/">download GitHub Desktop</a> and try again.</p>
          <button type="button" class="btn-link" data-action="click:get-repo#onDetailsToggle">Go back</button>
        </div>

        <div class="p-3" data-targets="get-repo.platforms" data-platform="windows" hidden="">
          <h4 class="lh-condensed mb-3">Launching GitHub Desktop<span class="AnimatedEllipsis"></span></h4>
          <p class="text-gray">If nothing happens, <a href="https://desktop.github.com/">download GitHub Desktop</a> and try again.</p>
          <button type="button" class="btn-link" data-action="click:get-repo#onDetailsToggle">Go back</button>
        </div>

        <div class="p-3" data-targets="get-repo.platforms" data-platform="xcode" hidden="">
          <h4 class="lh-condensed mb-3">Launching Xcode<span class="AnimatedEllipsis"></span></h4>
          <p class="text-gray">If nothing happens, <a href="https://developer.apple.com/xcode/">download Xcode</a> and try again.</p>
          <button type="button" class="btn-link" data-action="click:get-repo#onDetailsToggle">Go back</button>
        </div>

        <div class="p-3" data-targets="get-repo.platforms" data-platform="visual-studio" hidden="">
          <h4 class="lh-condensed mb-3">Launching Visual Studio<span class="AnimatedEllipsis"></span></h4>
          <p class="text-gray">If nothing happens, <a href="https://visualstudio.github.com/">download the GitHub extension for Visual Studio</a> and try again.</p>
          <button type="button" class="btn-link" data-action="click:get-repo#onDetailsToggle">Go back</button>
        </div>

      </div>
    </div>
  </details>
</get-repo>


      
    </span>
</div>


      

<div class="Box mb-3">
  <div class="Box-header Box-header--blue position-relative">
    <h2 class="sr-only">Latest commit</h2>
    <div class="js-details-container Details d-flex rounded-top-1 flex-items-center flex-wrap" data-issue-and-pr-hovercards-enabled="">
      
  <div class="flex-shrink-0 ml-n1 mr-n1 mt-n1 mb-n1 hx_avatar_stack_commit">
    
<div class="AvatarStack flex-self-start ">
  <div class="AvatarStack-body" aria-label="fuzhengwei">
        <a class="avatar avatar-user" data-skip-pjax="true" data-hovercard-type="user" data-hovercard-url="/users/fuzhengwei/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" style="width:24px;height:24px;" href="/fuzhengwei">
          <img height="24" width="24" alt="@fuzhengwei" src="https://avatars3.githubusercontent.com/u/3761578?s=60&amp;u=6bb0e6d0a4877100a6e6e1f327f2ac176100be51&amp;v=4" class=" avatar-user">
</a>  </div>
</div>

  </div>
  <div class="flex-1 d-flex flex-items-center ml-3 min-width-0">
    <div class="css-truncate css-truncate-overflow text-gray">
      
      <a href="/fuzhengwei/CodeGuide/commits?author=fuzhengwei" class="commit-author user-mention" title="View all commits by fuzhengwei">fuzhengwei</a>


  committed
  <a href="/fuzhengwei/CodeGuide/commit/3f76f87c98a1eca69dfef5f72418ab28b885687c" class="link-gray text-mono d-none d-md-inline text-small">3f76f87</a>
  <relative-time datetime="2020-07-07T14:25:05Z" class="no-wrap" title="2020年7月7日 GMT+8 下午10:25">2 days ago</relative-time>

    </div>
        <span class="ml-2">
          
  <details class="commit-build-statuses details-overlay details-reset js-dropdown-details" data-deferred-details-content-url="/_render_node/MDE3OlN0YXR1c0NoZWNrUm9sbHVwMjU1NTU4MzQ1OjNmNzZmODdjOThhMWVjYTY5ZGZlZjVmNzI0MThhYjI4Yjg4NTY4N2M=/statuses/combined_branch_status">
    <summary class="text-green">
      <svg aria-label="2 / 2 checks OK" class="octicon octicon-check" viewBox="0 0 16 16" version="1.1" width="16" height="16" role="img"><path fill-rule="evenodd" d="M13.78 4.22a.75.75 0 010 1.06l-7.25 7.25a.75.75 0 01-1.06 0L2.22 9.28a.75.75 0 011.06-1.06L6 10.94l6.72-6.72a.75.75 0 011.06 0z"></path></svg>
    </summary>
    <div class="dropdown-menu dropdown-menu-e overflow-hidden">
      <include-fragment class="m-4 d-flex flex-column flex-items-center">
        <div class="anim-pulse"><svg height="32" class="octicon octicon-octoface" viewBox="0 0 16 16" version="1.1" width="32" aria-hidden="true"><path fill-rule="evenodd" d="M14.7 5.34c.13-.32.55-1.59-.13-3.31 0 0-1.05-.33-3.44 1.3-1-.28-2.07-.32-3.13-.32s-2.13.04-3.13.32c-2.39-1.64-3.44-1.3-3.44-1.3-.68 1.72-.26 2.99-.13 3.31C.49 6.21 0 7.33 0 8.69 0 13.84 3.33 15 7.98 15S16 13.84 16 8.69c0-1.36-.49-2.48-1.3-3.35zM8 14.02c-3.3 0-5.98-.15-5.98-3.35 0-.76.38-1.48 1.02-2.07 1.07-.98 2.9-.46 4.96-.46 2.07 0 3.88-.52 4.96.46.65.59 1.02 1.3 1.02 2.07 0 3.19-2.68 3.35-5.98 3.35zM5.49 9.01c-.66 0-1.2.8-1.2 1.78s.54 1.79 1.2 1.79c.66 0 1.2-.8 1.2-1.79s-.54-1.78-1.2-1.78zm5.02 0c-.66 0-1.2.79-1.2 1.78s.54 1.79 1.2 1.79c.66 0 1.2-.8 1.2-1.79s-.53-1.78-1.2-1.78z"></path></svg></div>
        <div class="text-gray no-wrap">Loading status checks…</div>
      </include-fragment>
    </div>
  </details>


        </span>
  </div>
  <div class="pl-0 pl-md-5 flex-order-1 width-full Details-content--hidden">
      <div class="mt-2">
        <a data-pjax="true" class="link-gray-dark text-bold" href="/fuzhengwei/CodeGuide/commit/3f76f87c98a1eca69dfef5f72418ab28b885687c">小傅哥，文章更新 | 重学 Java 设计模式：实战模版模式「模拟爬虫各类电商商品，生成营销推广海报场景」</a>
      </div>

  </div>
      <div class="flex-shrink-0">
        <h2 class="sr-only">Git stats</h2>
        <ul class="list-style-none d-flex">
          <li class="ml-0 ml-md-3">
            <a data-pjax="" href="/fuzhengwei/CodeGuide/commits/master" class="pl-3 pr-3 py-3 p-md-0 mt-n3 mb-n3 mr-n3 m-md-0 link-gray-dark no-underline no-wrap">
              <svg height="16" class="octicon octicon-history text-gray" text="gray" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M1.643 3.143L.427 1.927A.25.25 0 000 2.104V5.75c0 .138.112.25.25.25h3.646a.25.25 0 00.177-.427L2.715 4.215a6.5 6.5 0 11-1.18 4.458.75.75 0 10-1.493.154 8.001 8.001 0 101.6-5.684zM7.75 4a.75.75 0 01.75.75v2.992l2.028.812a.75.75 0 01-.557 1.392l-2.5-1A.75.75 0 017 8.25v-3.5A.75.75 0 017.75 4z"></path></svg>

              <span class="d-none d-sm-inline">
                    <strong>175</strong>
                  <span aria-label="Commits on master" class="text-gray ">commits</span>
              </span>
            </a>
          </li>
            <li class="ml-3 d-none d-md-block">
              <a data-pjax="" href="/fuzhengwei/CodeGuide/branches" class="link-gray-dark no-underline d-inline-block">
                <svg height="16" class="octicon octicon-git-branch text-gray" text="gray" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M11.75 2.5a.75.75 0 100 1.5.75.75 0 000-1.5zm-2.25.75a2.25 2.25 0 113 2.122V6A2.5 2.5 0 0110 8.5H6a1 1 0 00-1 1v1.128a2.251 2.251 0 11-1.5 0V5.372a2.25 2.25 0 111.5 0v1.836A2.492 2.492 0 016 7h4a1 1 0 001-1v-.628A2.25 2.25 0 019.5 3.25zM4.25 12a.75.75 0 100 1.5.75.75 0 000-1.5zM3.5 3.25a.75.75 0 111.5 0 .75.75 0 01-1.5 0z"></path></svg>

                <strong>6</strong>
                branches
              </a>
            </li>
            <li class="ml-3 d-none d-md-block">
              <a data-pjax="" href="/fuzhengwei/CodeGuide/tags" class="link-gray-dark no-underline d-inline-block">
                <svg height="16" class="octicon octicon-tag text-gray" text="gray" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M2.5 7.775V2.75a.25.25 0 01.25-.25h5.025a.25.25 0 01.177.073l6.25 6.25a.25.25 0 010 .354l-5.025 5.025a.25.25 0 01-.354 0l-6.25-6.25a.25.25 0 01-.073-.177zm-1.5 0V2.75C1 1.784 1.784 1 2.75 1h5.025c.464 0 .91.184 1.238.513l6.25 6.25a1.75 1.75 0 010 2.474l-5.026 5.026a1.75 1.75 0 01-2.474 0l-6.25-6.25A1.75 1.75 0 011 7.775zM6 5a1 1 0 100 2 1 1 0 000-2z"></path></svg>

                <strong>0</strong>
                tags
              </a>
            </li>
        </ul>
      </div>
    </div>
  </div>
  <h2 id="files" class="sr-only">Files</h2>
  


    <a class="d-none js-permalink-shortcut" data-hotkey="y" href="/fuzhengwei/CodeGuide/tree/3f76f87c98a1eca69dfef5f72418ab28b885687c">Permalink</a>

  <div class="flash flash-full flash-error include-fragment-error py-2">
    <svg class="octicon octicon-alert mr-2" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.22 1.754a.25.25 0 00-.44 0L1.698 13.132a.25.25 0 00.22.368h12.164a.25.25 0 00.22-.368L8.22 1.754zm-1.763-.707c.659-1.234 2.427-1.234 3.086 0l6.082 11.378A1.75 1.75 0 0114.082 15H1.918a1.75 1.75 0 01-1.543-2.575L6.457 1.047zM9 11a1 1 0 11-2 0 1 1 0 012 0zm-.25-5.25a.75.75 0 00-1.5 0v2.5a.75.75 0 001.5 0v-2.5z"></path></svg> Failed to load latest commit information.
  </div>
  <div class="js-details-container Details">
    <div role="grid" aria-labelledby="files" class="Details-content--hidden-not-important js-navigation-container js-active-navigation-container d-md-block" data-pjax="">
      <div class="sr-only" role="row">
        <div role="columnheader">Type</div>
        <div role="columnheader">Name</div>
        <div role="columnheader" class="d-none d-md-block">Latest commit message</div>
        <div role="columnheader">Commit time</div>
      </div>

        <div role="row" class="Box-row Box-row--focus-gray py-2 d-flex position-relative js-navigation-item ">
          <div role="gridcell" class="mr-3 flex-shrink-0" style="width: 16px;">
            <svg height="16" class="octicon octicon-file-directory color-blue-3" color="blue-3" aria-label="Directory" viewBox="0 0 16 16" version="1.1" width="16" role="img"><path fill-rule="evenodd" d="M1.75 1A1.75 1.75 0 000 2.75v10.5C0 14.216.784 15 1.75 15h12.5A1.75 1.75 0 0016 13.25v-8.5A1.75 1.75 0 0014.25 3h-6.5a.25.25 0 01-.2-.1l-.9-1.2c-.33-.44-.85-.7-1.4-.7h-3.5z"></path></svg>


          </div>

          <div role="rowheader" class="flex-auto min-width-0 col-md-2 mr-3">
            <span class="css-truncate css-truncate-target d-block width-fit"><a class="js-navigation-open link-gray-dark" title="docs" id="e3e2a9bfd88566b05001b02a3f51d286-41bf33b8dc215152b3c831ec404a2a7adfda50a9" href="/fuzhengwei/CodeGuide/tree/master/docs">docs</a></span>
          </div>

          <div role="gridcell" class="flex-auto min-width-0 d-none d-md-block col-5 mr-3 commit-message">
              <span class="css-truncate css-truncate-target d-block width-fit">
                    <a data-pjax="true" title="Add files via upload" class="link-gray" href="/fuzhengwei/CodeGuide/commit/a8027e6c8e79388ed24a28fb5ca4e0abf0589390">Add files via upload</a>
              </span>
          </div>

          <div role="gridcell" class="text-gray-light text-right" style="width:100px;">
              <time-ago datetime="2020-06-23T02:15:52Z" class="no-wrap" title="2020年6月23日 GMT+8 上午10:15">16 days ago</time-ago>
          </div>

        </div>
        <div role="row" class="Box-row Box-row--focus-gray py-2 d-flex position-relative js-navigation-item ">
          <div role="gridcell" class="mr-3 flex-shrink-0" style="width: 16px;">
            <svg height="16" class="octicon octicon-file text-gray-light" color="gray-light" aria-label="File" viewBox="0 0 16 16" version="1.1" width="16" role="img"><path fill-rule="evenodd" d="M3.75 1.5a.25.25 0 00-.25.25v11.5c0 .138.112.25.25.25h8.5a.25.25 0 00.25-.25V6H9.75A1.75 1.75 0 018 4.25V1.5H3.75zm5.75.56v2.19c0 .138.112.25.25.25h2.19L9.5 2.06zM2 1.75C2 .784 2.784 0 3.75 0h5.086c.464 0 .909.184 1.237.513l3.414 3.414c.329.328.513.773.513 1.237v8.086A1.75 1.75 0 0112.25 15h-8.5A1.75 1.75 0 012 13.25V1.75z"></path></svg>


          </div>

          <div role="rowheader" class="flex-auto min-width-0 col-md-2 mr-3">
            <span class="css-truncate css-truncate-target d-block width-fit"><a class="js-navigation-open link-gray-dark" title="README.md" id="04c6e90faac2675aa89e2176d2eec7d8-c68a4746ad7eebc048182c641e441524285ffcbd" href="/fuzhengwei/CodeGuide/blob/master/README.md">README.md</a></span>
          </div>

          <div role="gridcell" class="flex-auto min-width-0 d-none d-md-block col-5 mr-3 commit-message">
              <span class="css-truncate css-truncate-target d-block width-fit">
                    <a data-pjax="true" title="小傅哥，文章更新 | 重学 Java 设计模式：实战模版模式「模拟爬虫各类电商商品，生成营销推广海报场景」" class="link-gray" href="/fuzhengwei/CodeGuide/commit/3f76f87c98a1eca69dfef5f72418ab28b885687c">小傅哥，文章更新 | 重学 Java 设计模式：实战模版模式「模拟爬虫各类电商商品，生成营销推广海报场景」</a>
              </span>
          </div>

          <div role="gridcell" class="text-gray-light text-right" style="width:100px;">
              <time-ago datetime="2020-07-07T14:25:05Z" class="no-wrap" title="2020年7月7日 GMT+8 下午10:25">2 days ago</time-ago>
          </div>

        </div>
        <div role="row" class="Box-row Box-row--focus-gray py-2 d-flex position-relative js-navigation-item ">
          <div role="gridcell" class="mr-3 flex-shrink-0" style="width: 16px;">
            <svg height="16" class="octicon octicon-file text-gray-light" color="gray-light" aria-label="File" viewBox="0 0 16 16" version="1.1" width="16" role="img"><path fill-rule="evenodd" d="M3.75 1.5a.25.25 0 00-.25.25v11.5c0 .138.112.25.25.25h8.5a.25.25 0 00.25-.25V6H9.75A1.75 1.75 0 018 4.25V1.5H3.75zm5.75.56v2.19c0 .138.112.25.25.25h2.19L9.5 2.06zM2 1.75C2 .784 2.784 0 3.75 0h5.086c.464 0 .909.184 1.237.513l3.414 3.414c.329.328.513.773.513 1.237v8.086A1.75 1.75 0 0112.25 15h-8.5A1.75 1.75 0 012 13.25V1.75z"></path></svg>


          </div>

          <div role="rowheader" class="flex-auto min-width-0 col-md-2 mr-3">
            <span class="css-truncate css-truncate-target d-block width-fit"><a class="js-navigation-open link-gray-dark" title="pom.xml" id="600376dffeb79835ede4a0b285078036-2407ded17903333f9ab135375f4d8156892ef256" href="/fuzhengwei/CodeGuide/blob/master/pom.xml">pom.xml</a></span>
          </div>

          <div role="gridcell" class="flex-auto min-width-0 d-none d-md-block col-5 mr-3 commit-message">
              <span class="css-truncate css-truncate-target d-block width-fit">
                    <a data-pjax="true" title="小傅哥 | 《汉字不能编程？别闹了，只是看着有点豪横！容易被开除！》" class="link-gray" href="/fuzhengwei/CodeGuide/commit/30b1a488b4e1c67b90d4f06aedf36240c5552466">小傅哥 | 《汉字不能编程？别闹了，只是看着有点豪横！容易被开除！》</a>
              </span>
          </div>

          <div role="gridcell" class="text-gray-light text-right" style="width:100px;">
              <time-ago datetime="2020-05-05T05:12:10Z" class="no-wrap" title="2020年5月5日 GMT+8 下午1:12">2 months ago</time-ago>
          </div>

        </div>
    </div>
    <div class="Details-content--shown Box-footer d-md-none p-0">
      <button type="button" class="d-block btn-link js-details-target width-full px-3 py-2" aria-expanded="false">
        View code
      </button>
    </div>
  </div>




</div>

  <div id="readme" class="Box md js-code-block-container Box--responsive">
    <div class="Box-header d-flex flex-items-center flex-justify-between bg-white border-bottom-0">
      <h2 class="Box-title pr-3">
        README.md
      </h2>
    </div>
      <div class="Box-body px-5 pb-5">
        <article class="markdown-body entry-content container-lg" itemprop="text"><h1><a id="user-content-codeguide--程序员编码指南" class="anchor" aria-hidden="true" href="#codeguide--程序员编码指南"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>CodeGuide | 程序员编码指南</h1>
<blockquote>
<p><strong>作者：</strong> 小傅哥，Java Developer，<a href="https://bugstack.cn" rel="nofollow"><g-emoji class="g-emoji" alias="pencil2" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/270f.png">✏️</g-emoji> 虫洞 · 科技栈，作者</a>，<a href="https://bugstack.blog.csdn.net" rel="nofollow"><g-emoji class="g-emoji" alias="trophy" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f3c6.png">🏆</g-emoji> CSDN 博客专家</a></p>
</blockquote>
<blockquote>
<p>本代码库是作者小傅哥多年从事一线互联网<code>Java</code>开发的学习历程技术汇总，旨在为大家提供一个清晰详细的学习教程，侧重点更倾向编写Java核心内容。如果本仓库能为您提供帮助，请给予支持(关注、点赞、分享)！</p>
</blockquote>
<br>
<div align="center">
    <a href="https://bugstack.cn" rel="nofollow"><img src="https://camo.githubusercontent.com/4c16d08d1a90d726e1b657f228dd2eef890bf7d5/68747470733a2f2f627567737461636b2e636e2f6173736574732f696d616765732f69636f6e2e737667" width="128px" data-canonical-src="https://bugstack.cn/assets/images/icon.svg" style="max-width:100%;"></a>
</div>
<br>  
<div align="center">
<a href="https://github.com/fuzhengwei/CodeGuide"><img src="https://camo.githubusercontent.com/53b841885acedef5398d276db5a3f596a60dd54b/68747470733a2f2f62616467656e2e6e65742f6769746875622f73746172732f66757a68656e677765692f436f646547756964653f69636f6e3d67697468756226636f6c6f723d346162386131" data-canonical-src="https://badgen.net/github/stars/fuzhengwei/CodeGuide?icon=github&amp;color=4ab8a1" style="max-width:100%;"></a>
<a href="https://github.com/fuzhengwei/CodeGuide"><img src="https://camo.githubusercontent.com/54038374ab453650eb9db157471c4a0fdff44dcc/68747470733a2f2f62616467656e2e6e65742f6769746875622f666f726b732f66757a68656e677765692f436f646547756964653f69636f6e3d67697468756226636f6c6f723d346162386131" data-canonical-src="https://badgen.net/github/forks/fuzhengwei/CodeGuide?icon=github&amp;color=4ab8a1" style="max-width:100%;"></a>
<a href="https://bugstack.cn" rel="nofollow"><img src="https://camo.githubusercontent.com/f30a026832ee32458c5ba7d065d53b0245c2fdcb/68747470733a2f2f627567737461636b2e636e2f6173736574732f696d616765732f6f6e6c696e65626f6f6b2e737667" data-canonical-src="https://bugstack.cn/assets/images/onlinebook.svg" style="max-width:100%;"></a>
<a href="https://bugstack.cn/assets/images/qrcode.png?x-oss-process=style/may" rel="nofollow"><img src="https://camo.githubusercontent.com/e2ce00728112a2973dea30a6ce6a51464b2c1a5c/68747470733a2f2f6974737461636b2e6f72672f5f6d656469612f7778627567737461636b2e737667" data-canonical-src="https://itstack.org/_media/wxbugstack.svg" style="max-width:100%;"></a>
</div>
<br>
<table>
<thead>
<tr>
<th align="center">ID</th>
<th align="center">Logo</th>
<th align="left">专栏文章</th>
<th align="left">源码下载</th>
</tr>
</thead>
<tbody>
<tr>
<td align="center">0</td>
<td align="center"><g-emoji class="g-emoji" alias="volcano" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f30b.png">🌋</g-emoji></td>
<td align="left"><code>网络调试助手</code></td>
<td align="left"><a href="https://download.csdn.net/download/yao__shun__yu/11835105" rel="nofollow">NetAssist下载</a></td>
</tr>
<tr>
<td align="center">1</td>
<td align="center"><g-emoji class="g-emoji" alias="sound" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f509.png">🔉</g-emoji></td>
<td align="left"><a href="#sound-Netty4%E4%B8%93%E9%A2%98"><code>Netty4.x专题</code></a></td>
<td align="left"><a href="https://github.com/fuzhengwei/itstack-demo-netty">itstack-demo-netty</a></td>
</tr>
<tr>
<td align="center">2</td>
<td align="center"><g-emoji class="g-emoji" alias="electric_plug" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f50c.png">🔌</g-emoji></td>
<td align="left"><a href="#electric_plug-%E6%89%8B%E5%86%99RPC%E6%A1%86%E6%9E%B6"><code>手写RPC框架</code></a></td>
<td align="left"><a href="https://github.com/fuzhengwei/itstack-demo-rpc">itstack-demo-rpc</a></td>
</tr>
<tr>
<td align="center">3</td>
<td align="center"><g-emoji class="g-emoji" alias="computer" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f4bb.png">💻</g-emoji></td>
<td align="left"><a href="#computer-%E7%94%A8Java%E5%AE%9E%E7%8E%B0JVM"><code>用Java实现JVM</code></a></td>
<td align="left"><a href="https://github.com/fuzhengwei/itstack-demo-jvm">itstack-demo-jvm</a></td>
</tr>
<tr>
<td align="center">4</td>
<td align="center"><g-emoji class="g-emoji" alias="ghost" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f47b.png">👻</g-emoji></td>
<td align="left"><a href="#ghost-%E5%9F%BA%E4%BA%8EJavaAgent%E7%9A%84%E5%85%A8%E9%93%BE%E8%B7%AF%E7%9B%91%E6%8E%A7"><code>基于JavaAgent的全链路监控</code></a></td>
<td align="left"><a href="https://github.com/fuzhengwei/itstack-demo-agent">itstack-demo-agent</a></td>
</tr>
<tr>
<td align="center">5</td>
<td align="center"><g-emoji class="g-emoji" alias="shower" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f6bf.png">🚿</g-emoji></td>
<td align="left"><a href="#shower-iot-gateway%E7%BD%91%E5%85%B3%E6%A1%88%E4%BE%8B"><code>iot-gateway网关案例</code></a></td>
<td align="left"><a href="https://github.com/fuzhengwei/itstack-demo-iot-gatewary">itstack-demo-iot-gatewary</a></td>
</tr>
<tr>
<td align="center">6</td>
<td align="center"><g-emoji class="g-emoji" alias="triangular_ruler" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f4d0.png">📐</g-emoji></td>
<td align="left"><a href="#triangular_ruler-DDD%E9%A2%86%E5%9F%9F%E9%A9%B1%E5%8A%A8%E8%AE%BE%E8%AE%A1%E8%90%BD%E5%9C%B0"><code>DDD领域驱动设计落地</code></a></td>
<td align="left"><a href="https://github.com/fuzhengwei/itstack-demo-ddd">itstack-demo-ddd</a></td>
</tr>
<tr>
<td align="center">7</td>
<td align="center"><g-emoji class="g-emoji" alias="outbox_tray" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f4e4.png">📤</g-emoji></td>
<td align="left"><a href="#outbox_tray-SpringCloud%E5%85%A5%E9%97%A8%E6%A1%88%E4%BE%8B"><code>SpringCloud入门案例</code></a></td>
<td align="left"><a href="https://github.com/fuzhengwei/itstack-demo-springcloud">itstack-demo-springcloud</a></td>
</tr>
<tr>
<td align="center">8</td>
<td align="center"><g-emoji class="g-emoji" alias="performing_arts" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f3ad.png">🎭</g-emoji></td>
<td align="left"><a href="#performing_arts-%E5%BE%AE%E4%BF%A1%E5%85%AC%E4%BC%97%E5%8F%B7%E5%BC%80%E5%8F%91"><code>微信公众号开发</code></a></td>
<td align="left"><a href="https://github.com/fuzhengwei/itstack-ark-wx-test">itstack-ark-wx</a></td>
</tr>
<tr>
<td align="center">9</td>
<td align="center"><g-emoji class="g-emoji" alias="nut_and_bolt" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f529.png">🔩</g-emoji></td>
<td align="left"><a href="#nut_and_bolt-SpringBoot%E4%B8%AD%E9%97%B4%E4%BB%B6%E5%BC%80%E5%8F%91"><code>SpringBoot中间件开发</code></a></td>
<td align="left"><a href="https://github.com/fuzhengwei/door-spring-boot-starter">door-spring-boot-starter</a></td>
</tr>
<tr>
<td align="center">10</td>
<td align="center"><g-emoji class="g-emoji" alias="art" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f3a8.png">🎨</g-emoji></td>
<td align="left"><a href="#art-%E6%9C%8D%E5%8A%A1%E6%A1%86%E6%9E%B6%E6%90%AD%E5%BB%BA"><code>服务框架搭建</code></a></td>
<td align="left"><a href="https://github.com/fuzhengwei/itstack-demo-frame">itstack-demo-frame</a></td>
</tr>
<tr>
<td align="center">11</td>
<td align="center"><g-emoji class="g-emoji" alias="flashlight" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f526.png">🔦</g-emoji></td>
<td align="left"><a href="#flashlight-%E6%BA%90%E7%A0%81%E5%88%86%E6%9E%90"><code>源码分析(Spring、Mybatis、Schedule)</code></a></td>
<td align="left"><a href="https://github.com/fuzhengwei/itstack-demo-code">itstack-demo-code</a></td>
</tr>
<tr>
<td align="center">12</td>
<td align="center"><g-emoji class="g-emoji" alias="airplane" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2708.png">✈️</g-emoji></td>
<td align="left"><a href="#airplane-Drools%E8%A7%84%E5%88%99%E5%BC%95%E6%93%8E"><code>Drools规则引擎</code></a></td>
<td align="left"><a href="https://github.com/fuzhengwei/itstack-demo-drools">itstack-demo-drools</a></td>
</tr>
<tr>
<td align="center">13</td>
<td align="center"><g-emoji class="g-emoji" alias="tractor" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f69c.png">🚜</g-emoji></td>
<td align="left"><a href="#tractor-ASM%E5%AD%97%E8%8A%82%E7%A0%81%E7%BC%96%E7%A8%8B"><code>ASM字节码编程</code></a></td>
<td align="left"><a href="https://github.com/fuzhengwei/itstack-demo-asm">itstack-demo-asm</a></td>
</tr>
<tr>
<td align="center">14</td>
<td align="center"><g-emoji class="g-emoji" alias="feet" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f43e.png">🐾</g-emoji></td>
<td align="left"><a href="#paw_prints-%E6%88%91%E7%9A%84%E5%A4%A7%E5%AD%A6%E5%9B%9B%E5%B9%B4%E5%88%B0%E6%AF%95%E4%B8%9A%E5%B7%A5%E4%BD%9C5%E5%B9%B4%E7%9A%84%E5%AD%A6%E4%B9%A0%E8%B7%AF%E7%BA%BF%E8%B5%84%E6%BA%90%E5%92%8C%E9%9D%A2%E8%AF%95%E6%B1%87%E6%80%BB"><code>我的大学四年到毕业工作5年的学习资源和面试汇总</code></a></td>
<td align="left"><a href="https://pan.baidu.com/s/4mmX7sDy" rel="nofollow">https://pan.baidu.com/s/4mmX7sDy - （if链接失效，加我微信：fustack）</a></td>
</tr>
<tr>
<td align="center">15</td>
<td align="center"><g-emoji class="g-emoji" alias="walking" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f6b6.png">🚶</g-emoji></td>
<td align="left"><a href="#walking-Netty%E4%BB%BF%E6%A1%8C%E9%9D%A2%E7%89%88%E5%BE%AE%E4%BF%A1%E8%81%8A%E5%A4%A9"><code>Netty+JavaFx实战：仿桌面版微信聊天</code></a></td>
<td align="left"><a href="https://github.com/fuzhengwei/NaiveChat">NaiveChat</a></td>
</tr>
<tr>
<td align="center">16</td>
<td align="center"><g-emoji class="g-emoji" alias="bookmark_tabs" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f4d1.png">📑</g-emoji></td>
<td align="left"><a href="https://bugstack.cn/itstack-demo-any/2019/12/10/%E6%9C%89%E7%82%B9%E5%B9%B2%E8%B4%A7-Jdk1.8%E6%96%B0%E7%89%B9%E6%80%A7%E5%AE%9E%E6%88%98%E7%AF%87(41%E4%B8%AA%E6%A1%88%E4%BE%8B).html" rel="nofollow"><code>JDK1.8新特性41个案例讲解</code></a></td>
<td align="left"><a href="https://github.com/fuzhengwei/itstack-demo-jdk8">itstack-demo-jdk8</a></td>
</tr>
<tr>
<td align="center">17</td>
<td align="center"><g-emoji class="g-emoji" alias="bike" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f6b2.png">🚲</g-emoji></td>
<td align="left"><a href="#bike-%E5%AD%97%E8%8A%82%E7%A0%81%E7%BC%96%E7%A8%8B%E4%B8%93%E6%A0%8F"><code>小傅哥的《字节码编程》专栏</code></a></td>
<td align="left"><a href="https://github.com/fuzhengwei/itstack-demo-bytecode">itstack-demo-bytecode</a></td>
</tr>
<tr>
<td align="center">18</td>
<td align="center"><g-emoji class="g-emoji" alias="school_satchel" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f392.png">🎒</g-emoji></td>
<td align="left"><a href="#school_satchel-%E5%AE%9E%E6%88%98%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F"><code>实战设计模式</code></a></td>
<td align="left"><a href="https://github.com/fuzhengwei/itstack-demo-design">itstack-demo-design</a></td>
</tr>
<tr>
<td align="center">-1</td>
<td align="center"><g-emoji class="g-emoji" alias="ferris_wheel" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f3a1.png">🎡</g-emoji></td>
<td align="left"><a href="#ferris_wheel-%E5%85%B6%E4%BB%96%E6%96%87%E7%AB%A0"><code>其他文章</code></a></td>
<td align="left"><a href="https://github.com/fuzhengwei/CodeGuide/tree/master/src">CodeGuide</a></td>
</tr>
</tbody>
</table>
<p><strong>如果</strong>，以上某些资源不能下载获取，可以添加作者：小傅哥，微信(fustack)</p>
<h2><a id="user-content-sound-netty4专题" class="anchor" aria-hidden="true" href="#sound-netty4专题"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><g-emoji class="g-emoji" alias="sound" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f509.png">🔉</g-emoji> Netty4专题</h2>
<p><em>Netty4.x案例从简单入门到应用实战，全篇37节优秀案例+实战源码[基础篇(12)、拓展篇(13)、应用篇(3章+)、源码篇(6)]，以上章节全部完成并不断持续更新中。</em></p>
<h3><a id="user-content-基础入门篇" class="anchor" aria-hidden="true" href="#基础入门篇"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>基础入门篇</h3>
<ul>
<li><a href="https://bugstack.cn/itstack-demo-netty-1/2019/07/30/netty%E6%A1%88%E4%BE%8B-netty4.1%E5%9F%BA%E7%A1%80%E5%85%A5%E9%97%A8%E7%AF%87%E9%9B%B6-%E5%88%9D%E5%85%A5JavaIO%E4%B9%8B%E9%97%A8BIO-NIO-AIO%E5%AE%9E%E6%88%98%E7%BB%83%E4%B9%A0.html" rel="nofollow"><code>netty4.1基础入门篇零《初入JavaIO之门BIO、NIO、AIO实战练习》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-1/2019/08/01/netty%E6%A1%88%E4%BE%8B-netty4.1%E5%9F%BA%E7%A1%80%E5%85%A5%E9%97%A8%E7%AF%87%E4%B8%80-%E5%97%A8-NettyServer.html" rel="nofollow"><code>netty4.1基础入门篇一《嗨！NettyServer》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-1/2019/08/05/netty%E6%A1%88%E4%BE%8B-netty4.1%E5%9F%BA%E7%A1%80%E5%85%A5%E9%97%A8%E7%AF%87%E4%BA%8C-NettyServer%E6%8E%A5%E6%94%B6%E6%95%B0%E6%8D%AE.html" rel="nofollow"><code>netty4.1基础入门篇二《NettyServer接收数据》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-1/2019/08/06/netty%E6%A1%88%E4%BE%8B-netty4.1%E5%9F%BA%E7%A1%80%E5%85%A5%E9%97%A8%E7%AF%87%E4%B8%89-NettyServer%E5%AD%97%E7%AC%A6%E4%B8%B2%E8%A7%A3%E7%A0%81%E5%99%A8.html" rel="nofollow"><code>netty4.1基础入门篇三《NettyServer字符串解码器》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-1/2019/08/07/netty%E6%A1%88%E4%BE%8B-netty4.1%E5%9F%BA%E7%A1%80%E5%85%A5%E9%97%A8%E7%AF%87%E5%9B%9B-NettyServer%E6%94%B6%E5%8F%91%E6%95%B0%E6%8D%AE.html" rel="nofollow"><code>netty4.1基础入门篇四《NettyServer收发数据》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-1/2019/08/08/netty%E6%A1%88%E4%BE%8B-netty4.1%E5%9F%BA%E7%A1%80%E5%85%A5%E9%97%A8%E7%AF%87%E4%BA%94-NettyServer%E5%AD%97%E7%AC%A6%E4%B8%B2%E7%BC%96%E7%A0%81%E5%99%A8.html" rel="nofollow"><code>netty4.1基础入门篇五《NettyServer字符串编码器》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-1/2019/08/09/netty%E6%A1%88%E4%BE%8B-netty4.1%E5%9F%BA%E7%A1%80%E5%85%A5%E9%97%A8%E7%AF%87%E5%85%AD-NettyServer%E7%BE%A4%E5%8F%91%E6%B6%88%E6%81%AF.html" rel="nofollow"><code>netty4.1基础入门篇六《NettyServer群发消息》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-1/2019/08/10/netty%E6%A1%88%E4%BE%8B-netty4.1%E5%9F%BA%E7%A1%80%E5%85%A5%E9%97%A8%E7%AF%87%E4%B8%83-%E5%97%A8-NettyClient.html" rel="nofollow"><code>netty4.1基础入门篇七《嗨！NettyClient》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-1/2019/08/11/netty%E6%A1%88%E4%BE%8B-netty4.1%E5%9F%BA%E7%A1%80%E5%85%A5%E9%97%A8%E7%AF%87%E5%85%AB-NettyClient%E5%8D%8A%E5%8C%85%E7%B2%98%E5%8C%85%E5%A4%84%E7%90%86-%E7%BC%96%E7%A0%81%E8%A7%A3%E7%A0%81%E5%A4%84%E7%90%86-%E6%94%B6%E5%8F%91%E6%95%B0%E6%8D%AE%E6%96%B9%E5%BC%8F.html" rel="nofollow"><code>netty4.1基础入门篇八《NettyClient半包粘包处理、编码解码处理、收发数据方式》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-1/2019/08/12/netty%E6%A1%88%E4%BE%8B-netty4.1%E5%9F%BA%E7%A1%80%E5%85%A5%E9%97%A8%E7%AF%87%E4%B9%9D-%E8%87%AA%E5%AE%9A%E4%B9%89%E7%BC%96%E7%A0%81%E8%A7%A3%E7%A0%81%E5%99%A8-%E5%A4%84%E7%90%86%E5%8D%8A%E5%8C%85-%E7%B2%98%E5%8C%85%E6%95%B0%E6%8D%AE.html" rel="nofollow"><code>netty4.1基础入门篇九《自定义编码解码器，处理半包、粘包数据》</code></a></li>
<li><a href="/fuzhengwei/CodeGuide/blob/master/netty%E6%A1%88%E4%BE%8B%EF%BC%8Cnetty4.1%E5%9F%BA%E7%A1%80%E5%85%A5%E9%97%A8%E7%AF%87%E5%8D%81%E3%80%8A%E5%85%B3%E4%BA%8EChannelOutboundHandlerAdapter%E7%AE%80%E5%8D%95%E4%BD%BF%E7%94%A8%E3%80%8B"><code>netty4.1基础入门篇十《关于ChannelOutboundHandlerAdapter简单使用》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-1/2019/08/14/netty%E6%A1%88%E4%BE%8B-netty4.1%E5%9F%BA%E7%A1%80%E5%85%A5%E9%97%A8%E7%AF%87%E5%8D%81%E4%B8%80-netty-udp%E9%80%9A%E4%BF%A1%E6%96%B9%E5%BC%8F%E6%A1%88%E4%BE%8BDemo.html" rel="nofollow"><code>netty4.1基础入门篇十一《netty udp通信方式案例Demo》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-1/2019/08/15/netty%E6%A1%88%E4%BE%8B-netty4.1%E5%9F%BA%E7%A1%80%E5%85%A5%E9%97%A8%E7%AF%87%E5%8D%81%E4%BA%8C-%E7%AE%80%E5%8D%95%E5%AE%9E%E7%8E%B0%E4%B8%80%E4%B8%AA%E5%9F%BA%E4%BA%8ENetty%E6%90%AD%E5%BB%BA%E7%9A%84Http%E6%9C%8D%E5%8A%A1.html" rel="nofollow"><code>netty4.1基础入门篇十二《简单实现一个基于Netty搭建的Http服务》</code></a></li>
</ul>
<h3><a id="user-content-中级拓展篇" class="anchor" aria-hidden="true" href="#中级拓展篇"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>中级拓展篇</h3>
<ul>
<li><a href="https://bugstack.cn/itstack-demo-netty-2/2019/08/16/netty%E6%A1%88%E4%BE%8B-netty4.1%E4%B8%AD%E7%BA%A7%E6%8B%93%E5%B1%95%E7%AF%87%E4%B8%80-Netty%E4%B8%8ESpringBoot%E6%95%B4%E5%90%88.html" rel="nofollow"><code>netty4.1中级拓展篇一《Netty与SpringBoot整合》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-2/2019/08/17/netty%E6%A1%88%E4%BE%8B-netty4.1%E4%B8%AD%E7%BA%A7%E6%8B%93%E5%B1%95%E7%AF%87%E4%BA%8C-Netty%E4%BD%BF%E7%94%A8Protobuf%E4%BC%A0%E8%BE%93%E6%95%B0%E6%8D%AE.html" rel="nofollow"><code>netty4.1中级拓展篇二《Netty使用Protobuf传输数据》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-2/2019/08/18/netty%E6%A1%88%E4%BE%8B-netty4.1%E4%B8%AD%E7%BA%A7%E6%8B%93%E5%B1%95%E7%AF%87%E4%B8%89-Netty%E4%BC%A0%E8%BE%93Java%E5%AF%B9%E8%B1%A1.html" rel="nofollow"><code>netty4.1中级拓展篇三《Netty传输Java对象》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-2/2019/08/19/netty%E6%A1%88%E4%BE%8B-netty4.1%E4%B8%AD%E7%BA%A7%E6%8B%93%E5%B1%95%E7%AF%87%E5%9B%9B-Netty%E4%BC%A0%E8%BE%93%E6%96%87%E4%BB%B6-%E5%88%86%E7%89%87%E5%8F%91%E9%80%81-%E6%96%AD%E7%82%B9%E7%BB%AD%E4%BC%A0.html" rel="nofollow"><code>netty4.1中级拓展篇四《Netty传输文件、分片发送、断点续传》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-2/2019/08/20/netty%E6%A1%88%E4%BE%8B-netty4.1%E4%B8%AD%E7%BA%A7%E6%8B%93%E5%B1%95%E7%AF%87%E4%BA%94-%E5%9F%BA%E4%BA%8ENetty%E6%90%AD%E5%BB%BAWebSocket-%E6%A8%A1%E4%BB%BF%E5%BE%AE%E4%BF%A1%E8%81%8A%E5%A4%A9%E9%A1%B5%E9%9D%A2.html" rel="nofollow"><code>netty4.1中级拓展篇五《基于Netty搭建WebSocket，模仿微信聊天页面》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-2/2019/08/21/netty%E6%A1%88%E4%BE%8B-netty4.1%E4%B8%AD%E7%BA%A7%E6%8B%93%E5%B1%95%E7%AF%87%E5%85%AD-SpringBoot+Netty+Elasticsearch%E6%94%B6%E9%9B%86%E6%97%A5%E5%BF%97%E4%BF%A1%E6%81%AF%E6%95%B0%E6%8D%AE%E5%AD%98%E5%82%A8.html" rel="nofollow"><code>netty4.1中级拓展篇六《SpringBoot+Netty+Elasticsearch收集日志信息数据存储》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-2/2019/08/22/netty%E6%A1%88%E4%BE%8B-netty4.1%E4%B8%AD%E7%BA%A7%E6%8B%93%E5%B1%95%E7%AF%87%E4%B8%83-Netty%E8%AF%B7%E6%B1%82%E5%93%8D%E5%BA%94%E5%90%8C%E6%AD%A5%E9%80%9A%E4%BF%A1.html" rel="nofollow"><code>netty4.1中级拓展篇七《Netty请求响应同步通信》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-2/2019/08/23/netty%E6%A1%88%E4%BE%8B-netty4.1%E4%B8%AD%E7%BA%A7%E6%8B%93%E5%B1%95%E7%AF%87%E5%85%AB-Netty%E5%BF%83%E8%B7%B3%E6%9C%8D%E5%8A%A1%E4%B8%8E%E6%96%AD%E7%BA%BF%E9%87%8D%E8%BF%9E.html" rel="nofollow"><code>netty4.1中级拓展篇八《Netty心跳服务与断线重连》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-2/2019/08/24/netty%E6%A1%88%E4%BE%8B-netty4.1%E4%B8%AD%E7%BA%A7%E6%8B%93%E5%B1%95%E7%AF%87%E4%B9%9D-Netty%E9%9B%86%E7%BE%A4%E9%83%A8%E7%BD%B2%E5%AE%9E%E7%8E%B0%E8%B7%A8%E6%9C%8D%E5%8A%A1%E7%AB%AF%E9%80%9A%E4%BF%A1%E7%9A%84%E8%90%BD%E5%9C%B0%E6%96%B9%E6%A1%88.html" rel="nofollow"><code>netty4.1中级拓展篇九《Netty集群部署实现跨服务端通信的落地方案》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-2/2019/08/25/netty%E6%A1%88%E4%BE%8B-netty4.1%E4%B8%AD%E7%BA%A7%E6%8B%93%E5%B1%95%E7%AF%87%E5%8D%81-Netty%E6%8E%A5%E6%94%B6%E5%8F%91%E9%80%81%E5%A4%9A%E7%A7%8D%E5%8D%8F%E8%AE%AE%E6%B6%88%E6%81%AF%E7%B1%BB%E5%9E%8B%E7%9A%84%E9%80%9A%E4%BF%A1%E5%A4%84%E7%90%86%E6%96%B9%E6%A1%88.html" rel="nofollow"><code>netty4.1中级拓展篇十《Netty接收发送多种协议消息类型的通信处理方案》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-2/2019/08/26/netty%E6%A1%88%E4%BE%8B-netty4.1%E4%B8%AD%E7%BA%A7%E6%8B%93%E5%B1%95%E7%AF%87%E5%8D%81%E4%B8%80-Netty%E5%9F%BA%E4%BA%8EChunkedStream%E6%95%B0%E6%8D%AE%E6%B5%81%E5%88%87%E5%9D%97%E4%BC%A0%E8%BE%93.html" rel="nofollow"><code>netty4.1中级拓展篇十一《Netty基于ChunkedStream数据流切块传输》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-2/2019/08/27/netty%E6%A1%88%E4%BE%8B-netty4.1%E4%B8%AD%E7%BA%A7%E6%8B%93%E5%B1%95%E7%AF%87%E5%8D%81%E4%BA%8C-Netty%E6%B5%81%E9%87%8F%E6%95%B4%E5%BD%A2%E6%95%B0%E6%8D%AE%E6%B5%81%E9%80%9F%E7%8E%87%E6%8E%A7%E5%88%B6%E5%88%86%E6%9E%90%E4%B8%8E%E5%AE%9E%E6%88%98.html" rel="nofollow"><code>netty4.1中级拓展篇十二《Netty流量整形数据流速率控制分析与实战》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-2/2019/08/28/netty%E6%A1%88%E4%BE%8B-netty4.1%E4%B8%AD%E7%BA%A7%E6%8B%93%E5%B1%95%E7%AF%87%E5%8D%81%E4%B8%89-Netty%E5%9F%BA%E4%BA%8ESSL%E5%AE%9E%E7%8E%B0%E4%BF%A1%E6%81%AF%E4%BC%A0%E8%BE%93%E8%BF%87%E7%A8%8B%E4%B8%AD%E5%8F%8C%E5%90%91%E5%8A%A0%E5%AF%86%E9%AA%8C%E8%AF%81.html" rel="nofollow"><code>netty4.1中级拓展篇十三《Netty基于SSL实现信息传输过程中双向加密验证》</code></a></li>
</ul>
<h3><a id="user-content-高级应用篇" class="anchor" aria-hidden="true" href="#高级应用篇"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>高级应用篇</h3>
<ul>
<li><a href="https://bugstack.cn/itstack-demo-netty-3/2019/09/01/%E6%89%8B%E5%86%99RPC%E6%A1%86%E6%9E%B6%E7%AC%AC%E4%B8%80%E7%AB%A0-%E8%87%AA%E5%AE%9A%E4%B9%89%E9%85%8D%E7%BD%AExml.html" rel="nofollow"><code>手写RPC框架第一章《自定义配置xml》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-3/2019/09/02/%E6%89%8B%E5%86%99RPC%E6%A1%86%E6%9E%B6%E7%AC%AC%E4%BA%8C%E7%AB%A0-netty%E9%80%9A%E4%BF%A1.html" rel="nofollow"><code>手写RPC框架第二章《netty通信》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-3/2019/09/03/%E6%89%8B%E5%86%99RPC%E6%A1%86%E6%9E%B6%E7%AC%AC%E4%B8%89%E7%AB%A0-RPC%E4%B8%AD%E9%97%B4%E4%BB%B6.html" rel="nofollow"><code>手写RPC框架第三章《RPC中间件》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-3/2019/12/01/websocket%E4%B8%8E%E4%B8%8B%E4%BD%8D%E6%9C%BA%E9%80%9A%E8%BF%87netty%E6%96%B9%E5%BC%8F%E9%80%9A%E4%BF%A1%E4%BC%A0%E8%BE%93%E8%A1%8C%E4%B8%BA%E4%BF%A1%E6%81%AF.html" rel="nofollow"><code>websocket与下位机通过netty方式通信传输行为信息</code></a></li>
</ul>
<h3><a id="user-content-源码分析篇" class="anchor" aria-hidden="true" href="#源码分析篇"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>源码分析篇</h3>
<ul>
<li><a href="https://bugstack.cn/itstack-demo-netty-4/2019/09/10/netty%E6%A1%88%E4%BE%8B-netty4.1%E6%BA%90%E7%A0%81%E5%88%86%E6%9E%90%E7%AF%87%E4%B8%80-NioEventLoopGroup%E6%BA%90%E7%A0%81%E5%88%86%E6%9E%90.html" rel="nofollow"><code>netty4.1源码分析篇一《NioEventLoopGroup源码分析》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-4/2019/09/11/netty%E6%A1%88%E4%BE%8B-netty4.1%E6%BA%90%E7%A0%81%E5%88%86%E6%9E%90%E7%AF%87%E4%BA%8C-ServerBootstrap%E9%85%8D%E7%BD%AE%E4%B8%8E%E7%BB%91%E5%AE%9A%E5%90%AF%E5%8A%A8.html" rel="nofollow"><code>netty4.1源码分析篇二《ServerBootstrap配置与绑定启动》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-4/2019/09/12/netty%E6%A1%88%E4%BE%8B-netty4.1%E6%BA%90%E7%A0%81%E5%88%86%E6%9E%90%E7%AF%87%E4%B8%89-Netty%E6%9C%8D%E5%8A%A1%E7%AB%AF%E5%88%9D%E5%A7%8B%E5%8C%96%E8%BF%87%E7%A8%8B%E4%BB%A5%E5%8F%8A%E5%8F%8D%E5%B0%84%E5%B7%A5%E5%8E%82%E7%9A%84%E4%BD%9C%E7%94%A8.html" rel="nofollow"><code>netty4.1源码分析篇三《Netty服务端初始化过程以及反射工厂的作用》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-4/2019/09/13/netty%E6%A1%88%E4%BE%8B-netty4.1%E6%BA%90%E7%A0%81%E5%88%86%E6%9E%90%E7%AF%87%E5%9B%9B-ByteBuf%E7%9A%84%E6%95%B0%E6%8D%AE%E7%BB%93%E6%9E%84%E5%9C%A8%E4%BD%BF%E7%94%A8%E6%96%B9%E5%BC%8F%E4%B8%AD%E7%9A%84%E5%89%96%E6%9E%90.html" rel="nofollow"><code>netty4.1源码分析篇四《ByteBuf的数据结构在使用方式中的剖析》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-4/2019/09/14/netty%E6%A1%88%E4%BE%8B-netty4.1%E6%BA%90%E7%A0%81%E5%88%86%E6%9E%90%E7%AF%87%E4%BA%94-%E4%B8%80%E8%A1%8C%E7%AE%80%E5%8D%95%E7%9A%84writeAndFlush%E9%83%BD%E5%81%9A%E4%BA%86%E5%93%AA%E4%BA%9B%E4%BA%8B.html" rel="nofollow"><code>netty4.1源码分析篇五《一行简单的writeAndFlush都做了哪些事》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-4/2019/09/15/netty%E6%A1%88%E4%BE%8B-netty4.1%E6%BA%90%E7%A0%81%E5%88%86%E6%9E%90%E7%AF%87%E5%85%AD-Netty%E5%BC%82%E6%AD%A5%E6%9E%B6%E6%9E%84%E7%9B%91%E5%90%AC%E7%B1%BBPromise%E6%BA%90%E7%A0%81%E5%88%86%E6%9E%90.html" rel="nofollow"><code>netty4.1源码分析篇六《Netty异步架构监听类Promise源码分析》</code></a></li>
</ul>
<h2><a id="user-content-electric_plug-手写rpc框架" class="anchor" aria-hidden="true" href="#electric_plug-手写rpc框架"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><g-emoji class="g-emoji" alias="electric_plug" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f50c.png">🔌</g-emoji> 手写RPC框架</h2>
<p><em>RPC是一种远程调用的通信协议，例如dubbo、thrift等，我们在互联网高并发应用开发时候都会使用到类似的服务。本专题主要通过三个章节简单的实现rpc基础功能，来深入学习rpc是如何交互通信的。</em></p>
<ul>
<li><a href="https://bugstack.cn/itstack-demo-netty-3/2019/09/01/%E6%89%8B%E5%86%99RPC%E6%A1%86%E6%9E%B6%E7%AC%AC%E4%B8%80%E7%AB%A0-%E8%87%AA%E5%AE%9A%E4%B9%89%E9%85%8D%E7%BD%AExml.html" rel="nofollow"><code>手写RPC框架第一章《自定义配置xml》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-3/2019/09/02/%E6%89%8B%E5%86%99RPC%E6%A1%86%E6%9E%B6%E7%AC%AC%E4%BA%8C%E7%AB%A0-netty%E9%80%9A%E4%BF%A1.html" rel="nofollow"><code>手写RPC框架第二章《netty通信》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-netty-3/2019/09/03/%E6%89%8B%E5%86%99RPC%E6%A1%86%E6%9E%B6%E7%AC%AC%E4%B8%89%E7%AB%A0-RPC%E4%B8%AD%E9%97%B4%E4%BB%B6.html" rel="nofollow"><code>手写RPC框架第三章《RPC中间件》</code></a></li>
</ul>
<h2><a id="user-content-computer-用java实现jvm" class="anchor" aria-hidden="true" href="#computer-用java实现jvm"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><g-emoji class="g-emoji" alias="computer" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f4bb.png">💻</g-emoji> 用Java实现JVM</h2>
<p><em>本专题主要介绍如何通过java代码来实现JVM的基础功能（搜索解析class文件、字节码命令、运行时数据区等），从而让java程序员通过最熟知的java程序，学习JVM是如何将java程序一步步跑起来的。</em></p>
<ul>
<li><a href="https://bugstack.cn/itstack-demo-jvm/2019/05/01/%E7%94%A8Java%E5%AE%9E%E7%8E%B0JVM%E7%AC%AC%E4%B8%80%E7%AB%A0-%E5%91%BD%E4%BB%A4%E8%A1%8C%E5%B7%A5%E5%85%B7.html" rel="nofollow"><code>用Java实现JVM第一章《命令行工具》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-jvm/2019/05/02/%E7%94%A8Java%E5%AE%9E%E7%8E%B0JVM%E7%AC%AC%E4%BA%8C%E7%AB%A0-%E6%90%9C%E7%B4%A2class%E6%96%87%E4%BB%B6.html" rel="nofollow"><code>用Java实现JVM第二章《搜索class文件》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-jvm/2019/05/03/%E7%94%A8Java%E5%AE%9E%E7%8E%B0JVM%E7%AC%AC%E4%B8%89%E7%AB%A0-%E8%A7%A3%E6%9E%90class%E6%96%87%E4%BB%B6.html" rel="nofollow"><code>用Java实现JVM第三章《解析class文件》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-jvm/2019/05/04/%E7%94%A8Java%E5%AE%9E%E7%8E%B0JVM%E7%AC%AC%E4%B8%89%E7%AB%A0-%E8%A7%A3%E6%9E%90class%E6%96%87%E4%BB%B6-%E9%99%84-classReader%E6%8B%86%E8%A7%A3.html" rel="nofollow"><code>用Java实现JVM第三章《解析class文件》附[classReader拆解]</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-jvm/2019/05/05/%E7%94%A8Java%E5%AE%9E%E7%8E%B0JVM%E7%AC%AC%E5%9B%9B%E7%AB%A0-%E8%BF%90%E8%A1%8C%E6%97%B6%E6%95%B0%E6%8D%AE%E5%8C%BA.html" rel="nofollow"><code>用Java实现JVM第四章《运行时数据区》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-jvm/2019/05/06/%E7%94%A8Java%E5%AE%9E%E7%8E%B0JVM%E7%AC%AC%E4%BA%94%E7%AB%A0-%E6%8C%87%E4%BB%A4%E9%9B%86%E5%92%8C%E8%A7%A3%E9%87%8A%E5%99%A8.html" rel="nofollow"><code>用Java实现JVM第五章《指令集和解释器》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-jvm/2019/05/07/%E7%94%A8Java%E5%AE%9E%E7%8E%B0JVM%E7%AC%AC%E5%85%AD%E7%AB%A0-%E7%B1%BB%E5%92%8C%E5%AF%B9%E8%B1%A1.html" rel="nofollow"><code>用Java实现JVM第六章《类和对象》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-jvm/2019/05/08/%E7%94%A8Java%E5%AE%9E%E7%8E%B0JVM%E7%AC%AC%E4%B8%83%E7%AB%A0-%E6%96%B9%E6%B3%95%E8%B0%83%E7%94%A8%E5%92%8C%E8%BF%94%E5%9B%9E.html" rel="nofollow"><code>用Java实现JVM第七章《方法调用和返回》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-jvm/2019/05/09/%E7%94%A8Java%E5%AE%9E%E7%8E%B0JVM%E7%AC%AC%E5%85%AB%E7%AB%A0-%E6%95%B0%E7%BB%84%E5%92%8C%E5%AD%97%E7%AC%A6%E4%B8%B2.html" rel="nofollow"><code>用Java实现JVM第八章《数组和字符串》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-jvm/2019/05/10/%E7%94%A8Java%E5%AE%9E%E7%8E%B0JVM%E7%AC%AC%E4%B9%9D%E7%AB%A0-%E6%9C%AC%E5%9C%B0%E6%96%B9%E6%B3%95%E8%B0%83%E7%94%A8.html" rel="nofollow"><code>用Java实现JVM第九章《本地方法调用》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-jvm/2019/05/11/%E7%94%A8Java%E5%AE%9E%E7%8E%B0JVM%E7%AC%AC%E5%8D%81%E7%AB%A0-%E5%BC%82%E5%B8%B8%E5%A4%84%E7%90%86.html" rel="nofollow"><code>用Java实现JVM第十章《异常处理》</code></a></li>
</ul>
<h2><a id="user-content-ghost-基于javaagent的全链路监控" class="anchor" aria-hidden="true" href="#ghost-基于javaagent的全链路监控"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><g-emoji class="g-emoji" alias="ghost" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f47b.png">👻</g-emoji> 基于JavaAgent的全链路监控</h2>
<p><em>目前市面的全链路监控系统基本都是参考Google的Dapper来做的，本专题主要通过六个章节的代码实战，来介绍如何使用javaagent以及字节码应用，来实现一个简单的java代码链路流程监控。</em></p>
<ul>
<li><a href="https://bugstack.cn/itstack-demo-agent/2019/07/10/%E5%9F%BA%E4%BA%8EJavaAgent%E7%9A%84%E5%85%A8%E9%93%BE%E8%B7%AF%E7%9B%91%E6%8E%A7%E4%B8%80-%E5%97%A8-JavaAgent.html" rel="nofollow"><code>基于JavaAgent的全链路监控一《嗨！JavaAgent》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-agent/2019/07/11/%E5%9F%BA%E4%BA%8EJavaAgent%E7%9A%84%E5%85%A8%E9%93%BE%E8%B7%AF%E7%9B%91%E6%8E%A7%E4%BA%8C-%E9%80%9A%E8%BF%87%E5%AD%97%E8%8A%82%E7%A0%81%E5%A2%9E%E5%8A%A0%E7%9B%91%E6%8E%A7%E6%89%A7%E8%A1%8C%E8%80%97%E6%97%B6.html" rel="nofollow"><code>基于JavaAgent的全链路监控二《通过字节码增加监控执行耗时》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-agent/2019/07/12/%E5%9F%BA%E4%BA%8EJavaAgent%E7%9A%84%E5%85%A8%E9%93%BE%E8%B7%AF%E7%9B%91%E6%8E%A7%E4%B8%89-ByteBuddy%E6%93%8D%E4%BD%9C%E7%9B%91%E6%8E%A7%E6%96%B9%E6%B3%95%E5%AD%97%E8%8A%82%E7%A0%81.html" rel="nofollow"><code>基于JavaAgent的全链路监控三《ByteBuddy操作监控方法字节码》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-agent/2019/07/13/%E5%9F%BA%E4%BA%8EJavaAgent%E7%9A%84%E5%85%A8%E9%93%BE%E8%B7%AF%E7%9B%91%E6%8E%A7%E5%9B%9B-JVM%E5%86%85%E5%AD%98%E4%B8%8EGC%E4%BF%A1%E6%81%AF.html" rel="nofollow"><code>基于JavaAgent的全链路监控四《JVM内存与GC信息》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-agent/2019/07/14/%E5%9F%BA%E4%BA%8EJavaAgent%E7%9A%84%E5%85%A8%E9%93%BE%E8%B7%AF%E7%9B%91%E6%8E%A7%E4%BA%94-ThreadLocal%E9%93%BE%E8%B7%AF%E8%BF%BD%E8%B8%AA.html" rel="nofollow"><code>基于JavaAgent的全链路监控五《ThreadLocal链路追踪》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-agent/2019/07/15/%E5%9F%BA%E4%BA%8EJavaAgent%E7%9A%84%E5%85%A8%E9%93%BE%E8%B7%AF%E7%9B%91%E6%8E%A7%E5%85%AD-%E5%BC%80%E5%8F%91%E5%BA%94%E7%94%A8%E7%BA%A7%E7%9B%91%E6%8E%A7.html" rel="nofollow"><code>基于JavaAgent的全链路监控六《开发应用级监控》</code></a></li>
</ul>
<h2><a id="user-content-shower-iot-gateway网关案例" class="anchor" aria-hidden="true" href="#shower-iot-gateway网关案例"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><g-emoji class="g-emoji" alias="shower" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f6bf.png">🚿</g-emoji> iot-gateway网关案例</h2>
<p><em>基于Netty实现的物联网网关服务，支持百万客户端连接，压力测试ing...，并优化了与服务端集群通信对平均算法做了优化,本次上传代码添加了很多功能，摒弃了以往只做心跳维护、数据转发的功能。</em></p>
<ul>
<li><a href="https://mp.weixin.qq.com/s/LLyG2ji2gDR2Fz8uDmfJ7A" rel="nofollow"><code>基于Netty实践搭建的物联网网关iot-gatway</code></a></li>
</ul>
<h2><a id="user-content-triangular_ruler-ddd领域驱动设计落地" class="anchor" aria-hidden="true" href="#triangular_ruler-ddd领域驱动设计落地"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><g-emoji class="g-emoji" alias="triangular_ruler" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f4d0.png">📐</g-emoji> DDD领域驱动设计落地</h2>
<p><em>本专题以DDD实战落地为根本，分章节设计不同的架构模型，学习并实战是奔入应用级开发最快的方法，Hi HelloWorld！我来了。</em></p>
<ul>
<li><a href="https://bugstack.cn/itstack-demo-ddd/2019/10/15/DDD%E4%B8%93%E9%A2%98%E6%A1%88%E4%BE%8B%E4%B8%80-%E5%88%9D%E8%AF%86%E9%A2%86%E5%9F%9F%E9%A9%B1%E5%8A%A8%E8%AE%BE%E8%AE%A1DDD%E8%90%BD%E5%9C%B0.html" rel="nofollow"><code>DDD专题案例一《初识领域驱动设计DDD落地》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-ddd/2019/10/16/DDD%E4%B8%93%E9%A2%98%E6%A1%88%E4%BE%8B%E4%BA%8C-%E9%A2%86%E5%9F%9F%E5%B1%82%E5%86%B3%E7%AD%96%E8%A7%84%E5%88%99%E6%A0%91%E6%9C%8D%E5%8A%A1%E8%AE%BE%E8%AE%A1.html" rel="nofollow"><code>DDD专题案例二《领域层决策规则树服务设计》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-ddd/2019/10/17/DDD%E4%B8%93%E9%A2%98%E6%A1%88%E4%BE%8B%E4%B8%89-%E9%A2%86%E5%9F%9F%E9%A9%B1%E5%8A%A8%E8%AE%BE%E8%AE%A1%E6%9E%B6%E6%9E%84%E5%9F%BA%E4%BA%8ESpringCloud%E6%90%AD%E5%BB%BA%E5%BE%AE%E6%9C%8D%E5%8A%A1.html" rel="nofollow"><code>DDD专题案例三《领域驱动设计架构基于SpringCloud搭建微服务》</code></a></li>
</ul>
<h2><a id="user-content-outbox_tray-springcloud入门案例" class="anchor" aria-hidden="true" href="#outbox_tray-springcloud入门案例"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><g-emoji class="g-emoji" alias="outbox_tray" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f4e4.png">📤</g-emoji> SpringCloud入门案例</h2>
<ul>
<li><a href="https://bugstack.cn/itstack-demo-springcloud/2019/10/31/Spring-Cloud(%E9%9B%B6)-%E6%80%BB%E6%9C%89%E4%B8%80%E5%81%8F%E6%A6%82%E8%BF%B0%E5%91%8A%E8%AF%89%E4%BD%A0SpringCloud%E6%98%AF%E4%BB%80%E4%B9%88.html" rel="nofollow"><code>Spring Cloud(零)《总有一偏概述告诉你SpringCloud是什么》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-springcloud/2019/11/01/Spring-Cloud(%E4%B8%80)-%E6%9C%8D%E5%8A%A1%E9%9B%86%E7%BE%A4%E6%B3%A8%E5%86%8C%E4%B8%8E%E5%8F%91%E7%8E%B0-Eureka.html" rel="nofollow"><code>Spring Cloud(一)《服务集群注册与发现 Eureka》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-springcloud/2019/11/02/Spring-Cloud(%E4%BA%8C)-%E6%9C%8D%E5%8A%A1%E6%8F%90%E4%BE%9B%E4%B8%8E%E8%B4%9F%E8%BD%BD%E5%9D%87%E8%A1%A1%E8%B0%83%E7%94%A8-Eureka.html" rel="nofollow"><code>Spring Cloud(二)《服务提供与负载均衡调用 Eureka》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-springcloud/2019/11/03/Spring-Cloud(%E4%B8%89)-%E5%BA%94%E7%94%A8%E6%9C%8D%E5%8A%A1%E5%BF%AB%E9%80%9F%E5%A4%B1%E8%B4%A5%E7%86%94%E6%96%AD%E9%99%8D%E7%BA%A7%E4%BF%9D%E6%8A%A4-Hystrix.html" rel="nofollow"><code>Spring Cloud(三)《应用服务快速失败熔断降级保护 Hystrix》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-springcloud/2019/11/04/Spring-Cloud(%E5%9B%9B)-%E6%9C%8D%E5%8A%A1%E5%93%8D%E5%BA%94%E6%80%A7%E8%83%BD%E6%88%90%E5%8A%9F%E7%8E%87%E7%9B%91%E6%8E%A7-Hystrix.html" rel="nofollow"><code>Spring Cloud(四)《服务响应性能成功率监控 Hystrix》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-springcloud/2019/11/05/Spring-Cloud(%E4%BA%94)-Turbine-%E7%9B%91%E6%8E%A7%E4%BF%A1%E6%81%AF%E8%81%9A%E5%90%88%E5%B1%95%E7%A4%BA-Hystrix.html" rel="nofollow"><code>Spring Cloud(五)《Turbine 监控信息聚合展示 Hystrix》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-springcloud/2019/11/06/Spring-Cloud(%E5%85%AD)-%E5%9F%BA%E4%BA%8EGithub-Webhook%E5%8A%A8%E6%80%81%E5%88%B7%E6%96%B0%E6%9C%8D%E5%8A%A1%E9%85%8D%E7%BD%AE.html" rel="nofollow"><code>Spring Cloud(六)《基于github webhook动态刷新服务配置》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-springcloud/2019/11/07/Spring-Cloud(%E4%B8%83)-%E5%9F%BA%E4%BA%8ERabbitMQ%E6%B6%88%E6%81%AF%E6%80%BB%E7%BA%BF%E6%96%B9%E5%BC%8F%E5%88%B7%E6%96%B0%E9%85%8D%E7%BD%AE%E6%9C%8D%E5%8A%A1.html" rel="nofollow"><code>Spring Cloud(七)《基于RabbitMQ消息总线方式刷新配置服务》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-springcloud/2019/11/08/Spring-Cloud(%E5%85%AB)-%E6%9C%8D%E5%8A%A1%E7%BD%91%E5%85%B3%E8%B7%AF%E7%94%B1-Zuul1.html" rel="nofollow"><code>Spring Cloud(八)《服务网关路由 Zuul1》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-springcloud/2019/11/24/Spring-Cloud(%E4%B9%9D)-%E6%9C%8D%E5%8A%A1%E7%BD%91%E5%85%B3Zuul-%E5%8A%A8%E6%80%81%E8%B7%AF%E7%94%B1%E4%B8%8E%E6%9D%83%E9%99%90%E8%BF%87%E6%BB%A4%E5%99%A8.html" rel="nofollow"><code>Spring Cloud(九)《服务网关Zuul 动态路由与权限过滤器》</code></a></li>
</ul>
<h2><a id="user-content-performing_arts-微信公众号开发" class="anchor" aria-hidden="true" href="#performing_arts-微信公众号开发"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><g-emoji class="g-emoji" alias="performing_arts" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f3ad.png">🎭</g-emoji> 微信公众号开发</h2>
<p><em>这是一套基于领域驱动设计方式搭建的Java公众号开发工程，主要服务于博客与公众号之间打通，引导用户关注公众号，做粉丝回流。</em></p>
<ul>
<li><a href="https://bugstack.cn/itstack-demo-any/2019/11/23/%E5%B9%B6%E4%B8%8D%E6%83%B3%E5%90%B9%E7%89%9B%E7%9A%AE-%E4%BD%86-%E4%B8%BA%E4%BA%86%E6%8A%8AGithub%E5%8D%9A%E5%AE%A2%E7%B2%89%E4%B8%9D%E8%BD%AC%E7%A7%BB%E5%88%B0%E5%85%AC%E4%BC%97%E5%8F%B7-%E6%88%91%E5%B9%B2%E4%BA%86.html" rel="nofollow"><code>并不想吹牛皮，但！为了把Github博客粉丝转移到公众号，我干了！</code></a></li>
</ul>
<h2><a id="user-content-nut_and_bolt-springboot中间件开发" class="anchor" aria-hidden="true" href="#nut_and_bolt-springboot中间件开发"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><g-emoji class="g-emoji" alias="nut_and_bolt" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f529.png">🔩</g-emoji> SpringBoot中间件开发</h2>
<p><em>Spring Boot 中间件开发，基于服务治理为目的将非业务行为的核心逻辑剥离出来开发为独立的中间件，赋能于业务系统快速开发。</em></p>
<ul>
<li><a href="https://bugstack.cn/itstack-demo-any/2019/12/07/%E5%8F%91%E5%B8%83Jar%E5%8C%85%E5%88%B0Maven%E4%B8%AD%E5%A4%AE%E4%BB%93%E5%BA%93(%E4%B8%BA%E5%BC%80%E5%8F%91%E5%BC%80%E6%BA%90%E4%B8%AD%E9%97%B4%E4%BB%B6%E5%81%9A%E5%87%86%E5%A4%87).html" rel="nofollow"><code>发布Jar包到Maven中央仓库(为开发开源中间件做准备)</code></a></li>
<li><a href="https://bugstack.cn/itstack-ark-middleware/2019/12/02/Spring-Boot-%E4%B8%AD%E9%97%B4%E4%BB%B6%E5%BC%80%E5%8F%91(%E4%B8%80)-%E6%9C%8D%E5%8A%A1%E6%B2%BB%E7%90%86%E4%B8%AD%E9%97%B4%E4%BB%B6%E4%B9%8B%E7%BB%9F%E4%B8%80%E7%99%BD%E5%90%8D%E5%8D%95%E9%AA%8C%E8%AF%81.html" rel="nofollow"><code>Spring Boot 中间件开发(一)《服务治理中间件之统一白名单验证》</code></a></li>
<li><a href="https://bugstack.cn/itstack-ark-middleware/2019/12/08/%E5%BC%80%E5%8F%91%E5%9F%BA%E4%BA%8ESpringBoot%E7%9A%84%E5%88%86%E5%B8%83%E5%BC%8F%E4%BB%BB%E5%8A%A1%E4%B8%AD%E9%97%B4%E4%BB%B6DcsSchedule(%E4%B8%BA%E5%BC%80%E6%BA%90%E8%B4%A1%E7%8C%AE%E5%8A%9B%E9%87%8F).html" rel="nofollow"><code>开发基于SpringBoot的分布式任务中间件DcsSchedule(为开源贡献力量)</code></a></li>
</ul>
<h2><a id="user-content-art-服务框架搭建" class="anchor" aria-hidden="true" href="#art-服务框架搭建"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><g-emoji class="g-emoji" alias="art" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f3a8.png">🎨</g-emoji> 服务框架搭建</h2>
<p><em>服务框架搭建，依赖于不同的业务诉求搭建出各种服务功能的框架结构。将逐步完成；单体服务应用(适合于ERP和个人)、分库分表应用、Mq服务、任务服务、分布式服务、RPC服务等。</em></p>
<ul>
<li><a href="https://bugstack.cn/itstack-demo-frame/2019/12/22/%E6%9E%B6%E6%9E%84%E6%A1%86%E6%9E%B6%E6%90%AD%E5%BB%BA(%E4%B8%80)-%E5%8D%95%E4%BD%93%E5%BA%94%E7%94%A8%E6%9C%8D%E5%8A%A1%E4%B9%8BSSM%E6%95%B4%E5%90%88-Spring4-+-SpringMvc-+-Mybatis.html" rel="nofollow"><code>架构框架搭建(一)《单体应用服务之SSM整合：Spring4 + SpringMvc + Mybatis》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-frame/2019/12/31/%E6%9E%B6%E6%9E%84%E6%A1%86%E6%9E%B6%E6%90%AD%E5%BB%BA(%E4%BA%8C)-Dubbo%E5%88%86%E5%B8%83%E5%BC%8F%E9%A2%86%E5%9F%9F%E9%A9%B1%E5%8A%A8%E8%AE%BE%E8%AE%A1%E6%9E%B6%E6%9E%84%E6%A1%86%E4%BD%93.html" rel="nofollow"><code>架构框架搭建(二)《Dubbo分布式领域驱动设计架构框体》</code></a></li>
</ul>
<h2><a id="user-content-flashlight-源码分析" class="anchor" aria-hidden="true" href="#flashlight-源码分析"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><g-emoji class="g-emoji" alias="flashlight" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f526.png">🔦</g-emoji> 源码分析</h2>
<p><em>源码分析以最核心干货内容为入手，将平时开发使用到的Spring、Mybatis、多线程等逐个渗透分析研究。不在只是单纯使用，而是要从原理分析获取更多的技术成长。</em></p>
<ul>
<li><a href="https://bugstack.cn/itstack-demo-any/2019/12/25/%E6%BA%90%E7%A0%81%E5%88%86%E6%9E%90-Mybatis%E6%8E%A5%E5%8F%A3%E6%B2%A1%E6%9C%89%E5%AE%9E%E7%8E%B0%E7%B1%BB%E4%B8%BA%E4%BB%80%E4%B9%88%E5%8F%AF%E4%BB%A5%E6%89%A7%E8%A1%8C%E5%A2%9E%E5%88%A0%E6%94%B9%E6%9F%A5.html" rel="nofollow"><code>源码分析 | Mybatis接口没有实现类为什么可以执行增删改查</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-any/2020/01/01/%E6%BA%90%E7%A0%81%E8%A7%A3%E6%9E%90-Spring%E5%AE%9A%E6%97%B6%E4%BB%BB%E5%8A%A1Quartz%E6%89%A7%E8%A1%8C%E5%85%A8%E8%BF%87%E7%A8%8B%E6%BA%90%E7%A0%81%E8%A7%A3%E8%AF%BB.html" rel="nofollow"><code>源码分析 | Spring定时任务Quartz执行全过程源码解读</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-any/2020/01/06/%E6%BA%90%E7%A0%81%E5%88%86%E6%9E%90-%E5%92%8B%E5%98%9E-%E4%BD%A0%E7%9A%84IDEA%E8%BF%87%E6%9C%9F%E4%BA%86%E5%90%A7-%E5%8A%A0%E4%B8%AAJar%E5%8C%85%E5%B0%B1%E7%A0%B4%E8%A7%A3%E4%BA%86-%E4%B8%BA%E4%BB%80%E4%B9%88.html" rel="nofollow"><code>源码分析 | 咋嘞？你的IDEA过期了吧！加个Jar包就破解了，为什么？</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-any/2020/01/08/%E6%BA%90%E7%A0%81%E5%88%86%E6%9E%90-%E5%83%8F%E7%9B%97%E5%A2%93%E4%B8%80%E6%A0%B7%E5%88%86%E6%9E%90Spring%E6%98%AF%E6%80%8E%E4%B9%88%E5%88%9D%E5%A7%8B%E5%8C%96xml%E5%B9%B6%E6%B3%A8%E5%86%8Cbean%E7%9A%84.html" rel="nofollow"><code>源码分析 | 像盗墓一样分析Spring是怎么初始化xml并注册bean的</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-any/2020/01/13/%E6%BA%90%E7%A0%81%E5%88%86%E6%9E%90-%E5%9F%BA%E4%BA%8Ejdbc%E5%AE%9E%E7%8E%B0%E4%B8%80%E4%B8%AADemo%E7%89%88%E7%9A%84Mybatis.html" rel="nofollow"><code>源码分析 | 基于jdbc实现一个Demo版的Mybatis</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-any/2020/01/20/%E6%BA%90%E7%A0%81%E5%88%86%E6%9E%90-%E6%89%8B%E5%86%99mybait-spring%E6%A0%B8%E5%BF%83%E5%8A%9F%E8%83%BD(%E5%B9%B2%E8%B4%A7%E5%A5%BD%E6%96%87%E4%B8%80%E6%AC%A1%E5%AD%A6%E4%BC%9A%E5%B7%A5%E5%8E%82bean-%E7%B1%BB%E4%BB%A3%E7%90%86-bean%E6%B3%A8%E5%86%8C%E7%9A%84%E4%BD%BF%E7%94%A8).html" rel="nofollow"><code>源码分析 | 手写mybait-spring核心功能(干货好文一次学会工厂bean、类代理、bean注册的使用)</code></a></li>
</ul>
<h2><a id="user-content-airplane-drools规则引擎" class="anchor" aria-hidden="true" href="#airplane-drools规则引擎"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><g-emoji class="g-emoji" alias="airplane" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2708.png">✈️</g-emoji> Drools规则引擎</h2>
<p><em>Drools 是 Java 语言基于Rete算法编写的规则引擎，可以方便的使用声明表达业务逻辑，非常简单易用。本专题会从入门开始逐步完成对Drools的讲解。</em></p>
<ul>
<li><a href="https://bugstack.cn/itstack-demo-drools/2020/03/07/%E8%BF%99%E7%A7%8D%E5%9C%BA%E6%99%AF%E4%BD%A0%E8%BF%98%E5%86%99ifelse%E4%BD%A0%E8%B7%9F%E5%AD%A9%E5%AD%90%E5%9D%90%E4%B8%80%E6%A1%8C%E5%8E%BB%E5%90%A7.html" rel="nofollow"><code>这种场景你还写ifelse你跟孩子坐一桌去吧</code></a></li>
</ul>
<h2><a id="user-content-tractor-asm字节码编程" class="anchor" aria-hidden="true" href="#tractor-asm字节码编程"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><g-emoji class="g-emoji" alias="tractor" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f69c.png">🚜</g-emoji> ASM字节码编程</h2>
<p><em>ASM是一个java字节码操纵框架，它能被用来动态生成类或者增强既有类的功能。ASM 可以直接产生二进制 class 文件，也可以在类被加载入 Java 虚拟机之前动态改变类行为。</em></p>
<ul>
<li><a href="https://bugstack.cn/itstack-demo-agent/2020/03/25/ASM%E5%AD%97%E8%8A%82%E7%A0%81%E7%BC%96%E7%A8%8B-%E5%A6%82%E6%9E%9C%E4%BD%A0%E5%8F%AA%E5%86%99CRUD-%E9%82%A3%E8%BF%99%E7%A7%8D%E6%8A%80%E6%9C%AF%E4%BD%A0%E6%B0%B8%E8%BF%9C%E7%A2%B0%E4%B8%8D%E5%88%B0.html" rel="nofollow"><code>ASM字节码编程 | 如果你只写CRUD，那这种技术你永远碰不到</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-agent/2020/04/05/ASM%E5%AD%97%E8%8A%82%E7%A0%81%E7%BC%96%E7%A8%8B-JavaAgent+ASM%E5%AD%97%E8%8A%82%E7%A0%81%E6%8F%92%E6%A1%A9%E9%87%87%E9%9B%86%E6%96%B9%E6%B3%95%E5%90%8D%E7%A7%B0%E4%BB%A5%E5%8F%8A%E5%85%A5%E5%8F%82%E5%92%8C%E5%87%BA%E5%8F%82%E7%BB%93%E6%9E%9C%E5%B9%B6%E8%AE%B0%E5%BD%95%E6%96%B9%E6%B3%95%E8%80%97%E6%97%B6.html" rel="nofollow"><code>ASM字节码编程 | JavaAgent+ASM字节码插桩采集方法名称以及入参和出参结果并记录方法耗时</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-any/2020/01/06/%E6%BA%90%E7%A0%81%E5%88%86%E6%9E%90-%E5%92%8B%E5%98%9E-%E4%BD%A0%E7%9A%84IDEA%E8%BF%87%E6%9C%9F%E4%BA%86%E5%90%A7-%E5%8A%A0%E4%B8%AAJar%E5%8C%85%E5%B0%B1%E7%A0%B4%E8%A7%A3%E4%BA%86-%E4%B8%BA%E4%BB%80%E4%B9%88.html" rel="nofollow"><code>源码分析 | 咋嘞？你的IDEA过期了吧！加个Jar包就破解了，为什么？</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-agent/2020/04/16/ASM%E5%AD%97%E8%8A%82%E7%A0%81%E7%BC%96%E7%A8%8B-%E7%94%A8%E5%AD%97%E8%8A%82%E7%A0%81%E5%A2%9E%E5%BC%BA%E6%8A%80%E6%9C%AF%E7%BB%99%E6%89%80%E6%9C%89%E6%96%B9%E6%B3%95%E5%8A%A0%E4%B8%8ATryCatch%E6%8D%95%E8%8E%B7%E5%BC%82%E5%B8%B8%E5%B9%B6%E8%BE%93%E5%87%BA.html" rel="nofollow"><code>ASM字节码编程 | 用字节码增强技术给所有方法加上TryCatch捕获异常并输出</code></a></li>
</ul>
<h2><a id="user-content-paw_prints-我的大学四年到毕业工作5年的学习路线资源和面试汇总" class="anchor" aria-hidden="true" href="#paw_prints-我的大学四年到毕业工作5年的学习路线资源和面试汇总"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><g-emoji class="g-emoji" alias="feet" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f43e.png">🐾</g-emoji> 我的大学四年到毕业工作5年的学习路线资源和面试汇总</h2>
<p><em>一直有伙伴问小傅哥，有没有一个Java的学习路线和面试，最好再有一些相关的资料、书籍、视频。因为现在自己学习也不知道哪不会，看到这个学这个，看到那个学那个，也摸不到头，还比较混乱。特别希望有一个大学到毕业的学习路线整理。</em></p>
<ul>
<li><a href="https://bugstack.cn/itstack-code-life/2020/03/31/%E5%A4%A7%E5%AD%A6%E5%9B%9B%E5%B9%B4%E5%88%B0%E6%AF%95%E4%B8%9A%E5%B7%A5%E4%BD%9C5%E5%B9%B4%E7%9A%84%E5%AD%A6%E4%B9%A0%E8%B7%AF%E7%BA%BF%E8%B5%84%E6%BA%90%E6%B1%87%E6%80%BB.html" rel="nofollow"><code>大学四年到毕业工作5年的学习路线资源汇总</code></a></li>
<li><a href="https://bugstack.cn/itstack-code-life/2020/04/11/%E5%B7%A5%E4%BD%9C%E4%B8%A4%E5%B9%B4%E7%AE%80%E5%8E%86%E5%86%99%E6%88%90%E8%BF%99%E6%A0%B7-%E8%B0%81%E8%A6%81%E4%BD%A0%E5%91%80.html" rel="nofollow"><code>工作两年简历写成这样，谁要你呀！</code></a></li>
</ul>
<h2><a id="user-content-walking-netty仿桌面版微信聊天" class="anchor" aria-hidden="true" href="#walking-netty仿桌面版微信聊天"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><g-emoji class="g-emoji" alias="walking" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f6b6.png">🚶</g-emoji> Netty仿桌面版微信聊天</h2>
<p><em>使用JavaFx、Netty4.x、SpringBoot、Mysql等技术栈和偏向于DDD领域驱动设计方式，搭建的仿桌面版微信聊天工程实现通信核心功能。如果本项目能为您提供帮助，请给予支持(关注、点赞、分享)！</em></p>
<ul>
<li><a href="https://chat.istack.org" rel="nofollow"><code>《Netty+JavaFx实战：仿桌面版微信聊天》</code></a></li>
<li><a href="https://mp.weixin.qq.com/s/OmXCY4fTfDpkvjlg5ME0ZA" rel="nofollow"><code>《Netty+JavaFx实战：仿桌面版微信聊天》代码开源、上云部署、视频讲解，只为让你给点个Star！</code></a></li>
</ul>
<h2><a id="user-content-bike-字节码编程专栏" class="anchor" aria-hidden="true" href="#bike-字节码编程专栏"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><g-emoji class="g-emoji" alias="bike" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f6b2.png">🚲</g-emoji> 字节码编程专栏</h2>
<ul>
<li><a href="https://bugstack.cn/itstack-demo-agent/2020/04/19/%E5%AD%97%E8%8A%82%E7%A0%81%E7%BC%96%E7%A8%8B-Javassist%E7%AF%87%E4%B8%80-%E5%9F%BA%E4%BA%8Ejavassist%E7%9A%84%E7%AC%AC%E4%B8%80%E4%B8%AA%E6%A1%88%E4%BE%8Bhelloworld.html" rel="nofollow"><code>字节码编程，Javassist篇一《基于javassist的第一个案例helloworld》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-agent/2020/04/20/%E5%AD%97%E8%8A%82%E7%A0%81%E7%BC%96%E7%A8%8B-Javassist%E7%AF%87%E4%BA%8C-%E5%AE%9A%E4%B9%89%E5%B1%9E%E6%80%A7%E4%BB%A5%E5%8F%8A%E5%88%9B%E5%BB%BA%E6%96%B9%E6%B3%95%E6%97%B6%E5%A4%9A%E7%A7%8D%E5%85%A5%E5%8F%82%E5%92%8C%E5%87%BA%E5%8F%82%E7%B1%BB%E5%9E%8B%E7%9A%84%E4%BD%BF%E7%94%A8.html" rel="nofollow"><code>字节码编程，Javassist篇二《定义属性以及创建方法时多种入参和出参类型的使用》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-agent/2020/04/21/%E5%AD%97%E8%8A%82%E7%A0%81%E7%BC%96%E7%A8%8B-Javassist%E7%AF%87%E4%B8%89-%E4%BD%BF%E7%94%A8Javassist%E5%9C%A8%E8%BF%90%E8%A1%8C%E6%97%B6%E9%87%8D%E6%96%B0%E5%8A%A0%E8%BD%BD%E7%B1%BB-%E6%9B%BF%E6%8D%A2%E5%8E%9F%E6%96%B9%E6%B3%95%E8%BE%93%E5%87%BA%E4%B8%8D%E4%B8%80%E6%A0%B7%E7%9A%84%E7%BB%93%E6%9E%9C.html" rel="nofollow"><code>字节码编程，Javassist篇三《使用Javassist在运行时重新加载类「替换原方法输出不一样的结果」》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-agent/2020/04/27/%E5%AD%97%E8%8A%82%E7%A0%81%E7%BC%96%E7%A8%8B-Javassist%E7%AF%87%E5%9B%9B-%E9%80%9A%E8%BF%87%E5%AD%97%E8%8A%82%E7%A0%81%E6%8F%92%E6%A1%A9%E7%9B%91%E6%8E%A7%E6%96%B9%E6%B3%95%E9%87%87%E9%9B%86%E8%BF%90%E8%A1%8C%E6%97%B6%E5%85%A5%E5%8F%82%E5%87%BA%E5%8F%82%E5%92%8C%E5%BC%82%E5%B8%B8%E4%BF%A1%E6%81%AF.html" rel="nofollow"><code>字节码编程，Javassist篇四《通过字节码插桩监控方法采集运行时入参出参和异常信息》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-agent/2020/04/29/%E5%AD%97%E8%8A%82%E7%A0%81%E7%BC%96%E7%A8%8B-Javassist%E7%AF%87%E4%BA%94-%E4%BD%BF%E7%94%A8Bytecode%E6%8C%87%E4%BB%A4%E7%A0%81%E7%94%9F%E6%88%90%E5%90%AB%E6%9C%89%E8%87%AA%E5%AE%9A%E4%B9%89%E6%B3%A8%E8%A7%A3%E7%9A%84%E7%B1%BB%E5%92%8C%E6%96%B9%E6%B3%95.html" rel="nofollow"><code>字节码编程，Javassist篇五《使用Bytecode指令码生成含有自定义注解的类和方法》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-agent/2020/05/08/%E5%AD%97%E8%8A%82%E7%A0%81%E7%BC%96%E7%A8%8B-Byte-buddy%E7%AF%87%E4%B8%80-%E5%9F%BA%E4%BA%8EByte-Buddy%E8%AF%AD%E6%B3%95%E5%88%9B%E5%BB%BA%E7%9A%84%E7%AC%AC%E4%B8%80%E4%B8%AAHelloWorld.html" rel="nofollow"><code>字节码编程，Byte-buddy篇一《基于Byte Buddy语法创建的第一个HelloWorld》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-agent/2020/05/12/%E5%AD%97%E8%8A%82%E7%A0%81%E7%BC%96%E7%A8%8B-Byte-buddy%E7%AF%87%E4%BA%8C-%E7%9B%91%E6%8E%A7%E6%96%B9%E6%B3%95%E6%89%A7%E8%A1%8C%E8%80%97%E6%97%B6%E5%8A%A8%E6%80%81%E8%8E%B7%E5%8F%96%E5%87%BA%E5%85%A5%E5%8F%82%E7%B1%BB%E5%9E%8B%E5%92%8C%E5%80%BC.html" rel="nofollow"><code>字节码编程，Byte-buddy篇二《监控方法执行耗时动态获取出入参类型和值》</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-agent/2020/05/14/%E5%AD%97%E8%8A%82%E7%A0%81%E7%BC%96%E7%A8%8B-Byte-buddy%E7%AF%87%E4%B8%89-%E4%BD%BF%E7%94%A8%E5%A7%94%E6%89%98%E5%AE%9E%E7%8E%B0%E6%8A%BD%E8%B1%A1%E7%B1%BB%E6%96%B9%E6%B3%95%E5%B9%B6%E6%B3%A8%E5%85%A5%E8%87%AA%E5%AE%9A%E4%B9%89%E6%B3%A8%E8%A7%A3%E4%BF%A1%E6%81%AF.html" rel="nofollow"><code>字节码编程，Byte-buddy篇三《使用委托实现抽象类方法并注入自定义注解信息》</code></a></li>
</ul>
<h2><a id="user-content-school_satchel-实战设计模式" class="anchor" aria-hidden="true" href="#school_satchel-实战设计模式"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><g-emoji class="g-emoji" alias="school_satchel" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f392.png">🎒</g-emoji> 实战设计模式</h2>
<h3><a id="user-content-创建型模式" class="anchor" aria-hidden="true" href="#创建型模式"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>创建型模式</h3>
<ul>
<li><a href="https://bugstack.cn/itstack-demo-design/2020/05/20/%E9%87%8D%E5%AD%A6Java%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F-%E5%AE%9E%E6%88%98%E5%B7%A5%E5%8E%82%E6%96%B9%E6%B3%95%E6%A8%A1%E5%BC%8F.html" rel="nofollow"><code>1. 重学 Java 设计模式：实战工厂方法模式「多种类型商品不同接口，统一发奖服务搭建场景」</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-design/2020/05/24/%E9%87%8D%E5%AD%A6Java%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F-%E6%8A%BD%E8%B1%A1%E5%B7%A5%E5%8E%82%E6%A8%A1%E5%BC%8F.html" rel="nofollow"><code>2. 重学 Java 设计模式：实战抽象工厂模式「替换Redis双集群升级，代理类抽象场景」</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-design/2020/05/26/%E9%87%8D%E5%AD%A6Java%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F-%E5%AE%9E%E6%88%98%E5%BB%BA%E9%80%A0%E8%80%85%E6%A8%A1%E5%BC%8F.html" rel="nofollow"><code>3. 重学 Java 设计模式：实战建造者模式「各项装修物料组合套餐选配场景」</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-design/2020/05/28/%E9%87%8D%E5%AD%A6-Java-%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F-%E5%AE%9E%E6%88%98%E5%8E%9F%E5%9E%8B%E6%A8%A1%E5%BC%8F.html" rel="nofollow"><code>4. 重学 Java 设计模式：实战原型模式「上机考试多套试，每人题目和答案乱序排列场景」</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-design/2020/05/31/%E9%87%8D%E5%AD%A6-Java-%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F-%E5%AE%9E%E6%88%98%E5%8D%95%E4%BE%8B%E6%A8%A1%E5%BC%8F.html" rel="nofollow"><code>5. 重学 Java 设计模式：实战单例模式「7种单例模式案例，Effective Java 作者推荐枚举单例模式」</code></a></li>
</ul>
<h3><a id="user-content-结构型模式" class="anchor" aria-hidden="true" href="#结构型模式"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>结构型模式</h3>
<ul>
<li><a href="https://bugstack.cn/itstack-demo-design/2020/06/02/%E9%87%8D%E5%AD%A6-Java-%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F-%E9%80%82%E9%85%8D%E5%99%A8%E6%A8%A1%E5%BC%8F.html" rel="nofollow"><code>1. 重学 Java 设计模式：实战适配器模式「从多个MQ消息体中，抽取指定字段值场景」)</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-design/2020/06/04/%E9%87%8D%E5%AD%A6-Java-%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F-%E5%AE%9E%E6%88%98%E6%A1%A5%E6%8E%A5%E6%A8%A1%E5%BC%8F.html" rel="nofollow"><code>2. 重学 Java 设计模式：实战桥接模式「多支付渠道(微信、支付宝)与多支付模式(刷脸、指纹)场景」</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-design/2020/06/08/%E9%87%8D%E5%AD%A6-Java-%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F-%E5%AE%9E%E6%88%98%E7%BB%84%E5%90%88%E6%A8%A1%E5%BC%8F.html" rel="nofollow"><code>3. 重学 Java 设计模式：实战组合模式「营销差异化人群发券，决策树引擎搭建场景」</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-design/2020/06/09/%E9%87%8D%E5%AD%A6-Java-%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F-%E5%AE%9E%E6%88%98%E8%A3%85%E9%A5%B0%E5%99%A8%E6%A8%A1%E5%BC%8F.html" rel="nofollow"><code>4. 重学 Java 设计模式：实战装饰器模式「SSO单点登录功能扩展，增加拦截用户访问方法范围场景」</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-design/2020/06/11/%E9%87%8D%E5%AD%A6-Java-%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F-%E5%AE%9E%E6%88%98%E5%A4%96%E8%A7%82%E6%A8%A1%E5%BC%8F.html" rel="nofollow"><code>5. 重学 Java 设计模式：实战外观模式「基于SpringBoot开发门面模式中间件，统一控制接口白名单场景」</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-design/2020/06/14/%E9%87%8D%E5%AD%A6-Java-%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F-%E5%AE%9E%E6%88%98%E4%BA%AB%E5%85%83%E6%A8%A1%E5%BC%8F.html" rel="nofollow"><code>6. 重学 Java 设计模式：实战享元模式「基于Redis秒杀，提供活动与库存信息查询场景」</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-design/2020/06/16/%E9%87%8D%E5%AD%A6-Java-%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F-%E5%AE%9E%E6%88%98%E4%BB%A3%E7%90%86%E6%A8%A1%E5%BC%8F.html" rel="nofollow"><code>7. 重学 Java 设计模式：实战代理模式「模拟mybatis-spring中定义DAO接口，使用代理类方式操作数据库原理实现场景」</code></a></li>
</ul>
<h3><a id="user-content-行为模式" class="anchor" aria-hidden="true" href="#行为模式"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>行为模式</h3>
<ul>
<li><a href="https://bugstack.cn/itstack-demo-design/2020/06/18/%E9%87%8D%E5%AD%A6-Java-%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F-%E5%AE%9E%E6%88%98%E8%B4%A3%E4%BB%BB%E9%93%BE%E6%A8%A1%E5%BC%8F.html" rel="nofollow"><code>1. 重学 Java 设计模式：实战责任链模式「模拟618电商大促期间，项目上线流程多级负责人审批场景」</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-design/2020/06/21/%E9%87%8D%E5%AD%A6-Java-%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F-%E5%AE%9E%E6%88%98%E5%91%BD%E4%BB%A4%E6%A8%A1%E5%BC%8F.html" rel="nofollow"><code>2. 重学 Java 设计模式：实战命令模式「模拟高档餐厅八大菜系，小二点单厨师烹饪场景」</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-design/2020/06/23/%E9%87%8D%E5%AD%A6-Java-%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F-%E5%AE%9E%E6%88%98%E8%BF%AD%E4%BB%A3%E5%99%A8%E6%A8%A1%E5%BC%8F.html" rel="nofollow"><code>3. 重学 Java 设计模式：实战迭代器模式「模拟公司组织架构树结构关系，深度迭代遍历人员信息输出场景」</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-design/2020/06/27/%E9%87%8D%E5%AD%A6-Java-%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F-%E5%AE%9E%E6%88%98%E4%B8%AD%E4%BB%8B%E8%80%85%E6%A8%A1%E5%BC%8F.html" rel="nofollow"><code>4. 重学 Java 设计模式：实战中介者模式「按照Mybatis原理手写ORM框架，给JDBC方式操作数据库增加中介者场景」</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-design/2020/06/28/%E9%87%8D%E5%AD%A6-Java-%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F-%E5%AE%9E%E6%88%98%E5%A4%87%E5%BF%98%E5%BD%95%E6%A8%A1%E5%BC%8F.html" rel="nofollow"><code>5. 重学 Java 设计模式：实战备忘录模式「模拟互联网系统上线过程中，配置文件回滚场景」</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-design/2020/06/30/%E9%87%8D%E5%AD%A6-Java-%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F-%E5%AE%9E%E6%88%98%E8%A7%82%E5%AF%9F%E8%80%85%E6%A8%A1%E5%BC%8F.html" rel="nofollow"><code>6. 重学 Java 设计模式：实战观察者模式「模拟类似小客车指标摇号过程，监听消息通知用户中签场景」</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-design/2020/07/02/%E9%87%8D%E5%AD%A6-Java-%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F-%E5%AE%9E%E6%88%98%E7%8A%B6%E6%80%81%E6%A8%A1%E5%BC%8F.html" rel="nofollow"><code>7. 重学 Java 设计模式：实战状态模式「模拟系统营销活动，状态流程审核发布上线场景」</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-design/2020/07/05/%E9%87%8D%E5%AD%A6-Java-%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F-%E5%AE%9E%E6%88%98%E7%AD%96%E7%95%A5%E6%A8%A1%E5%BC%8F.html" rel="nofollow"><code>8. 重学 Java 设计模式：实战策略模式「模拟多种营销类型优惠券，折扣金额计算策略场景」</code></a></li>
<li><a href="https://bugstack.cn/itstack-demo-design/2020/07/07/%E9%87%8D%E5%AD%A6-Java-%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F-%E5%AE%9E%E6%88%98%E6%A8%A1%E6%9D%BF%E6%A8%A1%E5%BC%8F.html" rel="nofollow"><code>9. 重学 Java 设计模式：实战模版模式「模拟爬虫各类电商商品，生成营销推广海报场景」</code></a></li>
</ul>
<h2><a id="user-content-ferris_wheel-其他文章" class="anchor" aria-hidden="true" href="#ferris_wheel-其他文章"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><g-emoji class="g-emoji" alias="ferris_wheel" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f3a1.png">🎡</g-emoji> 其他文章</h2>
<ul>
<li><a href="https://bugstack.cn/itstack-demo-any/2020/05/05/%E6%B1%89%E5%AD%97%E4%B8%8D%E8%83%BD%E7%BC%96%E7%A8%8B-%E5%88%AB%E9%97%B9%E4%BA%86-%E5%8F%AA%E6%98%AF%E7%9C%8B%E7%9D%80%E6%9C%89%E7%82%B9%E8%B1%AA%E6%A8%AA-%E5%AE%B9%E6%98%93%E8%A2%AB%E5%BC%80%E9%99%A4.html" rel="nofollow"><code>汉字不能编程？别闹了，只是看着有点豪横！容易被开除！</code></a> - <a href="https://github.com/fuzhengwei/CodeGuide/tree/master/src/itstack-demo-01">源码</a></li>
</ul>
<hr>
<h2><a id="user-content-转载分享" class="anchor" aria-hidden="true" href="#转载分享"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>转载分享</h2>
<p><em>建立本开源项目的初衷是基于个人学习与工作中对 Java 相关技术栈的总结记录，在这里也希望能帮助一些在学习 Java 过程中遇到问题的小伙伴，如果您需要转载本仓库的一些文章到自己的博客，请按照以下格式注明出处，谢谢合作。</em></p>
<pre><code>作者：小傅哥
链接：https://bugstack.cn
来源：bugstack虫洞栈
</code></pre>
<h2><a id="user-content-与我联系" class="anchor" aria-hidden="true" href="#与我联系"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>与我联系</h2>
<ul>
<li>
<p><strong>加群交流</strong>
本群的宗旨是给大家提供一个良好的技术学习交流平台，所以杜绝一切广告！由于微信群人满 100 之后无法加入，请扫描下方二维码先添加作者 “小傅哥” 微信(fustack)，备注：加群。</p>
  <a target="_blank" rel="noopener noreferrer" href="https://camo.githubusercontent.com/089934aac354c4ee52b696688588edbda71270ea/68747470733a2f2f6974737461636b2e6f72672f5f6d656469612f6675737461636b2e706e673f782d6f73732d70726f636573733d7374796c652f6d6179"><img src="https://camo.githubusercontent.com/089934aac354c4ee52b696688588edbda71270ea/68747470733a2f2f6974737461636b2e6f72672f5f6d656469612f6675737461636b2e706e673f782d6f73732d70726f636573733d7374796c652f6d6179" width="180" height="180" data-canonical-src="https://itstack.org/_media/fustack.png?x-oss-process=style/may" style="max-width:100%;"></a>
</li>
<li>
<p><strong>公众号(bugstack虫洞栈)</strong>
沉淀、分享、成长，专注于原创专题案例，以最易学习编程的方式分享知识，让自己和他人都能有所收获。目前已完成的专题有；Netty4.x实战专题案例、用Java实现JVM、基于JavaAgent的全链路监控、手写RPC框架、DDD专题案例、源码分析等。</p>
  <a target="_blank" rel="noopener noreferrer" href="https://camo.githubusercontent.com/2c4dc64fa24dc5a658c359b69166bdb4cb79c4a6/68747470733a2f2f6974737461636b2e6f72672f5f6d656469612f7172636f64652e706e673f782d6f73732d70726f636573733d7374796c652f6d6179"><img src="https://camo.githubusercontent.com/2c4dc64fa24dc5a658c359b69166bdb4cb79c4a6/68747470733a2f2f6974737461636b2e6f72672f5f6d656469612f7172636f64652e706e673f782d6f73732d70726f636573733d7374796c652f6d6179" width="180" height="180" data-canonical-src="https://itstack.org/_media/qrcode.png?x-oss-process=style/may" style="max-width:100%;"></a>
</li>
</ul>
<h2><a id="user-content-参与贡献" class="anchor" aria-hidden="true" href="#参与贡献"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>参与贡献</h2>
<ol>
<li>如果您对本项目有任何建议或发现文中内容有误的，欢迎提交 issues 进行指正。</li>
<li>对于文中我没有涉及到知识点，欢迎提交 PR。</li>
</ol>
<h2><a id="user-content-致谢" class="anchor" aria-hidden="true" href="#致谢"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>致谢</h2>
<p>感谢以下人员对本仓库做出的贡献或者对小傅哥的赞赏，当然不仅仅只有这些贡献者，这里就不一一列举了。如果你希望被添加到这个名单中，并且提交过 Issue 或者 PR，请与我联系。</p>
<p><strong><g-emoji class="g-emoji" alias="seedling" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f331.png">🌱</g-emoji> 感谢大家对仓库建设的贡献</strong></p>
<a href="https://github.com/linw7">
    <img src="https://avatars0.githubusercontent.com/u/3761578?s=460&amp;v=4" width="50px" style="max-width:100%;">
</a> 
<a href="https://github.com/g10guang">
    <img src="https://avatars0.githubusercontent.com/u/30902679?s=400&amp;v=4" width="50px" style="max-width:100%;">
</a> 
<a href="https://github.com/g10guang">
    <img src="https://avatars1.githubusercontent.com/u/15908832?s=180&amp;v=4" width="50px" style="max-width:100%;">
</a>
<hr>
<p><strong><g-emoji class="g-emoji" alias="gift_heart" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f49d.png">💝</g-emoji> 感谢大家对我资金的赞赏</strong></p>
<table>
<thead>
<tr>
<th>时间</th>
<th>小伙伴</th>
<th>赞赏金额</th>
</tr>
</thead>
<tbody>
<tr>
<td>2020-06-16</td>
<td>贾学兵</td>
<td>5.00元</td>
</tr>
<tr>
<td>2020-06-11</td>
<td>刘洪泽</td>
<td>6.66元</td>
</tr>
<tr>
<td>2020-06-05</td>
<td><a href="https://github.com/996546860">时光之刃</a></td>
<td>5元</td>
</tr>
<tr>
<td>2020-05-25</td>
<td><a href="https://juejin.im/user/5db135d86fb9a020512b3289/posts" rel="nofollow">柠檬楠</a></td>
<td>23.33元</td>
</tr>
<tr>
<td>2020-05-19</td>
<td>王刚</td>
<td>20元</td>
</tr>
<tr>
<td>2020-05-19</td>
<td>如鱼</td>
<td>3元</td>
</tr>
<tr>
<td>2020-05-18</td>
<td>帅地</td>
<td>6.66元</td>
</tr>
<tr>
<td>2020-05-18</td>
<td>放飞心情</td>
<td>6元</td>
</tr>
<tr>
<td>2020-05-18</td>
<td>lemon</td>
<td>1元</td>
</tr>
<tr>
<td>2020-05-18</td>
<td>贺</td>
<td>1元</td>
</tr>
<tr>
<td>2020-05-18</td>
<td>!sssss</td>
<td>1元</td>
</tr>
<tr>
<td>2020-05-18</td>
<td>ZHANG</td>
<td>1元</td>
</tr>
<tr>
<td>2020-05-18</td>
<td>vovovov</td>
<td>1元</td>
</tr>
<tr>
<td>2020-04-01</td>
<td>姬贵阳</td>
<td>1元</td>
</tr>
<tr>
<td>2020-02-29</td>
<td>日落黄昏下</td>
<td>1元</td>
</tr>
<tr>
<td>2019-12-26</td>
<td>clearDay</td>
<td>1元</td>
</tr>
<tr>
<td>2019-11-27</td>
<td>Jasonzhou</td>
<td>1元</td>
</tr>
<tr>
<td>2019-11-08</td>
<td>贺</td>
<td>1元</td>
</tr>
<tr>
<td>2019-08-06</td>
<td>贺</td>
<td>1元</td>
</tr>
</tbody>
</table>
</article>
      </div>
  </div>


</div>

    <div class="flex-shrink-0 col-12 col-md-3">
            

      <div class="BorderGrid BorderGrid--spacious" data-pjax="">
        <div class="BorderGrid-row hide-sm hide-md">
          <div class="BorderGrid-cell">
            <h2 class="mb-3 h4">About</h2>

    <p class="f4 mt-3">
      
<g-emoji class="g-emoji" alias="books" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f4da.png">📚</g-emoji> 本代码库是作者小傅哥多年从事一线互联网 Java 开发的学习历程技术汇总，旨在为大家提供一个清晰详细的学习教程，侧重点更倾向编写Java核心内容。如果本仓库能为您提供帮助，请给予支持(关注、点赞、分享)！
    </p>
    <div class="mt-3 d-flex flex-items-center">
      <svg height="16" class="octicon octicon-link flex-shrink-0 mr-2" mr="2" classes="flex-shrink-0" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg>

      <span class="flex-auto min-width-0 css-truncate css-truncate-target width-fit">
        <a title="https://bugstack.cn" role="link" target="_blank" class="text-bold" rel="noopener noreferrer" href="https://bugstack.cn">bugstack.cn</a>
      </span>
    </div>

  <h3 class="sr-only">Topics</h3>
  <div class="mt-3">
      <div class="f6">
      <a class="topic-tag topic-tag-link " data-ga-click="Topic, repository page" data-octo-click="topic_click" data-octo-dimensions="topic:java" href="/topics/java" title="Topic: java">
  java
</a>

      <a class="topic-tag topic-tag-link " data-ga-click="Topic, repository page" data-octo-click="topic_click" data-octo-dimensions="topic:javafx" href="/topics/javafx" title="Topic: javafx">
  javafx
</a>

      <a class="topic-tag topic-tag-link " data-ga-click="Topic, repository page" data-octo-click="topic_click" data-octo-dimensions="topic:spring" href="/topics/spring" title="Topic: spring">
  spring
</a>

      <a class="topic-tag topic-tag-link " data-ga-click="Topic, repository page" data-octo-click="topic_click" data-octo-dimensions="topic:mybaits" href="/topics/mybaits" title="Topic: mybaits">
  mybaits
</a>

      <a class="topic-tag topic-tag-link " data-ga-click="Topic, repository page" data-octo-click="topic_click" data-octo-dimensions="topic:asm" href="/topics/asm" title="Topic: asm">
  asm
</a>

      <a class="topic-tag topic-tag-link " data-ga-click="Topic, repository page" data-octo-click="topic_click" data-octo-dimensions="topic:bytecode" href="/topics/bytecode" title="Topic: bytecode">
  bytecode
</a>

      <a class="topic-tag topic-tag-link " data-ga-click="Topic, repository page" data-octo-click="topic_click" data-octo-dimensions="topic:javassist" href="/topics/javassist" title="Topic: javassist">
  javassist
</a>

      <a class="topic-tag topic-tag-link " data-ga-click="Topic, repository page" data-octo-click="topic_click" data-octo-dimensions="topic:aop" href="/topics/aop" title="Topic: aop">
  aop
</a>

      <a class="topic-tag topic-tag-link " data-ga-click="Topic, repository page" data-octo-click="topic_click" data-octo-dimensions="topic:springboot" href="/topics/springboot" title="Topic: springboot">
  springboot
</a>

      <a class="topic-tag topic-tag-link " data-ga-click="Topic, repository page" data-octo-click="topic_click" data-octo-dimensions="topic:mysql" href="/topics/mysql" title="Topic: mysql">
  mysql
</a>

      <a class="topic-tag topic-tag-link " data-ga-click="Topic, repository page" data-octo-click="topic_click" data-octo-dimensions="topic:drools" href="/topics/drools" title="Topic: drools">
  drools
</a>

      <a class="topic-tag topic-tag-link " data-ga-click="Topic, repository page" data-octo-click="topic_click" data-octo-dimensions="topic:ddd" href="/topics/ddd" title="Topic: ddd">
  ddd
</a>

  </div>

  </div>

  <h3 class="sr-only">Resources</h3>
  <div class="mt-3">
    <a class="muted-link" href="#readme">
      <svg height="16" class="octicon octicon-book mr-2" mr="2" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M0 1.75A.75.75 0 01.75 1h4.253c1.227 0 2.317.59 3 1.501A3.744 3.744 0 0111.006 1h4.245a.75.75 0 01.75.75v10.5a.75.75 0 01-.75.75h-4.507a2.25 2.25 0 00-1.591.659l-.622.621a.75.75 0 01-1.06 0l-.622-.621A2.25 2.25 0 005.258 13H.75a.75.75 0 01-.75-.75V1.75zm8.755 3a2.25 2.25 0 012.25-2.25H14.5v9h-3.757c-.71 0-1.4.201-1.992.572l.004-7.322zm-1.504 7.324l.004-5.073-.002-2.253A2.25 2.25 0 005.003 2.5H1.5v9h3.757a3.75 3.75 0 011.994.574z"></path></svg>

      Readme
</a>  </div>


          </div>
        </div>
          <div class="BorderGrid-row">
            <div class="BorderGrid-cell">
              <h2 class="h4 mb-3">
  <a class="link-gray-dark no-underline " href="/fuzhengwei/CodeGuide/releases">
    Releases
</a>

</h2>

    <div class="text-small">No releases published</div>

            </div>
          </div>
      </div>

</div>
</div>




  </div>


