# smart-physio

Here you can find the implementation of the Human Body Pose Estimation algorithm.

**Eldar Insafutdinov, Leonid Pishchulin, Bjoern Andres, Mykhaylo Andriluka and Bernt Schiele DeeperCut: A Deeper, Stronger, and Faster Multi-Person Pose Estimation Model. In European Conference on Computer Vision (ECCV), 2016**

**Eldar Insafutdinov, Mykhaylo Andriluka, Leonid Pishchulin, Siyu Tang, Evgeny Levinkov, Bjoern Andres and Bernt Schiele ArtTrack: Articulated Multi-person Tracking in the Wild. In Conference on Computer Vision and Pattern Recognition (CVPR), 2017**

For more information visit http://pose.mpi-inf.mpg.de

## SETUP

Python 3 is required to run this code. First of all, you should install TensorFlow as described in the official documentation. We recommended to use virtualenv.

You will also need to install the following Python packages:

```python
pip3 install scipy scikit-image matplotlib pyyaml easydict cython munkres
```

```python
# Download pre-trained model files
cd models/mpii
./download_models.sh
cd -
```

## RUNNING THE SMART PHYSIO APP

1. Move one known image of the person using the app to data/known_images/ folder.
2. Replace name_of_image.jpg with your image name and Person1 name with your name in PROFILES in physio.py file.
3. Run speak.py for audio output.
4. Run physio.py
5. Stand clear with full body in front of webcam so that the app could detect all your body parts.

## CITATION

```
@inproceedings{insafutdinov2017cvpr,
    title = {ArtTrack: Articulated Multi-person Tracking in the Wild},
    booktitle = {CVPR'17},
    url = {http://arxiv.org/abs/1612.01465},
    author = {Eldar Insafutdinov and Mykhaylo Andriluka and Leonid Pishchulin and Siyu Tang and Evgeny Levinkov and Bjoern Andres and Bernt Schiele}
}

@article{insafutdinov2016eccv,
    title = {DeeperCut: A Deeper, Stronger, and Faster Multi-Person Pose Estimation Model},
    booktitle = {ECCV'16},
    url = {http://arxiv.org/abs/1605.03170},
    author = {Eldar Insafutdinov and Leonid Pishchulin and Bjoern Andres and Mykhaylo Andriluka and Bernt Schiele}
}
```
