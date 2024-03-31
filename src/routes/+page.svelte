<script>
  import { P, Heading, Li, List, Img, Button } from "flowbite-svelte";
  import { CheckCircleSolid } from "flowbite-svelte-icons";
</script>

<div class="md:container md:mx-auto">
  <div class="grid grid-cols-1 md:grid-cols-2 gap-20 mx-5">
    <div>
      <Heading tag="h1" class="mb-10">Willkommen bei Formulate</Heading>
      <P>
        Formulate ist eine Open-Source-Lösung, mit der Sie ganz einfach
        Formulare für Schule, Arbeit, Unternehmen oder den privaten Gebrauch
        erstellen können.
        <Heading tag="h2" customSize="text-lg font-semibold" class="mt-10"
          >Erstellen Sie:</Heading
        >
        <List tag="ul" class="text-gray-500 dark:text-gray-400 ps-5">
          <Li icon
            ><CheckCircleSolid
              class="w-3.5 h-3.5 me-2 text-green-500 dark:text-green-400"
            />Umfragen</Li
          >
          <Li icon
            ><CheckCircleSolid
              class="w-3.5 h-3.5 me-2 text-green-500 dark:text-green-400"
            />Quizfragen</Li
          >
          <Li icon
            ><CheckCircleSolid
              class="w-3.5 h-3.5 me-2 text-green-500 dark:text-green-400"
            />Anmeldeformulare</Li
          >
          <Li icon
            ><CheckCircleSolid
              class="w-3.5 h-3.5 me-2 text-green-500 dark:text-green-400"
            />Bestellformulare</Li
          >
          <Li icon
            ><CheckCircleSolid
              class="w-3.5 h-3.5 me-2 text-green-500 dark:text-green-400"
            />und vieles mehr...</Li
          >
        </List>
      </P>
    </div>
    <Img src="undraw_forms_re_pkrt.svg" alt="form" class="lg:w-1/2 m-auto" />
    <div class="flex gap-5">
      <Button>Sofort loslegen</Button>
      <Button color="alternative">Funktionen entdecken</Button>
    </div>
  </div>
</div>
