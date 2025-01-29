<h1 align="center">Automated Thoracic Disease Detection from Chest X-Rays Using Deep Learning</h1>

<h2>📌 Overview</h2>
<ul>
  <li>Developed a deep learning system to detect and classify 14 thoracic diseases (e.g., Pneumothorax, Cardiomegaly) and a "No Findings" class from chest X-ray images.</li>
  <li>Leveraged the NIH Chest X-ray Dataset (5,606 images) and trained three CNN architectures: VGG16-based models and EfficientNetB7.</li>
  <li>Achieved a test accuracy of <strong>65.07%</strong> using EfficientNetB7, demonstrating the potential of AI-assisted diagnostics in healthcare.</li>
</ul>

<h2>✨ Key Features</h2>
<ul>
  <li><strong>Data Preprocessing:</strong> Resized images to 224x224 pixels, normalized RGB values, and applied binary classification ("Finding" vs. "No Finding").</li>
  <li><strong>Data Augmentation:</strong> Enhanced robustness via random rotations (20°), shifts (20%), and horizontal flips.</li>
  <li><strong>Model Architectures:</strong>
    <ul>
      <li>Custom VGG16-based CNN with dropout and L2 regularization.</li>
      <li>EfficientNetB7 with Global Average Pooling and dense layers for optimized feature extraction.</li>
    </ul>
  </li>
  <li><strong>Training:</strong> Utilized Adam optimizer, binary cross-entropy loss, and callbacks (EarlyStopping, ModelCheckpoint).</li>
</ul>

<h2>📊 Dataset</h2>
<ul>
  <li><strong>Source:</strong> NIH Chest X-ray Dataset (5,606 images, 1024x1024 pixels).</li>
  <li><strong>Classes:</strong> 14 diseases + "No Findings" (e.g., Atelectasis: 508 images, Hernia: 13 images).</li>
  <li><strong>Imbalance Handling:</strong> Addressed class imbalance through stratified sampling and augmentation.</li>
  <li><strong>Download Links:</strong>
    <ul>
      <li><a href="https://www.kaggle.com/datasets/nih-chest-xrays/sample">Sample Dataset (Used in Project)</a></li>
      <li><a href="https://www.kaggle.com/datasets/nih-chest-xrays/data">Full NIH Chest X-ray Dataset</a></li>
    </ul>
  </li>
</ul>

<h2>🧠 Models and Results</h2>
<ul>
  <li><strong>Model 1 (VGG16-based CNN):</strong> 56.11% test accuracy.</li>
  <li><strong>Model 2 (Modified VGG16):</strong> 56.11% test accuracy with fine-tuning.</li>
  <li><strong>Model 3 (EfficientNetB7):</strong> 65.07% test accuracy, outperforming others due to advanced architecture.</li>
</ul>

<h2>📝 Conclusion</h2>
<ul>
  <li>Demonstrated the feasibility of deep learning for automated thoracic disease detection, with EfficientNetB7 as the top performer.</li>
  <li>Future improvements: Address class imbalance, test on larger datasets, and integrate clinical metadata for higher accuracy.</li>
  <li>Potential to reduce radiologists' workload and improve early diagnosis in resource-limited settings.</li>
</ul>

<h2>🔗 References</h2>
<ul>
  <li><a href="https://arxiv.org/abs/1705.09435">Deep Learning for Lung Cancer Detection</a></li>
  <li><a href="https://www.who.int/news-room/fact-sheets/detail/chronic-obstructive-pulmonary-disease">WHO COPD Report</a></li>
</ul>

<h3 align="center">🌟 Contributions welcome! Open an issue or PR for suggestions.</h3>
