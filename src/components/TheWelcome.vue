<script setup lang="ts">
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import HumanGreetingIcon from 'vue-material-design-icons/HumanGreeting.vue';
import DesktopClassicIcon from 'vue-material-design-icons/DesktopClassic.vue';
import FoodVariantIcon from 'vue-material-design-icons/FoodVariant.vue';
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Vortragsfolien</template>
    <p>Der KNF stellt zu den meisten Vorträgen zeitnah die jeweiligen
    Foliensätze im PDF-Format zum Download bereit.</p>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <HumanGreetingIcon />
    </template>
    <template #heading>Treffpunkt</template>
    <p>Wie in den letzten Jahren findet die Präsenzveranstaltung in
    den Räumlichkeiten des <a href="https://www.parks-nuernberg.de">PARKS</a>
    in Nürnberg statt.</p>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <DesktopClassicIcon />
    </template>
    <template #heading>Online</template>
    <p>Alle Vorträge sind auch über die Online-Meeting-Infrastruktur
    des KNF e.V. zugänglich. Für den Zugang ist eine vorherige
    Registrierung erforderlich.</p>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <FoodVariantIcon />
    </template>
    <template #heading>Verpflegung</template>
    <p>Am Ort der Präsenzveranstaltung stellt der KNF ein Buffet zur
    Verfügung. Zudem gibt es während der gesamten Veranstaltungszeit
    kalte und warme Getränke.</p>
  </WelcomeItem>
</template>
