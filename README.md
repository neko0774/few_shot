# 更新方法
'git pull' をする

# 使い方
imgsに画像をいれる
画像の形式はjpg, 名前は1.jpg, 2.jpg, ...の形にする
shotsの数はmain.pyの内部の nb_features = 3 の数を変更する．
wayの数を変えたい場合はpossible_input_pynq/keyboardの編集が必要

画像が入っているかずよりもwayの数が多い場合はエラーが生じる．

重みファイルを適切に設定する必要がある．テスト用に重みファイルが準備してある，
python main.py --framework pytorch --device-pytorch cpu --path-pytorch-weight weights/cifarfs_resnet12_res84_map32_epoch100.pt
は動くはず．

# その他参照

https://github.com/brain-bzh/PEFSL/tree/main