# Git基本概念及應用

git 版本控制可以幫你紀錄一個專案（repository）裡面，只要下一個commit指令就可以紀錄曾經做過得更動（新增編輯刪除檔案）。因此，可以在完成到特定段落時使用commit功能，就可以為當下的版本留下紀錄，哪天你想要回到那個時間點就輕而易舉拉！不用記在腦子裡了！

概念類似

你現在有一個資料夾（repository)裡面存放你最初的草稿，當你想要為資料夾加入git版本控制時使用git init，若有些不需要加入版本控制的文件就加入.gitignore檔裡，接著，因為檔案是新建立的，使用git add .將所有檔案加入tracked,然後用git commit -am "本次存檔說明文字" ，系統就會類似以新的一個資料夾幫你在當下留下紀錄，之後有任何更動都會有新的存檔動作，之後想回到哪個時間點，系統就會幫你切換到那個資料夾裡拉！

###### 想和別人（遠端）產生有連結：push pull

前面的介紹是在自己的電腦（本機）上運作，如果希望把東西放到網路上，可以用push上傳到網路；同樣也可以把東西從網路取回來，用pull下載到自己的電腦上。

**push**

先在github新增一個repository並用

```
git remote add orgin repo-url.git
```

```
git push -u origin master
```

**pull**

```
git pull origin master
```

