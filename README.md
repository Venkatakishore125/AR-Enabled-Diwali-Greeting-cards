# AR-Enabled-Diwali-Greeting-cards
public class Soundmanager : MonoBehaviour
{
   public AudioSource Asource;
   public AudioClip Aclip;
   public void playsound()
   {
        Asource.PlayOneShot(Aclip);
        public void Stopsound()
        {
             Asource.Stop();
        }
    }
