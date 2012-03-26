1.Tabbed Applicationで新規プロジェクトを作る
New project is made(Tabbed Application). 

2.MasterViewController、DetailViewControllerをUIViewControllerで作成(New File)
MasterViewController and DetailViewController is made(UIViewController,New File).

3.iOS→Core Data→Data Modelを選択、プロジェクト名.xcdatamodeldで新規ファイルを作成
New File,iOS→Core Data→Data Model,ProjectName.xcdatamodeld(New File).

4.プロジェクト→TARGETS→Linked Frameworks and Librariesの+をクリックして、CoreData.frameworkを選択、追加する
Project→TARGETS→Linked Frameworks and Libraries→+button→CoreData.framework

5.Supporting Files→プロジェクト名-Prefix.pchをクリックし、#endifの前に#import <CoreData/CoreData.h>を付け加える
Supporting Files→ProjectName-Prefix.pch→Add "#import <CoreData/CoreData.h>"

6.プロジェクト名.xcdatamodeldのAdd EntityをクリックしてENTITESに「Event」と入力、Attributesの+をクリックして「timeStamp」と入力、TypeをDateにする
ProjectName.xcdatamodeld→Add Entity→ENTITES input "Event"→Attributes + →timeStamp,Type:Date

7.MainStoryboard.storyboardにNavigation ControllerとView ControllerなどUIパーツを配置して結んでいく。TableはNavigation Controllerを配置した際にくっついてくるView ControllerにTable Viewを配置すればOK。ユーザにデータを入力させるタイプのプロジェクトの場合はTable ViewのContentはDynamic Prototypesに、Table View CellのStyleはBasicにしてIdentiferに「Cell」と入力する
UIpart is arranged. Table View-Content "Dynamic Prototypes",Table View Cell-Basic-Identifer "Cell"

8.Table ViewをViewの上にドラッグする。VIewが見えなくなるが大丈夫
Table View is dragged on View.
 
9.Table Viewを右クリックして、dataSourceとdelegateをView Controllerまでドラッグして結びつける
Table View right-click,dataSource-View Controller,delegate-View Controller.

10.View Controller -Root View ControllerとView Controllerをクリックして、ClassをそれぞれMasterViewController、DetailViewControllerにする
View Controller -Root View Controller's class "MasterViewController",View Controller's class "DetailViewController".

11.AppDelegate.hと.mの//追加 と書かれている部分を追加する(この時点でエラーがひとつ出てますが気にしないでOK)
AppDelegate.h and .m add code.
12.MasterViewController.hと.mの//追加 と書かれている部分を追加する
MasterViewController.h and. m add code.

13.DetailViewController.hと.mの//追加 と書かれている部分を追加する
DetailViewController.h and. m add code.
