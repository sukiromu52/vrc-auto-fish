# VRChat 自动钓鱼助手 (FISH!)


## 中文

VRChat 世界 **FISH!** 的自动钓鱼脚本。支持 YOLO 目标检测 + PD 控制器，全自动抛竿、提竿、小游戏操控。

### 功能

- **自动抛竿 / 提竿** — 检测咬钩动画，自动完成钓鱼流程
- **小游戏自动控制** — PD 控制器追踪鱼的位置，自动操控白条
- **YOLO 目标检测** — 训练后可替代模板匹配，准确率更高
- **GUI 界面** — 参数可视化调节，实时调试窗口
- **热键控制** — F9 开始/暂停，F10 停止，F11 调试模式
- **VRChat OSC 输入** — 可选 OSC 输入方式，不占用鼠标
- **多语言支持** — 支持中文、英语、日语界面切换

### 快速开始

#### 方式一：一键启动 (推荐)

1. 安装 [Python 3.10+](https://www.python.org/downloads/)（安装时勾选 **Add to PATH**）
2. 双击 **`启动.bat`** — 首次自动安装依赖，之后直接启动

> 自动检测显卡：NVIDIA GPU 安装 CUDA 加速版，AMD / Intel 安装 CPU 版，都能用。

#### 方式二：手动安装

```bash
# 安装 PyTorch (GPU 版)
pip install torch torchvision --index-url https://download.pytorch.org/whl/cu128

# 或 CPU 版
pip install torch torchvision --index-url https://download.pytorch.org/whl/cpu

# 安装其他依赖
pip install -r requirements.txt

# 启动
python main.py
```

### 使用说明

1. 先启动 VRChat 并进入 FISH! 世界
2. 运行程序，点击「选择窗口」绑定 VRChat 窗口
3. 点击「框选区域」选择钓鱼小游戏的检测范围（可选）
4. 按 **F9** 开始自动钓鱼

### 快捷键

| 按键 | 功能 |
|------|------|
| F9   | 开始 / 暂停 |
| F10  | 停止 |
| F11  | 调试模式 (显示检测窗口) |

---


## English

Auto fishing bot for VRChat world **FISH!**. Features YOLO object detection + PD controller for fully automated casting, hooking, and minigame control.

### Features

- **Auto Cast / Hook** — Detect bite animation, automate entire fishing process
- **Minigame Auto Control** — PD controller tracks fish position, automatically controls the bar
- **YOLO Object Detection** — Trainable alternative to template matching for higher accuracy
- **GUI Interface** — Visual parameter adjustment, real-time debug window
- **Hotkey Control** — F9 Start/Pause, F10 Stop, F11 Debug Mode
- **VRChat OSC Input** — Optional OSC input method, doesn't occupy mouse
- **Multi-language Support** — Switch between Chinese, English, and Japanese interfaces

### Quick Start

#### Method 1: One-click Launch (Recommended)

1. Install [Python 3.10+](https://www.python.org/downloads/) (Check **Add to PATH** during installation)
2. Double-click **`启动.bat`** — Auto-installs dependencies on first run, then launches directly

> Auto GPU detection: NVIDIA GPU installs CUDA accelerated version, AMD/Intel installs CPU version, both work.

#### Method 2: Manual Installation

```bash
# Install PyTorch (GPU version)
pip install torch torchvision --index-url https://download.pytorch.org/whl/cu128

# Or CPU version
pip install torch torchvision --index-url https://download.pytorch.org/whl/cpu

# Install other dependencies
pip install -r requirements.txt

# Launch
python main.py
```

### Usage

1. Launch VRChat and enter the FISH! world first
2. Run the program, click "Connect Window" to bind VRChat window
3. Click "Select ROI" to choose fishing minigame detection area (optional)
4. Press **F9** to start auto fishing

### Hotkeys

| Key  | Function |
|------|----------|
| F9   | Start / Pause |
| F10  | Stop |
| F11  | Debug Mode (show detection window) |

---



## 日本語

VRChat ワールド **FISH!** 用自動釣りボット。YOLO 物体検出 + PD コントローラー対応、自動キャスト、フック、ミニゲーム操作。

### 機能

- **自動キャスト / フック** — 釣りアニメーションを検出し、釣りプロセスを自動化
- **ミニゲーム自動制御** — PD コントローラーが魚の位置を追跡、バーを自動操作
- **YOLO 物体検出** — テンプレートマッチングより高精度な学習可能な検出
- **GUI インターフェース** — パラメータ可視化調整、リアルタイムデバッグウィンドウ
- **ホットキー制御** — F9 開始/一時停止、F10 停止、F11 デバッグモード
- **VRChat OSC 入力** — マウスを占有しないオプションの OSC 入力方式
- **多言語サポート** — 中国語、英語、日本語インターフェース切り替え対応

### クイックスタート

#### 方法1：ワンクリック起動（推奨）

1. [Python 3.10+](https://www.python.org/downloads/) をインストール（インストール時に **Add to PATH** をチェック）
2. **`启动.bat`** をダブルクリック — 初回のみ自動で依存関係をインストール、その後は直接起動

> 自動 GPU 検出：NVIDIA GPU は CUDA 高速版、AMD/Intel は CPU 版をインストール、どちらも動作します。

#### 方法2：手動インストール

```bash
# PyTorch のインストール（GPU 版）
pip install torch torchvision --index-url https://download.pytorch.org/whl/cu128

# または CPU 版
pip install torch torchvision --index-url https://download.pytorch.org/whl/cpu

# その他の依存関係をインストール
pip install -r requirements.txt

# 起動
python main.py
```

### 使い方

1. まず VRChat を起動し、FISH! ワールドに入る
2. プログラムを実行し、「ウィンドウ接続」で VRChat ウィンドウをバインド
3. 「検出領域選択」で釣りミニゲームの検出範囲を選択（オプション）
4. **F9** を押して自動釣りを開始

### ホットキー

| キー | 機能 |
|------|------|
| F9   | 開始 / 一時停止 |
| F10  | 停止 |
| F11  | デバッグモード（検出ウィンドウ表示） |

---

## Project Structure / 项目结构 / プロジェクト構造

```
├── main.py          # Entry / 入口 / エントリー
├── config.py        # Global config / 全局配置 / グローバル設定
├── core/            # Core logic / 核心逻辑 / コアロジック
│   ├── bot.py       # Main loop + PD controller
│   ├── detector.py  # Template matching
│   ├── yolo_detector.py  # YOLO detection
│   ├── screen.py    # Screenshot / 截屏 / スクリーンショット
│   ├── window.py    # Window management
│   └── input_ctrl.py     # Input control
├── gui/             # GUI interface / GUI 界面 / GUI インターフェース
│   └── app.py
├── utils/           # Utilities / 工具 / ユーティリティ
│   ├── logger.py
│   └── i18n.py      # Internationalization / 国际化 / 国際化
├── img/             # Template images / 模板图片 / テンプレート画像
├── yolo/            # YOLO model & training tools
├── 启动.bat          # One-click launch / 一键启动 / ワンクリック起動
├── install.bat      # Install dependencies
└── start.bat        # Start program
```

## YOLO Model Training / YOLO 模型训练 / YOLO モデル訓練

### 1. Data Collection / 采集数据 / データ収集

```bash
python -m yolo.collect               # Default 2 fps / 默认每秒 2 帧 / デフォルト每秒 2 フレーム
python -m yolo.collect --fps 4       # 4 fps / 每秒 4 帧 / 每秒 4 フレーム
python -m yolo.collect --roi         # ROI only
python -m yolo.collect --max 500     # Max 500 images / 最多 500 张 / 最大 500 枚
```

### 2. Labeling / 标注数据 / データラベリング

```bash
python -m yolo.label
python -m yolo.label --split 0.2     # 20% validation set / 20% 验证集 / 20% 検証セット
python -m yolo.label --relabel       # Relabel existing / 补标已有 / 既存の再ラベル
```

**Controls / 操作 / 操作:**

| Key / 按键 / キー | Function / 功能 / 機能 |
|------------------|------------------------|
| Mouse drag / 鼠标拖拽 / マウスドラッグ | Draw box / 画框 / ボックス描画 |
| 1 | fish (fish icon / 鱼图标 / 魚アイコン) |
| 2 | bar (white bar / 白色捕捉条 / 白いバー) |
| 3 | track (fishing track / 钓鱼轨道 / 釣り軌道) |
| 4 | progress (green bar / 绿色进度条 / 緑の進行バー) |
| Z | Undo / 撤销 / 元に戻す |
| S / Enter | Save & next / 保存并下一张 / 保存して次へ |
| D | Skip / 跳过 / スキップ |
| Q / Esc | Quit / 退出 / 終了 |

### 3. Training / 训练 / 訓練

```bash
python -m yolo.train                 # Default yolov8n, 50 epochs / 默认 50 轮 / デフォルト 50 エポック
python -m yolo.train --epochs 100    # 100 epochs / 100 轮 / 100 エポック
python -m yolo.train --model yolov8s.pt  # Larger model / 更大模型 / より大きなモデル
python -m yolo.train --resume        # Resume / 继续 / 再開
python -m yolo.train --batch 8       # Batch size / 批大小 / バッチサイズ
```

Trained model saves to / 训练后保存到 / 訓練後の保存先: `yolo/runs/fish_detect/weights/best.pt`

### Dataset Structure / 数据集目录结构 / データセット構造

```
yolo/dataset/
├── data.yaml              # Config / 配置 / 設定
├── images/
│   ├── unlabeled/         # Raw screenshots / 原始截图 / 生スクリーンショット
│   ├── train/             # Training set / 训练集 / 訓練セット
│   └── val/               # Validation set / 验证集 / 検証セット
└── labels/
    ├── train/             # Training labels / 训练标注 / 訓練ラベル
    └── val/               # Validation labels / 验证标注 / 検証ラベル
```

## Update Patch / 更新补丁 / アップデートパッチ

For EXE version: Download patch zip, extract to EXE folder to create `patch/` folder. Program auto-loads on startup.

EXE 版本：下载补丁 zip 解压到 EXE 同级目录，确保生成 `patch/` 文件夹。程序启动时自动加载。

EXE バージョン：パッチ zip をダウンロードし、EXE と同じフォルダに解凍して `patch/` フォルダを作成。プログラム起動時に自動読み込み。

## License / 许可 / ライセンス

MIT
