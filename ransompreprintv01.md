RANSOM: Toward an Open Corpus of Emotional Configurations for Artificial Intelligence
Augustin Sénégou
Novia Technologies / Independent Research
augustinmichelrobert@gmail.com
Preprint — submitted to OSF MetaArXiv
Version 0.1 — 2026-04-16

Abstract
Current approaches to affective computing rely on emotional datasets built from labelled utterances, acted recordings, and flat categorical taxonomies. We argue that these datasets are structurally insufficient — not because they are too small, but because they misrepresent the nature of human emotion as a temporal, relational, and inherently ambiguous phenomenon. We propose RANSOM (Recognizing Affect through Narrative, Semantics, and Observable Markers), an open research foundation built on a different hypothesis: that human cultural production — cinema, literature, theatre — constitutes the largest existing archive of intentionally documented emotional complexity, annotated implicitly by expert human observers across more than a century of production. This paper defines the theoretical foundations of the RANSOM taxonomy, proposes an annotation methodology for extracting emotional configurations from cultural sources, and argues for an open corpus model on both epistemic and ethical grounds.

1. Introduction
The problem of emotional recognition in artificial intelligence is widely understood as a data problem. Systems lack sufficient labeled examples of human emotional states to generalize reliably across real-world contexts.
We argue this framing is incorrect.
The problem is not a quantity problem. It is a structural problem. Existing emotional datasets encode a model of emotion that is categorically wrong — and adding more data of the same kind will not produce better recognition. It will produce more confident misrecognition.
The dominant model treats emotion as a discrete state: a sentence, a face, or a voice clip belongs to one of N categories — joy, sadness, anger, fear, disgust, surprise. This model derives from Paul Ekman's basic emotion theory (Ekman, 1992), which, despite substantial empirical criticism (Barrett, 2017; Russell, 1980), continues to dominate dataset construction in affective computing.
The problems with this model are well-documented in the psychological literature but have not yet been operationalized as dataset design principles:
Emotions are temporal. They unfold, intensify, plateau, transform, and resolve — or are suppressed. A single-frame annotation captures a cross-section of a process, not the process itself.
Emotions are relational. The same internal state manifests differently depending on the relationship between speaker and listener. Grief in front of a close friend, a stranger, and a superior are behaviorally distinct configurations of the same underlying state.
Emotions are contradictory. Mixed states — shame masking as arrogance, fear expressing as anger, desire presenting as indifference — are not annotation errors. They are the normative condition of adult emotional experience in social contexts.
Emotions are culturally inflected. The behavioral markers of an emotional configuration vary across cultures in ways that existing predominantly anglophone datasets systematically fail to capture.
Ambiguity is a valid state. The condition in which a person does not know what they are feeling, or in which outside observers cannot reliably distinguish between two possible states, is not a failure of annotation. It is a real emotional phenomenon that recognition systems must be able to represent.
No existing large-scale emotional dataset adequately addresses these five properties. RANSOM is a proposal to build one that does.

2. The Cultural Archive Hypothesis
We propose that the largest existing archive of adequately complex emotional documentation is human cultural production — specifically narrative fiction in the form of literature, cinema, and theatre.
This claim requires justification.
2.1 Art as intentional emotional documentation
Works of narrative fiction are, among other things, systematic attempts to render human emotional experience legible to outside observers. A novelist constructing a character in grief is solving the same problem an affective computing researcher faces: how do you make an internal state visible through observable behavior?
The novelist's solution — accumulated over centuries of literary tradition — is to show emotion as configuration: a pattern of behaviors, language choices, perceptual distortions, relational shifts, and temporal dynamics that constitute a recognizable whole.
This solution has been validated by a unique feedback mechanism: reader recognition. A novelist whose emotional configurations are not recognized as true does not find readers. The corpus of enduring narrative fiction has been filtered, across centuries and across cultures, by the criterion of emotional truth.
2.2 Expert annotation at scale
A film directed by Ingmar Bergman contains emotional configurations that have been processed by multiple expert observers before reaching the screen: the screenwriter who constructed the emotional arc, the director who shaped its expression, the actor who embodied it, the editor who determined its temporal presentation, and the critical tradition that has analyzed its components.
This is not equivalent to crowdsourced annotation. It is expert annotation — distributed, iterative, and validated against the standard of human recognition across decades of reception.
2.3 The diversity of the archive
The cultural archive spans centuries, cultures, and traditions. Japanese cinema encodes emotional configurations that differ substantially from French cinema. West African oral narrative tradition encodes configurations absent from European literary tradition. This diversity, properly sampled, offers something no existing dataset provides: a genuinely cross-cultural library of emotional expression.

3. The RANSOM Taxonomy
3.1 Design principles
The RANSOM taxonomy is built on four principles that distinguish it from existing categorical approaches:
Configurations, not categories. A RANSOM unit is not an emotion label but an emotional configuration — a structured description of observable markers across linguistic, prosodic, behavioral, and relational dimensions.
Temporal extension. Each configuration is described as a process with phases: onset markers, development patterns, resolution or suppression trajectories.
Masking relationships. Each configuration includes documentation of common masking states — the emotional presentations that typically overlay it in social contexts.
Cultural specificity flags. Each configuration is tagged for its degree of cross-cultural stability versus cultural specificity, based on evidence from the annotation process.
3.2 Configuration structure
Each entry in the RANSOM taxonomy has the following structure:
CONFIGURATION ID: [unique identifier]
WORKING NAME: [descriptive label, not a categorical emotion name]
DEFINITION: [phenomenological description of the state]

ONSET MARKERS:
  - Linguistic: [characteristic language patterns]
  - Prosodic: [characteristic vocal patterns]
  - Behavioral: [characteristic non-verbal patterns]
  - Relational: [characteristic interpersonal patterns]

DEVELOPMENT PATTERN: [how the configuration typically evolves]

COMMON MASKING STATES: [what this configuration typically presents as]

RESOLUTION TRAJECTORIES: [how this configuration typically ends]

AMBIGUITY ZONE: [configurations commonly confused with this one, and distinguishing markers]

CULTURAL STABILITY: [high / medium / low, with notes]

REFERENCE INSTANCES: [annotated examples from the cultural corpus]
3.3 Sample configuration
CONFIGURATION ID: RANSOM-007
WORKING NAME: Suppressed grief presenting as controlled efficiency
DEFINITION: A state of acute loss in which the subject maintains 
  functional performance while actively preventing emotional expression, 
  producing a characteristic pattern of hyper-competence combined with 
  micro-interruptions of affect.

ONSET MARKERS:
  Linguistic: shortened sentences, increased precision of word choice, 
    avoidance of evaluative language, unusual formality in casual contexts
  Prosodic: slightly elevated pitch baseline, controlled breath patterns 
    with occasional arrested exhalation, reduced prosodic variation
  Behavioral: increased physical stillness, brief gaze aversions at 
    semantically significant moments, micro-expressions of pain at 
    references to the loss domain
  Relational: increased task-orientation, reduced social initiative, 
    discomfort with expressions of sympathy

DEVELOPMENT PATTERN: Onset is typically rapid following triggering event. 
  Maintenance requires increasing cognitive load over time. Breaks 
  typically occur in private or in response to unexpected kindness.

COMMON MASKING STATES: Professional composure, stoicism, coldness, 
  disengagement, unusual productivity

RESOLUTION TRAJECTORIES: Gradual emergence of grief markers as 
  suppression cost increases; sudden collapse under emotional trigger; 
  displacement into somatic complaints

AMBIGUITY ZONE: Distinguishing from genuine disengagement: look for 
  micro-expressions at loss-domain references. Distinguishing from 
  professional coldness: look for prosodic breaks at unexpected kindness.

CULTURAL STABILITY: Medium — suppression pattern is cross-cultural; 
  specific behavioral markers vary by cultural display rules

REFERENCE INSTANCES: 
  - [Film reference 1 — scene description]
  - [Literary reference 1 — passage description]

4. Annotation Methodology
4.1 Annotator profiles
RANSOM annotation requires human experts whose training gives them access to emotional configurations that are invisible to untrained observers.
We identify four annotator profiles:
Clinical psychologists and psychotherapists — trained to observe emotional states beneath social presentation. Particularly valuable for masking configurations and ambiguity zones.
Trained actors and acting teachers — specifically those trained in methods that require embodied understanding of emotional states (Stanislavski, Meisner, Viewpoints). Particularly valuable for onset markers and temporal development.
Film directors and dramaturges — trained to construct and evaluate emotional configurations for recognizability and truth. Particularly valuable for reference instance selection.
Literary critics specializing in psychological realism — trained to articulate the structural components of emotional representation in narrative. Particularly valuable for taxonomy definition and linguistic markers.
4.2 Annotation process
Annotation proceeds in three phases:
Phase 1 — Configuration identification. Annotators review cultural source material and identify candidate configurations — moments or sequences in which a complex emotional state is clearly rendered. Each candidate is tagged with a working description and source reference.
Phase 2 — Marker extraction. For each confirmed configuration, annotators extract observable markers across all four dimensions (linguistic, prosodic, behavioral, relational). This phase requires multi-annotator consensus with structured disagreement resolution.
Phase 3 — Taxonomy integration. Extracted configurations are compared against existing taxonomy entries. New configurations are added; existing entries are enriched with new reference instances and marker variants.
4.3 Handling ambiguity
Ambiguity is not resolved by majority vote. When annotators cannot reach consensus on a configuration, the disagreement is itself annotated — recording the competing interpretations, the markers that support each, and the conditions under which one or the other would be more probable.
This produces a richer representation than false consensus. It teaches recognition systems that some emotional states are genuinely ambiguous — and what the distinguishing evidence would look like if it were available.

5. The Open Corpus Model
5.1 Epistemic argument
A closed corpus of emotional recognition encodes the decisions of a small group about what human emotion means — and propagates those decisions into systems that affect the entire population of users.
This is not a neutral technical choice. Emotional recognition systems trained on a closed corpus will systematically misread the emotional states of anyone whose emotional expression diverges from the corpus's implicit norms. Given the historical anglophone and Western bias of existing datasets, this means systematic misrecognition of non-Western emotional expression — encoded into infrastructure at scale.
An open corpus is not just ethically preferable. It is epistemically necessary. The diversity of human emotional expression cannot be adequately captured by any single institution. It requires the distributed contribution of experts across cultural traditions.
5.2 Ethical argument
C.S. Lewis, in The Abolition of Man (1943), described the condition of human beings who have lost the capacity to recognize objective emotional value — what he called men without chests. He warned that such people, armed with technique, become Conditioners: those who shape the emotional responses of others according to private will rather than shared human truth.
A closed corpus of emotional recognition — owned by a private entity, encoding a proprietary understanding of what human emotion means — is precisely this structure at technological scale.
RANSOM is built on the opposite principle: that the knowledge of how human beings feel belongs to humanity, and that any infrastructure built on it must be answerable to humanity.
5.3 Strategic argument
The history of technological infrastructure suggests that open foundations produce more robust and more widely adopted applications than closed ones. TCP/IP, Linux, and the World Wide Web became standards precisely because no single entity owned them — and the applications built on them generated value that proprietary alternatives could not match.
RANSOM is designed as infrastructure. The applications built on it — including Oria — are where value is captured. The foundation is where trust is built.

6. Relation to Oria
RANSOM is the open foundation underlying Oria, a professional conversation intelligence platform developed by Novia Technologies.
Oria applies emotional recognition to the specific context of professional B2B conversations — identifying decision patterns, commitment signals, risk indicators, and relational dynamics in recorded calls.
The RANSOM corpus is not proprietary to Oria. It is released under open license and may be used by any researcher or developer. Oria's competitive advantage lies in its application layer — the specific implementation, integration, and contextual calibration built on top of the foundation — not in control of the foundation itself.
This structure is deliberate. Novia Technologies believes that the quality of emotional recognition available to all AI systems is a matter of public concern — and that a company positioned as the steward of an open standard is more defensible, more trustworthy, and ultimately more valuable than one positioned as the owner of a closed secret.

7. Conclusion
The failure of AI systems to recognize human emotion is not a failure of architecture or processing capacity. It is a failure of data — specifically, a failure to provide systems with data that accurately represents the temporal, relational, contradictory, and ambiguous nature of human emotional experience.
RANSOM proposes to address this failure by building an open corpus derived from the richest existing archive of documented emotional complexity: human cultural production.
The foundation is open. The methodology is rigorous. The commitment is long-term.
We invite researchers, annotators, engineers, and cultural experts to contribute.

References
Barrett, L. F. (2017). How Emotions Are Made: The Secret Life of the Brain. Houghton Mifflin Harcourt.
Ekman, P. (1992). An argument for basic emotions. Cognition & Emotion, 6(3–4), 169–200.
Lewis, C. S. (1943). The Abolition of Man. Oxford University Press.
Russell, J. A. (1980). A circumplex model of affect. Journal of Personality and Social Psychology, 39(6), 1161–1178.
Tolkien, J. R. R. (1947). On fairy-stories. In Essays Presented to Charles Williams. Oxford University Press.

RANSOM project repository: github.com/[organisation]/ransom
Contact: [à compléter]
License: CC BY 4.0
