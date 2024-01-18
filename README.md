# unrolled_piano_sightreading_score
Annotated unrolled piano sight-reading score data for Music Information Retreival(MIR) tasks, including Score Following and Optical Music Recognition(OMR) 

This dataset contains typed unrolled piano sight-reading excerpts that contains audio and score representations annotated and aligned at high precision. It can be used for MIR cross modality training and evalutation tasks.

The following dataset is inspired by the MSMD dataset created by Matthias Dorfer and Jan Hajič jr.
MSMD Dataset: 
- https://github.com/CPJKU/msmd?tab=readme-ov-file

Feel free to contact author for any questions and enquries:
alexchuk@gmail.com


## Aligned sheet music and audio (spectrogram) aligned with MIDI and image coordinates
<img width="731" alt="image" src="https://github.com/chukalexander/unrolled_piano_sightreading_score/assets/117527004/34e5a5dc-ed83-4833-b2cb-055aafe41847">

![image](https://github.com/chukalexander/unrolled_piano_sightreading_score/assets/117527004/82e3e043-1830-4bf2-831f-d305dd1d2707)

Sources:
- Christian Schäfer - Sight reading Exercises for the Pianoforte (1-50)
- Hermann Berens Piano Pieces for First Beginners (51-100)
- #101 sample test piece

Structure of files

data/
  - 001/
     - annotation/
         - bar.npy (xy coordinates of barlines on img.png)
         - notes.npy (xy coordinates of notehead on img.png)
         - sys.npy (xy coordinates of the system on img.png)
     - 001img.png (image of score)
     - 001spec.png (spectrogram from .mp3)
     - 001d_spec.png (one step difference spectrogtram from .mp3)
     - 001.mp3 (synthesized audio)
     - 001mid.mid 
 - 002/
 - ...


Notes:
- only notehead included, expresssion markings omitted
