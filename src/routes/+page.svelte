<script>
  import {P, Heading, Li, List, Img, Button, Card} from "flowbite-svelte";
  import {CheckCircleSolid} from "flowbite-svelte-icons";
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
        >Erstellen Sie:
        </Heading
        >
        <List tag="ul" class="text-gray-500 dark:text-gray-400 ps-5">
          <Li icon>
            <CheckCircleSolid class="w-3.5 h-3.5 me-2 text-green-500 dark:text-green-400"/>
            Umfragen
          </Li>
          <Li icon>
            <CheckCircleSolid class="w-3.5 h-3.5 me-2 text-green-500 dark:text-green-400"/>
            Quizfragen
          </Li>
          <Li icon>
            <CheckCircleSolid class="w-3.5 h-3.5 me-2 text-green-500 dark:text-green-400"/>
            Anmeldeformulare
          </Li>
          <Li icon>
            <CheckCircleSolid class="w-3.5 h-3.5 me-2 text-green-500 dark:text-green-400"/>
            Bestellformulare
          </Li>
          <Li icon>
            <CheckCircleSolid class="w-3.5 h-3.5 me-2 text-green-500 dark:text-green-400"/>
            und vieles mehr...
          </Li>
        </List>
      </P>
      <div class="flex gap-5 mt-14">
        <Button>Sofort loslegen</Button>
        <Button color="alternative">Funktionen entdecken</Button>
      </div>
    </div>
    <Img src="undraw_forms_re_pkrt.svg" alt="form" class="lg:w-1/2 m-auto"/>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-20 mx-5 mt-14 md:mt-40">
    <Card>
      <h5 class="mb-5 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Freiheit</h5>
      <p class="mb-5 font-normal text-gray-700 dark:text-gray-400 leading-tight">Mit unserer Open-Source-Plattform sind
        Sie nicht durch restriktive Lizenzen oder teure Abonnements eingeschränkt. Erstellen Sie Formulare, die Ihre
        einzigartige Vision widerspiegeln, ohne dabei Ihr Budget zu sprengen.</p>
    </Card>
    <Card>
      <h5 class="mb-5 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Anpassung ohne Kompromisse</h5>
      <p class="mb-5 font-normal text-gray-700 dark:text-gray-400 leading-tight">Passen Sie Ihre Formulare an Ihre
        spezifischen Anforderungen an mit unserer flexiblen und anpassbaren Plattform. Von Designelementen bis hin zur
        Funktionalität - übernehmen Sie die Kontrolle über jeden Aspekt Ihrer Formulare und heben Sie das Nutzererlebnis
        auf ein neues Level.</p>
    </Card>
    <Card>
      <h5 class="mb-5 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Noteworthy technology
        acquisitions 2021</h5>
      <p class="mb-5 font-normal text-gray-700 dark:text-gray-400 leading-tight">Here are the biggest enterprise
        technology acquisitions of 2021 so far, in reverse chronological order.</p>
    </Card>
  </div>
</div>
