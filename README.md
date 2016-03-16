# photoflood
相册访问器

//显示Image Picker
//这边的一为选择照片的最大数量
                PtosGroupNavControllwer *nav = [PtosGroupNavControllwer photosNavVc:1];
                __weak typeof(self) weakself = self;
                //相册最后选择图片
                nav.lastDataBlock = ^(NSArray *array){
                    for (PhotosImageInfoModel *model in array) {
                        
                        [weakself setBUTimage:model.originImage];
                        
                    }
                };
