# Face-and-Sound-Recognition-System
Deep Learning - Digitan Signal and Image Management

E' stato sviluppato un sistema di riconoscimento vocale, di riconoscimento facciale e di image retrieval tramite l'utilizzo di algoritmi di Deep Learning.
Link diretto alle slide di presentazione del progetto: https://prezi.com/view/lyO6ZLI6zPc6pHvU10wN/

In questa repository sono presenti 4 tipologie di file, contrassegnati da:

SOUND: sono i codici relativi al task di processing di segnali monodimensionali (classificazione audio).
Più nello specifico:
			
	- '1_Audio_capturing.ipynb': acquisizione automatica di segnali audio tramite microfono del pc.
	- '2_Audio_augmenter.ipynb': augmentation (crop, noise, speed, tract) di segnali audio
	- '3.1_Audio_model_Monocanale.ipynb': feature extraction + modelli di classificazione (NNet e SVM con HPO-GridSearch)
	- '3.2_Audio_model_Bicanale.ipynb': estrazione dello spetrogramma + modello di classificazione (NNet)
		
		

IMAGE: sono i codici relativi al task di processing di segnali bidimensionali (classificazione volti).
Più nello specifico:

	- '1_capturing_images.ipynb': acquisizione automatica di foto tramite webcam.
	- '2_Face_Augmentation_Recognition.ipynb': augmentation delle immagini (brightness, flip) e face detection.
	- '3_Face_classification.ipynb': feature extraction (VGGface net) + face classification (SVM con HPO-GridSearch)
		
RETRIEVAL: è il codice relativo al task di image retrieval (estrazione dei 10 volti più simili).
			
	- '1_Retrieval': face detection + feature extraction (mobilenet) + costruzione dell'albero di ricerca.

DEMO_LIVE: è il codice per la dimostrazione live dei 3 task sovradescritti.
			
	- 'DemoLive_ImageSoundRetrieval.ipynb'
	
