# Deep Learning Prediction Quest (v10.1)

**Deep Learning Prediction Quest** is an interactive, browser-based educational game created to help students in the **Deep Learning** module familiarise themselves with essential terminology, Python/Keras syntax, and end-to-end machine learning workflows.

## Learning Objectives

By completing this game, students will be able to:

* **Recognise Core Terminology**: Distinguish genuine Deep Learning, Keras, Scikit-Learn, and Pandas terms (e.g., `EarlyStopping`, `fit_transform`, `StandardScaler`, `sparse_categorical_crossentropy`) from plausible impostors.
* **Sequence the Deep Learning Pipeline**: Order the 7 standard stages of a predictive modelling workflow—from framing the problem and cleaning data to evaluation and deployment on unseen data.
* **Match Tasks to Architectures & Losses**: Select the correct output layer activation and loss function for **Regression**, **Binary Classification**, and **Multiclass Classification** problems.
* **Recall Essential Python & Keras Syntax**: Complete common code patterns for data inspection, leakage-free splitting and scaling, building dense neural networks, applying regularisation, and saving/reloading models.
* **Identify and Prevent Common Pitfalls**: Spot and resolve real-world pipeline issues such as **data leakage** and **overfitting**.

## How to Play

### 1. Launch the Game
* Open `deep_learning_prediction_quest_v10_1.html` in any modern desktop or mobile web browser (Chrome, Edge, Firefox, or Safari). No installation or internet connection is required.

### 2. Complete the Pre-Check: Keyword Rain
* Falling cards will appear on screen containing either **real Deep Learning/Python keywords** or **impostors**.
* **Click or tap** only the real keywords (`+1` point). Clicking an impostor subtracts `1` point.
* Reach **50 / 50** to unlock Stage 0. You can toggle the audio on or off at any time using the **Sound** button in the top-right corner.

### 3. Clear Stage 0: Arrange the Pipeline
* **Drag and drop** the 7 pipeline cards into the correct chronological order (on touchscreens or keyboards, use the **↑** and **↓** buttons).
* Click **Check Pipeline** to verify your sequence. Clearing Stage 0 unlocks your randomly assigned mission and awards starting XP and Credits.

### 4. Progress Through Stages 1–7
* At Stage 1, you will receive a **Random Mission** (*Regression*, *Binary Classification*, or *Multiclass Classification*) that tailors certain questions to that specific task.
* Complete each stage's **multiple-choice questions** and **fill-in-the-blank code puzzles**, then click **Check Stage**.
* Answering correctly on your first try builds a **Streak (🔥)** for up to a `2×` XP multiplier and earns **Credits (🪙)**.
* **Need help?** Spend your earned Credits on:
  * **Hint (5 🪙)**: Displays a conceptual clue.
  * **First + Last Letter (10 🪙)**: Reveals the first and last characters of each missing code blank.
  * *(Note: Purchasing a clue resets your current streak.)*

### 5. Resolve Random Incidents & Defeat the Boss
* Between stages, you will encounter **Random Incidents** (such as spotting a line of code causing test-set leakage) and a **Stage Boss (*The Overfitter*)** where you must interpret training vs. validation loss logs and choose the right countermeasures.

### 6. Review Your Results & Replay
* After completing Stage 7, review your final **Rank**, **XP**, **First-Try Rate**, and unlocked **Achievement Badges** (*Pipeline Master*, *Zero Assistance*, *Streak Specialist*, *Overfitter Slayer*).
* Click **New Random Mission** (or refresh the page) to practise again with a different prediction scenario.

## Curriculum Overview

1. **Pre-Check — Keyword Rain**: Rapid-fire vocabulary recognition (Keras, Scikit-Learn, Pandas).
2. **Stage 0 — Pipeline Ordering**: Sequencing the 7-step Deep Learning workflow.
3. **Stage 1 — Frame the Mission**: Model family selection, output activations (`linear`, `sigmoid`, `softmax`), and loss functions.
4. **Stage 2 — Inspect & Clean**: `read_csv`, `shape`, `isna`, `dropna`, `drop_duplicates`, `reset_index`.
5. **Stage 3 — Split Without Leakage**: Feature/target separation, `train_test_split`, and leakage-free `StandardScaler` (`fit_transform` vs. `transform`).
6. **Stage 4 — Build a Baseline**: Hidden `Dense` layers (`relu`) and `model.fit` (`epochs`, `batch_size`).
7. **Stage 5 — Optimise**: `Dropout`, `l2` regularisation, and `EarlyStopping`.
8. **Stage 6 — Evaluate**: Validation vs. test set discipline, `model.predict`, and task-specific metrics/thresholds.
9. **Stage 7 — Deploy & Infer**: Saving models (`model.save`) and reloading scalers (`joblib.load`) to predict on unseen data.

## Technical Details

* **Self-Contained Single File**: Built with vanilla HTML5, CSS3, and JavaScript (ES6+) with zero external dependencies.
* **Synthesized Audio**: Uses the browser's Web Audio API for interactive feedback during Keyword Rain.
* **Responsive & Accessible**: Supports desktop and mobile screens, including button-based sorting controls in Stage 0.