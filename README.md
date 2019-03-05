# MMPhoto
一个图片浏览器
接手公司项目后发现图片浏览没有滑动关闭的功能，所以在此基础上加上了
用法
MMPhotoViewController *vc = [[MMPhotoViewController alloc] init];
    vc.urlArray = @[@"https://img-my.csdn.net/uploads/201407/26/1406383299_1976.jpg",
                    @"https://img-my.csdn.net/uploads/201407/26/1406383291_6518.jpg",
                    @"https://img-my.csdn.net/uploads/201407/26/1406383291_8239.jpg"
                   ];
    vc.imgIndex = 1;
    if (btn.tag == 1000) {
        vc.rect = btn.frame;//传一个frame,消失时会回归原位，不传会在手指离开的位置消失
    }
    
    [self.view addSubview:vc.view];
    [self addChildViewController:vc];
    
![image](https://github.com/nantianwang/MMPhoto/blob/master/IMB_O30ccN.GIF)
    
