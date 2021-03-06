---
title: Stepper React component
components: MobileStepper, Step, StepButton, StepConnector, StepContent, StepIcon, StepLabel, Stepper
---

# Steppers

<p class="description">ステッパーは、番号の付いたステップを通して進捗を伝えます。 ウィザードのようなワークフローを提供します。</p>

[Steppers](https://material.io/archive/guidelines/components/steppers.html)は、一連の論理ステップと番号付きステップの進行状況を表示します。 ナビゲーションにも使用できます。 ステッパーは、ステップが保存された後に一時的なフィードバックメッセージを表示する場合があります。

- **ステップのタイプ**： Editable, Non-editable, Mobile, Optional
- **ステッパーのタイプ**：Horizontal, Vertical, Linear, Non-linear

> **注：** ステッパーは [Material Design guidelines](https://material.io/)には文書化されなくなりましたが、Material-UIは引き続きそれらをサポートします。

## Horizontal Stepper

### Linear

`Stepper` は、現在のステップインデックス（ゼロベース）を `activeStep` プロパティとして渡すことで制御できます。` <code>Stepper`方向は、 `orientation`プロパティを使用して設定されます。

この例では、 `optional`プロパティを第2の`Step`コンポーネントに配置して、オプションの手順を使用する方法も示します。 オプションの手順がスキップされる場合の管理はユーザー次第です。 特定のステップでこれを決定したら、`completed={false}` を設定して、アクティブなステップインデックスがオプションのステップを超えていても、実際には完了していないことを示す必要があります。

{{"demo": "pages/components/steppers/HorizontalLinearStepper.js"}}

### Linear - Alternative Label

`alternativeLabel`コンポーネントで`alternativeLabel` propを設定すると、ステップアイコンの下にラベルを配置できます。

{{"demo": "pages/components/steppers/HorizontalLinearAlternativeLabelStepper.js"}}

### Customized Stepper

コンポーネントのカスタマイズ例を次に示します。 詳細については、 [overrides documentation page](/customization/components/)を参照してください。

{{"demo": "pages/components/steppers/CustomizedSteppers.js"}}

### Non-linear

Non-linearステッパーにより、ユーザーはいつでもマルチステップフローを入力できます。

この例は、ステップが `activeStep` プロパティに基づいて `disabled ={true}` 自動的に設定されることを除いて、通常の水平ステッパーに似ています。

ここでは、</code>StepButton</code>を使用して、クリック可能なステップラベルと、`completed`の設定を示します。 しかし、ステップはノンリニアな方法でアクセスできるので、それはあなた自身の実装次第です。 すべての手順が完了したことを確認します(完成させる必要があっても)。

{{"demo": "pages/components/steppers/HorizontalNonLinearStepper.js"}}

### Non Linear - Alternative Label

`Stepper`コンポーネントで`alternativeLabel`propを 設定すると、ステップアイコンの下にラベルを配置できます。

{{"demo": "pages/components/steppers/HorizontalNonLinearAlternativeLabelStepper.js"}}

### Non Linear - Error Step

{{"demo": "pages/components/steppers/HorizontalNonLinearStepperWithError.js"}}

## 垂直ステッパー

{{"demo": "pages/components/steppers/VerticalLinearStepper.js"}}

## モバイルステッパー

このコンポーネントは、モバイルデバイスに適したコンパクトなステッパーを実装します。 その着想については、[mobile steps](https://material.io/archive/guidelines/components/steppers.html#steppers-types-of-steps)を参照してください。

### テキスト

これは基本的に、正しく配置された戻る/次へボタンです。 テキストの説明は自分で実装する必要がありますが、参考のために例を以下に示します。

{{"demo": "pages/components/steppers/VerticalLinearStepper.js"}}

### Text with Carousel effect

このデモは前のデモとよく似ていますが、 [react-swipeable-views](https://github.com/oliviertassinari/react-swipeable-views) ステップの遷移を行います。

{{"demo": "pages/components/steppers/SwipeableTextMobileStepper.js"}}

### Dots

ステップ数が多くない場合はドットを使用します。

{{"demo": "pages/components/steppers/DotsMobileStepper.js"}}

### Progress

Use a progress bar when there are many steps, or if there are steps that need to be inserted during the process (based on responses to earlier steps).

{{"demo": "pages/components/steppers/ProgressMobileStepper.js"}}