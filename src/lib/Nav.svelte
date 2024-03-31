<script>
  import {
    Navbar,
    NavBrand,
    NavHamburger,
    NavUl,
    NavLi,
    Dropdown,
    DropdownItem,
    DropdownDivider,
  } from "flowbite-svelte";
  import { ChevronDownOutline } from "flowbite-svelte-icons";
  import { DarkMode } from "flowbite-svelte";
  import { page } from "$app/stores";
  $: activeUrl = $page.url.pathname;
</script>

<Navbar color="form" class="mb-20">
  <NavBrand href="/">
    <img src="logo.svg" class="me-3 h-6 sm:h-9" alt="Formulate Logo" />
    <span
      class="self-center whitespace-nowrap text-xl font-semibold dark:text-white"
      >Formulate</span
    >
  </NavBrand>
  <div class="flex md:order-2 gap-3">
    <DarkMode
      class="text-primary-500 dark:text-primary-600 border border-gray-300 dark:border-gray-600"
    />
    <NavHamburger />
  </div>
  <NavUl class="md:order-1" {activeUrl}>
    <NavLi href="/">Übersicht</NavLi>
    <NavLi href="/functions">Funktionen</NavLi>
    <NavLi href="/documentation">Dokumentation</NavLi>
    <NavLi href="/pricing">Preise</NavLi>
    <NavLi href="/contact">Kontakt</NavLi>
    <NavLi class="cursor-pointer">
      Loslegen<ChevronDownOutline
        class="w-5 h-5 ms-2 text-primary-800 dark:text-white inline"
      />
    </NavLi>
    <Dropdown
      class="w-44 z-20 border-2 border-gray-300 dark:border-gray-600 rounded-md"
    >
      <DropdownItem href="#">Login</DropdownItem>
      <DropdownItem href="#">Registrieren</DropdownItem>
      <DropdownDivider />
      <DropdownItem href="/">Sign out</DropdownItem>
    </Dropdown>
  </NavUl>
</Navbar>
