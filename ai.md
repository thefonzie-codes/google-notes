# AI and Machine Learning

- **Supervised Models**: Data is labelled with a tag, number, name or similar
        - Unsupervised models look at raw data and seeing if it falls into groups naturally


                    ----------------------------
                   |                            |
                   V                            |
        Input -> Model -> Predicted Output -> Error
                                |               ^
                                | **compare**   |
                                V               |
                          Expected Output -------


- **Unsupervised Models**: No tags
        - Supervised uses past examples to predict future values

        Input -> Model -> Generated Example

- **AI Models**
    - y: output = f:function(x: input)
    - Discrimitative - Label ex. Number, Class, Probablility - predictive?
    - Generative - NEW CONTENT - ex. images, text, video - "creates"
        - Generative LANGUAGE models -  TEXT to image, audio, text or other format
        - Transformers - encoder and decoder
            - Encoder takes x and decoder outputs x based on task

## Google's AI products:

- **Vertex AI**: create your own chatbots, didital assistands, training apps etc
- **Gemini**: complex AI tasks

## Data Quality Metrics

- **Relevance**
- **Completeness**
- **Accuracy**
- **Representation**
- **Consistency**

## Data Accessibility

- Availability
- Cost
- Format

## Data Types/Categorizations

- Structured : Think Rows and Columns
- Unstructured : Think documents/free form text, images, music.

- Labeled
    - Has a type, name or number.  Basically is "tagged" or categorized
- Unlabeled
    - Raw, unprocessed info with no meaning, eg. Audio logs, text with no categorization
    - Algorithms built to discover the patterns as there are no labels. 

## Machine Learning

- **Supervised Learning**:
    - Trains on labeled data where input is paired with correct output
    - Identify patterns and relationships with labeled data
        - eg. Predicting housing prices
- **Unsupervised Learning**:
    - Raw, unlabeled data to find natural groupings.
    - Targeted marketing or product recommendations. Think exploratory analysis.
- **Reinforcement Learning**:
    - Learning through interaction and feedback
    - Reward "good" behaviour and discourage "bad" behaviour.
    - The algorithm maximizes rewards and minimizes penalties by interacting with the environment.
    - Most useful when you can't provide explicit instructions or labeled data.
        - Eg. Train self driving car to navigate trafffic situations
    - Think trial and error

    ### Some use cases
    - **Predictive Maintenance** with VertexAI (Supervised Learning)
        - Training a model on sensor data from machines like temperature, pressure, vibration to detect failure before it happens.
    - **Anomaly Detection** with BigQuery ML (unsupervised learning)

- **Deep Learning** - subset of ML, differentiated by usage of artificial neural netoworks. Both labelled and unlabelled data - supervised learning.

## Foundation Models

- Complex Patterns
- Variety of tasks across multiple domains

Examples:

- **LLMs**
    - Designed to understand and generate human language
- **Diffusion Models**
    - Images, audio and video by refining noise or unsturcured/random data and patterns into structured data

**Considerations when choosing a model**

- Modality
    - What kind of info is being processed, what you want as imput and output
- Context
    - Amount of info being processed/a model can remember/consider at one time
- Security
- Availability and reliability
- Cost
- Performance
- Fine tuning and customization
- Ease of integration

## Google Cloud's ML Models

- **Gemini**
    - Multimodal - text, video, audtio
- **Gemma**
    - Lightweight, open models based on gemini tech
- **Imagen**
    - Text to image
- **Gemini**
    - Text/images to Video content

## Limitations

- Data Dependency
- Date cutoff
- Bias
- Fairness
- Hallucinations
- Edge Cases

**Overcoming limitations**
    - Grounding - connecting to verifiable sources
    - RAG
    - Prompt engineering
    - Fine tuning

**Humans in the loop** (HITL)
    - Content moderation
        - Filtering harmful or appropriate material
    - Sensitive applications
        - Accuracy and risk mitigation in fields like finance or healthcare
    - High-risk decision making
        - Safeguard for decisions such as medical diagnoses or justice assessments
    - Pre-generation review
        - Review or validate outputs pre-deployment
    - Post-generation review
        - Review post-deployment

## Security and Responsibility

- Applying the SAIF - Safe AI Framework
- Cloud Security tools

- **Transparency**
- **Privacy**
- **Data Quality, Bias and Fairness**
- **Accountability and Explainability**
