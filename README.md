# AR-Enabled Diwali Greeting Cards

This academic project explores how augmented reality could make a traditional Diwali greeting card more interactive by connecting a printed or digital card with a digital experience.

I have kept this repository focused on the material that is currently available. At the moment, it contains the project report and this README; it does not contain a complete Unity project that someone can open and run.

## Project idea

A greeting card is usually a printed design or a flat image. The idea behind this project is to make the greeting more engaging with an augmented-reality experience.

The project goals are to:

- Explore an AR-based Diwali greeting experience.
- Present festive visual content in a more interactive way.
- Consider audio feedback as part of the experience.
- Document the idea and the development approach.

## Technology notes

The existing documentation refers to Unity's C# APIs, including `MonoBehaviour`, `AudioSource` and `AudioClip`.

| Area | What is currently documented |
|---|---|
| Programming language | C# |
| Development environment | Unity APIs are referenced |
| AR SDK or tracking method | Not specified in the uploaded files |
| Target device | Not specified in the uploaded files |

I have not listed an AR SDK or Unity version because those details are not confirmed by the repository files.

## Example: playing a greeting sound in Unity

The following is a small reference example for playing an assigned audio clip. It is included as documentation; it is not represented as an existing source file in this repository.

```csharp
using UnityEngine;

public class SoundManager : MonoBehaviour
{
    [SerializeField] private AudioSource audioSource;
    [SerializeField] private AudioClip greetingClip;

    public void PlayGreeting()
    {
        if (audioSource == null || greetingClip == null)
        {
            Debug.LogWarning("Please assign the AudioSource and greeting clip.");
            return;
        }

        audioSource.PlayOneShot(greetingClip);
    }

    public void StopGreeting()
    {
        if (audioSource != null)
        {
            audioSource.Stop();
        }
    }
}
```

## Repository contents

- `AR Enabled greeting cards Report.docx` — the project report.
- `README.md` — project overview and current repository notes.
- `.gitignore` — excludes common generated files.

## How to review the current upload

1. Open the Word report and review the project description and details included there.
2. Use this README as a guide to the current repository scope.
3. The application cannot be built from this repository yet because the Unity scenes, scripts, assets and project settings are not included.

## Next steps for a complete project repository

When the original project files are available, I would like to add:

- The Unity project, including `Assets`, `Packages` and `ProjectSettings`.
- The actual AR tracking or image-target setup used.
- Screenshots of the application running on a device.
- A short demo video.
- The Unity version, device requirements and build instructions.

Only the files used by the actual project should be added. Unity-generated folders such as `Library/`, `Temp/` and `Obj/` should stay out of Git.

## About

This is an academic project documented by **Venkata Kishore Seelam**.

[GitHub profile](https://github.com/Venkatakishore125)

---

**Repository status:** The report and documentation are available. A runnable Unity implementation has not been uploaded here yet.
