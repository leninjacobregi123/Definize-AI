# Definize

**Definize** is a next-generation, AI-powered vocabulary assistant designed to help readers, researchers, and learners not only understand unfamiliar words but also retain and master them over time.

It combines state-of-the-art language models, intelligent contextualization, and personalized learning tools into a seamless browser-based experience.

> Select a word. Understand its meaning in context. Save it. Master it.


## Features

* **Context-Aware Definitions**
  Powered by AI, Definize delivers definitions that adapt to the context and domain of the text being read, avoiding generic or irrelevant explanations.

* **Personal Vocabulary Bank**
  Every word looked up is saved to a secure, personal word bank for later review.

* **Learning and Retention Tools**
  Includes flashcards, spaced repetition quizzes, and gamified progress tracking to reinforce learning and retention.

* **Domain-Specific Modes**
  Tailor definitions for specific domains such as Academic, Legal, Medical, and Literary, ensuring relevance and precision.

* **Simplified Explanations**
  Optional "Explain Like I’m Five" mode for simplified explanations, ideal for non-native speakers and early learners.

* **Pronunciation Support**
  Provides correct pronunciation in multiple accents, with the option to practice and receive feedback on recorded pronunciation.

* **Vocabulary Analytics**
  Visual dashboard to monitor vocabulary growth, identify weak areas, and track learning progress over time.

* **Cross-Device Synchronization**
  Word bank and progress are securely synchronized across all devices.

---

## Why Definize

Traditional tools stop at providing dictionary definitions, leaving the burden of learning and remembering entirely on the user.
Definize is designed to actively assist in understanding, memorization, and mastery, using adaptive AI and pedagogical principles, while respecting user context and intent.

---

## Installation

### For End Users

#### Chrome / Edge

1. Download the latest release archive from the [Releases](https://github.com/your-org/definize/releases) page.
2. Unzip the archive to a folder.
3. Open `chrome://extensions/` in your browser.
4. Enable *Developer mode*.
5. Select *Load unpacked* and choose the unzipped folder.
6. Pin the Definize icon to your browser toolbar for easy access.

#### Firefox

1. Open `about:debugging#/runtime/this-firefox`.
2. Click *Load Temporary Add-on*.
3. Select `manifest.json` from the unzipped folder.

---

## Developer Setup

Clone the repository and install dependencies:

```
git clone https://github.com/your-org/definize.git
cd definize
npm install
npm run build
```

To start the backend API service:

```
cd server
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
uvicorn app:app --reload
```

---

## Project Structure

```
definize/
├── src/
│   ├── background.js
│   ├── content.js
│   ├── popup/
│   │   ├── popup.html
│   │   ├── popup.js
│   │   └── popup.css
│   ├── dashboard/
│   │   ├── index.html
│   │   ├── dashboard.js
│   │   └── dashboard.css
├── server/
│   ├── app.py
│   └── requirements.txt
├── manifest.json
├── package.json
├── README.md
└── LICENSE
```

---

## Architecture Overview

* **Frontend**:
  A browser extension built on the WebExtensions API (Manifest V3) with a React-based popup and dashboard.
  Includes content scripts for intercepting user selections.

* **Backend**:
  A RESTful API service (FastAPI or Flask) providing AI-based definitions, user account management, and synchronization.
  Integrates with LLMs (e.g., GPT-based models) and cloud storage for user data.

---

## Roadmap

| Phase                  | Description                                           |
| ---------------------- | ----------------------------------------------------- |
| Minimum Viable Product | Select word and show AI-powered contextual definition |
| Word Bank              | Persist looked-up words in a user-specific list       |
| Learning Tools         | Implement flashcards, spaced repetition quizzes       |
| Domain Modes           | Enable domain-specific definition tuning              |
| Analytics Dashboard    | Display vocabulary trends and progress                |
| Cross-Device Sync      | Synchronize user data across devices                  |

---

## Testing

Run frontend and backend tests:

```
npm test
pytest
```

Test coverage reports and CI pipeline configurations are provided in the repository.

---

## Contributing

We welcome contributions under the guidelines outlined in [CONTRIBUTING.md](CONTRIBUTING.md).

To contribute:

* Fork this repository.
* Create a new branch for your feature or bugfix.
* Commit your changes with clear and descriptive messages.
* Submit a pull request against the `main` branch.

By contributing, you agree to abide by the [Code of Conduct](CODE_OF_CONDUCT.md).

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Maintainers

* [Your Name](mailto:your.email@example.com) — Lead Developer
* [Your Organization](https://your-organization.example.com)

For support or business inquiries, please contact [support@definize.com](mailto:support@definize.com).

---

## Vision

Definize aspires to redefine how people interact with language while reading.
It empowers readers to deepen their understanding, retain their learning, and expand their vocabulary, seamlessly integrated into their daily reading experience.

---

## Documentation and Additional Resources

* Product Requirements Document: `docs/PRD.md`
* API Specification: `docs/API_SPEC.md`
* Test Plan: `docs/TEST_PLAN.md`
* Brand Guidelines and Assets: `docs/BRAND.md`

For further information, visit the [project website](https://definize.example.com) or the [GitHub repository](https://github.com/your-org/definize).

---

