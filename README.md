# Spiegel Plus 
Spon Plus - Tampermonkey script um die "Verschlüsselung" zu umgehen, alles in einer Zeile.

Es handelt sich hier um lediglich eine Zeile Code. Welche auch bei einer tatsächlichen Zahlung ausgeührt werden würde wie im HEAD definiert:

```html
<meta property="laterpay:connector:callbacks:on_user_has_access" content="SPLaterpayCallbackHasAccess" />
```

Auf Basis dessen dann folgender Script, die Methode könnt ihr natürlich in eine beliebige Extention kopieren, muss ja nicht Tampermonkey sein.
```javascript
(function() {
	 SPLaterpayCallbackHasAccess();
})();
```

Kann sein, dass es beim ersten Laden des Artikels nicht direkt greift, kurzer refresh reicht.
