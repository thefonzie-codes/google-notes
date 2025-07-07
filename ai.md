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

## Layers of GenAI

- Infrastructure
- Agents
- Platform
- Models
- AI Powered Application

### Agents

Agents allow you to personalize and specialize models for tasks

Multiple agents, different specializations in one application. AKA Multi-agent system

eg. **Travel Booking app**

                           **AGENTS**

    Recommend flights and hotels ----
                                      \
                                       \
    Relevant activities ------------------- Info presented in interface
                                       /
                                      /
    Activities and attractions ------

#### Types of Agents

    - Conversational
    - Workflow

**Tools**

- Tools allow AI to interact with the environment
    - For example, automatically order new stock when store is low

### Platform Layer

- Provides the solution to build and scale AI initiatives

#### Vertex AI

- Infrastructure 
- Pre-trained models
- Tools
- Easy Integration
- Customization
- Open and Flexible

- ML Ops Tools
    - End to end workflows
    - Feature store
    - Model Registry
    - Model Evaluation
    - Workflow Orchestration
    - Model Monitoring

- AI Model
    - Brain of the operation
    - **Vertex AI: Model Hub**
        - Model Garden
        - First-party foundation models
        - First-party pre-trained API's
        - Open models
        - Third party models

- Build Models with Vertex AI
    - AutoML OR custom frameworks like PyTorch, TensorFlow, scikit-learn, or XGBoost
    - AutoML
        - Image Data
        - Video Data
        - Text Data
        - Tabular Data

<p style="color:green">
**Gather Data -> Prepare -> Train -> Manage -> Deploy**
<p>

### Foundations of GenAI solutions
    
    - high performance computing
    - GPU's and TPU's
        - Built for parallel processing
        - TPU's are specifically Google designed for AI
    - Hypercomputer
        - Connected individual computers (nodes)
        - Connected as a single unit
        - Have GPU's and TPU's to maximize parallel processing
    - Large-scale storage
        - High throughput, scalability and dense clusters
    - Fast storage
        - Quick read and write speeds for faster training
    - Networking
        - High bandwidth and low latency

### Edge Computing
    - PriUvacy
    - Speed
    - Offline Access

    - Works well for smaller tasks

### Project Resources
    - People
        - Devs
        - Execs
        - AI Practitioners
    - Cost
        - Train
        - Deploy
        - Use

        - Pricing models
            - Usage
            - License
            - Subscription
            - Free
        - Pricing Metrics for using models (How they charge, if by use)
            - Tokens
            - Characters
            - Requests
            - Compute time
        - Factors that affect cost
            - Model size and complexity
            - Context window
            - Features
            - Deployment
    - Time

### Solution Needs
    - Scale
    - Customization
        - Start with existing models
        - Identify needs
        - Consider data specificity aka domains like law or medicine
        - Task complexity
    - UI/UX
    - Privacy
        - Data Security
        - Compliance
    - Others
        - How specialized?
        - Latency
        - Connectivity
        - Accuracy
        - Explainability
    - Maintenance
        - Model monitoring and retraining
        - Data updates
        - Software updates and bug fixes
        - Hardware and infra
        - Security and compliance
