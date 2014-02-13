Obj.kn v1.01 (for Kuin 1.01):
	Last Modified: 2014/02/13 22:43:39.
	Created by Tatt(@tatt61880)
	https://twitter.com/tatt61880
	https://github.com/tatt61880

objファイルをknobjファイルに変換するプログラムです。

ファイルの説明:
	Obj.kn
		objファイルを扱うライブラリです。

	Obj2knobj.kn
		Obj2knobj.exe にドラッグ＆ドロップされたobjファイルを元にknobjファイルを作成します。

	Resフォルダ
		Obj2knobj.exe にドラッグ＆ドロップする objファイルのサンプル(mybox.obj)が入っています。

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
