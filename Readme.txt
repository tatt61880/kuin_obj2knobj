Obj.kn v1.00 (for Kuin 1.00):
    Last Modified: 2014/01/06 19:13:37.
    Created by Tatt(@tatt61880)
    https://twitter.com/tatt61880
    https://github.com/tatt61880

objファイルをknobjファイルに変換するプログラムです。

ファイルの説明:
    Obj.kn
        objファイルを扱うライブラリです。

    Obj2knobj.kn
        mybox.objを読み込んで、mybox.knobjを作成します。

    Resフォルダ
        Obj2knobj.exe で使用するファイル(mybox.obj)が入っています。

Spetial Thanks, cohfinさん for the Info below.
struct knobj {
	u64 anim_flag;
	if (anim_flag) {
		データ構造未解析
	}
	u64 num_groups;
	struct group[num_groups] {
		u64 num_triangles;
		struct triangles[num_triangles] {
			struct vertices[3] {
				f64 x;
				f64 y;
				f64 z;
				f64 u;
				f64 v;
				f64 nx;
				f64 ny;
				f64 nz;
			};
		};
	};
};
