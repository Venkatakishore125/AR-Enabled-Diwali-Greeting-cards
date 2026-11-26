# AR-Enabled Diwali Greeting Cards

An academic project focused on presenting Diwali greeting cards through an augmented-reality (AR) experience. The repository currently contains the project report and this documentation; the Unity project source, scenes, assets, and a runnable demo are not included yet.

## Project overview

Traditional greeting cards are usually viewed as printed or flat digital designs. This project explores an AR-based way to make Diwali greetings more interactive by connecting a greeting-card design with a digital experience.

> **Repository status:** Documentation and project report are available. The complete Unity implementation is not currently present in this repository, so the AR workflow and supported features cannot yet be independently verified from the files here.

## Project goals

- Explore how augmented reality can make greeting cards more engaging.
- Present a Diwali-themed greeting in a digital, interactive format.
- Explore audio feedback as part of the user experience.
- Document the project clearly so that it can be reviewed and reproduced when the source files are added.

## Technology

The existing README included a C# script using Unity's `MonoBehaviour`, `AudioSource`, and `AudioClip` APIs. This indicates a Unity/C# component was part of the project. The specific AR SDK, Unity version, target platform, and device requirements are not documented in the current repository.

| Area | Current evidence |
|---|---|
| Programming language | C# |
| Development environment | Unity APIs are referenced in the existing code snippet |
| AR framework | Not specified in the repository |
| Target platform | Not specified in the repository |

## Audio script reference

The original README contained a sound-manager example with a method declaration placed inside another method. The corrected reference below separates the methods and checks that the required audio references are assigned.

```csharp
using UnityEngine;

public class SoundManager : MonoBehaviour
{
    [SerializeField] private AudioSource audioSource;
    [SerializeField] private AudioClip audioClip;

    public void PlaySound()
    {
        if (audioSource == null || audioClip == null)
        {
            Debug.LogWarning("Assign an AudioSource and AudioClip in the Inspector.");
            return;
        }

        audioSource.PlayOneShot(audioClip);
    }

    public void StopSound()
    {
        if (audioSource != null)
        {
            audioSource.Stop();
        }
    }
}
```

This is a documentation example, not a claim that the script is currently included in the repository. Add it as a Unity C# file under `Assets/Scripts/` if it matches the implementation you want to use.

## Repository contents

- `AR Enabled greeting cards Report.docx` — project report.
- `README.md` — project overview and documentation.

The Unity source code, scenes, AR image targets, greeting-card assets, audio files, screenshots, and demo video are not currently visible in this repository.

## How to review the project

1. Open and read the project report linked in the repository.
2. Review the project goals and implementation details described in the report.
3. When the original Unity project is available, add the source files and the exact setup steps here.
4. Capture screenshots or a short demo video of the working application and add them to a `Screenshots/` or `Demo/` folder.

There are no verified build or run instructions yet because the Unity project files and configuration are not included.

## Suggested repository structure

When the original project files are available, consider organising them like this:

```text
AR-Enabled-Diwali-Greeting-cards/
├── Assets/
│   ├── Scenes/
│   ├── Scripts/
│   ├── Images/
│   ├── Audio/
│   └── Prefabs/
├── ProjectSettings/
├── Packages/
├── Documentation/
│   └── AR-Enabled-Greeting-Cards-Report.docx
├── Screenshots/
├── Demo/
├── .gitignore
└── README.md
```

Only add folders and files that belong to the actual project. Avoid uploading generated Unity folders such as `Library/`, `Temp/`, and `Obj/`.

## Future improvements

- Add the complete Unity project, including scenes and scripts.
- Document the AR framework and image-tracking or marker-detection workflow actually used.
- Add screenshots showing the application running.
- Add a short demonstration video.
- Record the Unity version, device requirements, and exact build steps.
- Test the setup instructions on a clean environment.

## Author

**Venkatakishore125**

GitHub: [@Venkatakishore125](https://github.com/Venkatakishore125)

---

If you are reviewing this repository, please note that the current upload is a project report and documentation snapshot rather than a complete, runnable Unity project.
