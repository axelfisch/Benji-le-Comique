# Benji le Comique

Mise à jour du site existant `generatordrole.netlify.app`.

## Configuration serveur

- Netlify AI Gateway fournit `ANTHROPIC_BASE_URL` au serveur et garde l’authentification hors du navigateur.
- `BENJI_CLAUDE_MODEL` : facultatif. Par défaut : `claude-sonnet-4-5-20250929`.

La fonction `/api/benji-description` accepte uniquement les requêtes POST et applique une limite Netlify de trois appels par trois minutes, par IP et par domaine. Le navigateur garde aussi une limite simple de dix propositions par jour.

## Photo

La photo approuvée est `public/benji.jpeg`. Le cadrage CSS conserve le visage et les oreilles dans le portrait circulaire.

## Validation

1. Tester localement avec `netlify dev`.
2. Créer une prévisualisation avec `netlify deploy`.
3. Vérifier le bouton IA, les modifications du texte, les erreurs, les deux boutons de copie existants et le portrait sur ordinateur et mobile.
4. Publier seulement après validation de la photo et de la variable serveur.
