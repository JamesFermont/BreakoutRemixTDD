# Sounds

## Implementation

To implement a new sound, open the "AudioManager" prefab located in the folder "MyAssets/Prefabs/AudioManager". You will find a component attached to it called "AudioManager" with a "Sounds" public table.

1. Increase the "Size" value of the sounds array by 1
2. Scroll down to your newly created entry and change it's name
3. Drag the sound to be added into the AudioClip field
4. Define it's type (SFX or BGM), whether or not it should loop as well as its default volume and pitch.
5. Done!

## Use

### Methods

If your script needs to play a sound effect, reference the AudioManager game object. It is present in every scene so there is no need to create one.

    AudioManager.Play(string name);

Plays the Sound that matches this name.

    AudioManager.Stop(string name);

Stops playback of the Sound that matches this name.

    AudioManager.UpdatePitch(string name, float pitch);

Updates the pitch of the Sound that matches this name to this pitch. Note that pitch is clamped between 0.1f and 3f.

    AudioManager.UpdateVolumeOfType(SoundType type, float volume);

Updates the volume of all sounds that match this SoundType. Should only be used in the creation of the Options menu.
