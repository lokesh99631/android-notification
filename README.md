# android-notification
from kivy.app import App
from kivy.uix.button import Button
import plyer

class Instagram(App):
    def build(self):
        return Button(text='press For Updates', on_press=self.notify)

    def notify(self, obj):
        plyer.notification.notify(title="Hello User", messsage="You have New Friend Request")

Instagram().run()
