# PyMNA Pro Web

Browser-based DC operating-point analyzer with component tolerances.
部品公差つき直流動作点解析ツール(Web版)

**▶ Try it / 使ってみる:** https://zyuta0720-cmd.github.io/pymna-web/ ([English](https://zyuta0720-cmd.github.io/pymna-web/index.en.html))

## Features / 機能
- Worst-case analysis / ワーストケース解析(感度+反復探索)
- Tornado sensitivity chart / トルネードチャート
- Monte Carlo (Gaussian / Uniform) / モンテカルロ
- Resistor power check with temperature derating / 抵抗の電力判定(温度ディレーティング)
- SPICE-like netlist: R, V, I, E, F, G, H, C, L, D

All calculations run locally in your browser. No data is sent anywhere.
計算はすべてブラウザ内で行われ、入力データは外部に送信されません。

## Verification / 検証
Nominal node voltages match LTspice for a 20-resistor mesh network (within LTspice's convergence tolerance).
20抵抗のメッシュ回路で、公称値の動作点が LTspice と一致することを確認済み。

## Limitations / 制限事項
- Worst case uses sensitivity-sign + iterative search, not exhaustive enumeration.
- Max resistor power is evaluated only over node-voltage worst-case combinations and may be optimistic for floating resistors.
- Results are for reference only. Verify final designs by other means.

## License
MIT © 2026 Zyutama

This is a personal project and is not affiliated with any company.
個人で開発したもので、特定の企業とは関係ありません。
