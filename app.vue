<script setup lang="ts">
const route = useRoute()
const items = [
  'https://picsum.photos/1920/1080?random=1',

]

const isOpen = ref(false)
const isOpen2 = ref(false)
const isOpen3 = ref(false)
const isOpen4 = ref(false)
 
</script>

<template class="bg-indigo-950">
  <div class="flex flex-col w-screen h-screen bg-zinc-200 items-center overflow-x-hidden">

    <div class="flex w-screen fixed z-10 h-15 bg-slate-100/85 backdrop-blur-lg items-center justify-evenly">

      <div class="flex items-center justify-center">
        <Icon name="i-ri-supabase-fill" class="text-2xl text-yellow-400" />
        <div class="flex items-center justify-center text-indigo-950 text-3xl font-light pl-3 cursor-default">OndinaTec</div>
      </div>

        <div class="flex items-center justify-center">
          <div class="flex transition-all items-center justify-center font-semibold text-indigo-950 text-sm border-b border-indigo-950/0
            hover:border-indigo-950 cursor-pointer m-5 text-center">
          <Icon name="i-ri-user-line" class="text-lg m-1 text-center" />Entrar</div>
      
          <div class="flex transition-all items-center justify-center bg-indigo-950 p-2 px-5 rounded-md text-center
            hover:bg-indigo-950/90 cursor-pointer max-sm:px-2"
          > 
            <Icon name="heroicons-bars-3" class="text-2xl text-yellow-400 hidden max-sm:flex" />
            <h1 class="font-semibold text-center text-yellow-400 text-sm max-sm:hidden">Cadastre-se</h1>
          </div>
        </div>

    </div>

    <div class="flex flex-col pt-11 w-screen h-full items-center">
      <div class="flex flex-col w-screen h-screen bg-[url('public/servico.png')] bg-center items-center justify-center">
        <div class="flex w-screen h-screen bg-transparent rounded-md backdrop-blur-lg
        items-center justify-center
         ">
         
         <div class="flex flex-col p-2  items-center justify-center">
            <h1 class="flex text-6xl text-indigo-100 font-bold italic max-sm:text-4xl">Serviços Eletricos</h1>

            <h2 class="flex transition-all text-sm m-4 font-medium text-yellow-400 bg-indigo-950/85 p-2 px-5 rounded-md cursor-pointer hover:bg-indigo-950
            items-center justify-center
            ">
              <Icon name="i-ri-shield-flash-fill" class="text-lg mx-2" />
              Agende um serviço rapidamente</h2>
         </div>


        </div>

      </div>

      <div class="flex flex-col w-11/12 rounded-md m-8 h-screen bg-white shadow-xl items-center justify-center">
        <h1 class="flex p-4 text-4xl text-indigo-950 font-light">Sobre</h1>

        <h1 class="flex items-center justify-center p-8 font-semibold text-sm text-center text-indigo-950">
          Nossa equipe de profissionais qualificados e experientes está pronta para atender a todas as suas necessidades elétricas, incluindo:
          Instalação de Painéis Solares: Projetamos e instalamos sistemas
           de energia solar personalizados para residências e empresas,
            ajudando você a economizar na conta de luz e a contribuir
             para um futuro mais sustentável.
          Manutenção e Reparos:
           Oferecemos serviços de manutenção preventiva
            e corretiva para garantir que seus sistemas
             elétricos funcionem com eficiência e segurança,
              minimizando o risco de falhas e interrupções.
         </h1>
      </div>

      <div class="flex flex-col w-screen h-screen bg-[url('public/produto1.png')] bg-center items-center justify-center">
        <div class="flex w-screen h-screen backdrop-blur-md bg-black/70 transition-all
        items-center justify-center
         ">
         
         <div class="flex flex-row w-screen items-center justify-around max-sm:flex-col">
          <img src="public/produto1.png" alt="servico" class="flex w-72 rounded-md shadow-xl transition-al
          cursor-pointer
          ">

          <div class="flex flex-col p-2 items-center justify-center m-9">
            <h1 class="flex flex-col text-6xl font-bold italic items-center justify-center">Serviço<h1 class="flex font-normal text-sm">Exclusivo</h1></h1>
            
            <UButton class="flex m-2 px-4 border bg-transparent" color="" @click="isOpen2 = true"><h1 class="text-indigo-100">Detalhes</h1></UButton>
          </div>
         </div>


        </div>

      </div>


      <div class="flex flex-col w-screen h-screen bg-[url('public/produto2.png')] border-t-2 bg-center items-center justify-center">
        <div class="flex w-screen h-screen backdrop-blur-md bg-black/70 transition-all
        items-center justify-center
         ">
         
         <div class="flex flex-row w-screen items-center justify-around max-sm:flex-col">
          <img src="public/produto2.png" alt="servico" class="flex w-72 rounded-md shadow-xl transition-all border-indigo-200
          cursor-pointer
          ">

          <div class="flex flex-col p-2 items-center justify-center m-9">
            <h1 class="flex flex-col text-6xl font-bold italic items-center justify-center">Servico<h1 class="flex font-normal text-sm">Exclusivo</h1></h1>
            
            <UButton class="flex m-2 px-4 border bg-transparent" color="" @click="isOpen3 = true"><h1 class="text-indigo-100">Detalhes</h1></UButton>
          </div>
         </div>


        </div>

      </div>


      <div class="flex flex-col w-screen h-screen bg-[url('public/produto3.png')] border-t-2 bg-center items-center justify-center">
        <div class="flex w-screen h-screen backdrop-blur-md bg-black/70 transition-all
        items-center justify-center
         ">
         
         <div class="flex flex-row w-screen items-center justify-around max-sm:flex-col">
          <img src="public/produto3.png" alt="servico" class="flex w-72 rounded-md shadow-xl transition-all border-indigo-200
          cursor-pointer
          ">

          <div class="flex flex-col p-2 items-center justify-center m-9">
            <h1 class="flex flex-col text-6xl font-bold italic items-center justify-center">Servico<h1 class="flex font-normal text-sm">Exclusivo</h1></h1>
            
            <UButton class="flex m-2 px-4 border bg-transparent" color="" @click="isOpen4 = true"><h1 class="text-indigo-100">Detalhes</h1></UButton>
          </div>
         </div>


        </div>

      </div>


      <div class="flex flex-col w-screen h-screen bg-[url('public/produto4.png')] border-t-2 bg-center items-center justify-center">
        <div class="flex w-screen h-screen backdrop-blur-md bg-black/70 transition-all
        items-center justify-center
         ">
         
         <div class="flex flex-row w-screen items-center justify-around max-sm:flex-col">
          <img src="public/produto4.png" alt="servico" class="flex w-72 rounded-md shadow-xl transition-all border-indigo-200
          cursor-pointer
          ">

          <div class="flex flex-col p-2 items-center justify-center m-9">
            <h1 class="flex flex-col text-6xl font-bold italic items-center justify-center">Servico<h1 class="flex font-normal text-sm">Exclusivo</h1></h1>
            
            <UButton class="flex m-2 px-4 border bg-transparent" color="" @click="isOpen = true"><h1 class="text-indigo-100">Detalhes</h1></UButton>
          </div>
         </div>


        </div>

      </div>

      <UModal v-model="isOpen">
        <UButton color="" variant="ghost" icon="i-heroicons-x-mark-20-solid" class="bg-indigo-950 py-2 px-4 justify-end" @click="isOpen = false" />
        <div class="flex flex-row items-center justify-center p-4 bg-indigo-950 rounded-md">
          <h1 class="flex flex-col items-center justify-center p-2">
            <h1 class="flex flex-row p-2 text-xl font-light text-white items-center justify-center">
              <Icon name="i-ri-supabase-fill" class="text-2xl text-yellow-400 mr-2 " />
              OndinaTec
            </h1>
            <h1 class="flex p-3 text-3xl font-extralight italic text-center">Instalaçao de Painel Solar</h1>

            <h1 class="flex text-sm font-bold text-white text-center">Sustentabilidade:</h1>
            <h1 class="flex mb-2 text-lg font-extralight text-white/55 text-center">
              A energia solar é uma fonte renovável e inesgotável de energia, diferente dos combustíveis fósseis que são finitos.
            </h1>

            <h1 class="flex text-sm font-bold text-white mt-2 text-center">Redução de Emissões de CO2:</h1>
            <h1 class="flex mb-2 text-lg font-extralight text-white/55 text-center">
              A produção de energia solar não emite gases de efeito estufa, contribuindo para a redução da pegada de carbono e mitigação das mudanças climáticas.
            </h1>

            <h1 class="flex text-sm font-bold text-white mt-2 text-center">Economia de Longo Prazo::</h1>
            <h1 class="flex mb-2 text-lg font-extralight text-white/55 text-center">
              Apesar do custo inicial de instalação, a energia solar pode resultar
               em economias significativas na conta de luz ao longo do tempo,
                especialmente em locais com alta incidência solar.
            </h1>
            
            <h1 class="flex mt-2 text-lg font-extralight text-indigo-400 shadow-xl p-1 px-10 transition-all bg-indigo-900/25
            hover:bg-indigo-900/50
             cursor-pointer rounded-md">Orçamento</h1>
          </h1>
        </div>
      </UModal>

            <UModal v-model="isOpen2">
              <UButton color="" variant="ghost" icon="i-heroicons-x-mark-20-solid" class="bg-indigo-950 py-2 px-4 justify-end" @click="isOpen2 = false" />
        <div class="flex flex-row items-center justify-center p-4 bg-indigo-950 rounded-md">
          <h1 class="flex flex-col items-center justify-center p-2">
            <h1 class="flex flex-row p-2 text-xl font-light text-white items-center justify-center">
              <Icon name="i-ri-supabase-fill" class="text-2xl text-yellow-400 mr-2" />
              OndinaTec
            </h1>
            <h1 class="flex p-3 text-3xl font-extralight italic text-center">Instalação Elétrica Residencial</h1>

            <h1 class="flex mb-2 text-lg font-extralight text-center text-white/55">
              Transforme sua casa
               com segurança e eficiência
                com nossos serviços de instalação elétrica residencial.
                 Nossa equipe de profissionais experientes está pronta para
                  garantir que sua instalação elétrica atenda a todos os padrões
                   de qualidade e segurança.
            </h1>

            <h1 class="flex text-sm font-bold text-white mt-2 text-center">Nossos serviços incluem:</h1>
            <h1 class="flex mb-2 text-lg font-extralight text-center text-white/55">
              Instalação de Circuitos Elétricos:
               Planejamento e instalação de circuitos
                elétricos para iluminação, tomadas e equipamentos,
                 garantindo que sua casa tenha energia suficiente e segura.
            </h1>

            <h1 class="flex text-sm font-bold text-white mt-2 text-center">Atualização de Fiação:</h1>
            <h1 class="flex mb-2 text-lg font-extralight text-white/55 text-center">
              Substituição ou atualização de fiação antiga para melhorar a segurança e eficiência energética da sua casa.
            </h1>

            <h1 class="flex text-sm font-bold text-white mt-2 text-center">Instalação de Iluminação:</h1>
            <h1 class="flex mb-2 text-lg font-extralight text-white/55 text-center">
              Instalação de sistemas de iluminação internos e externos, incluindo luzes de teto, spots e iluminação decorativa.
            </h1>

            <h1 class="flex text-sm font-bold text-white mt-2 text-center">Instalação de Tomadas e Interruptores:</h1>
            <h1 class="flex mb-2 text-lg font-extralight text-white/55 text-center">
              Instalação de tomadas e interruptores em locais estratégicos para atender às suas necessidades específicas.
            </h1>

            <h1 class="flex mt-2 text-lg font-extralight text-indigo-400 shadow-xl p-1 px-10 transition-all bg-indigo-900/25
            hover:bg-indigo-900/50
             cursor-pointer rounded-md">Orçamento</h1>
          </h1>
        </div>
      </UModal>

      <UModal v-model="isOpen3">
              <UButton color="" variant="ghost" icon="i-heroicons-x-mark-20-solid" class="bg-indigo-950 py-2 px-4 justify-end" @click="isOpen3 = false" />
        <div class="flex flex-row items-center justify-center p-4 bg-indigo-950 rounded-md">
          <h1 class="flex flex-col items-center justify-center p-2">
            <h1 class="flex flex-row p-2 text-xl font-light text-white items-center justify-center">
              <Icon name="i-ri-supabase-fill" class="text-2xl text-yellow-400 mr-2" />
              OndinaTec
            </h1>
            <h1 class="flex p-3 text-3xl font-extralight italic text-center">Instalação Elétrica Predial</h1>

            <h1 class="flex mb-2 text-lg font-extralight text-center text-white/55">
              Garanta a eficiência e segurança elétrica do seu edifício
               com nossos serviços especializados de instalação elétrica predial.
                Nossa equipe de eletricistas qualificados está preparada para atender todas as suas necessidades,
                 desde a fase de instalação até a manutenção contínua.
            </h1>

            <h1 class="flex text-sm font-bold text-white mt-2 text-center">Sistemas de Segurança Elétrica:</h1>
            <h1 class="flex mb-2 text-lg font-extralight text-center text-white/55">
              Instalação de dispositivos de proteção contra surtos,
               disjuntores e outros sistemas de segurança elétrica para proteger
                seu edifício e seus ocupantes.
            </h1>

            <h1 class="flex text-sm font-bold text-white mt-2 text-center">Automação Predial:</h1>
            <h1 class="flex mb-2 text-lg font-extralight text-white/55 text-center">
              Integração de sistemas de automação para controlar iluminação,
               climatização e outros equipamentos, proporcionando maior conforto e eficiência energética.
            </h1>

            <h1 class="flex text-sm font-bold text-white mt-2 text-center">Manutenção e Diagnóstico:</h1>
            <h1 class="flex mb-2 text-lg font-extralight text-white/55 text-center">
              Serviços regulares de manutenção e diagnósticos para assegurar que todo o sistema elétrico
               funcione de maneira eficiente e segura.
            </h1>

            <h1 class="flex mt-2 text-lg font-extralight text-indigo-400 shadow-xl p-1 px-10 transition-all bg-indigo-900/25
            hover:bg-indigo-900/50
             cursor-pointer rounded-md">Orçamento</h1>
          </h1>
        </div>
      </UModal>


      <UModal v-model="isOpen4">
            <UButton color="" variant="ghost" icon="i-heroicons-x-mark-20-solid" class="bg-indigo-950 py-2 px-4 justify-end" @click="isOpen4 = false" />
        <div class="flex flex-row items-center justify-center p-4 bg-indigo-950 rounded-md">
          <h1 class="flex flex-col items-center justify-center p-2">
            <h1 class="flex flex-row p-2 text-xl font-light text-white items-center justify-center">
              <Icon name="i-ri-supabase-fill" class="text-2xl text-yellow-400 mr-2" />
              OndinaTec
            </h1>
            <h1 class="flex p-3 text-3xl font-extralight italic text-center">Troca de Resistência Elétrica</h1>

            <h1 class="flex mb-2 text-lg font-extralight text-center text-white/55">
              Seus aparelhos elétricos em perfeito
               funcionamento com nosso serviço especializado
                de troca de resistência. Nossos técnicos qualificados
                 estão prontos para identificar e substituir resistências
                  defeituosas em uma variedade de dispositivos e sistemas.
            </h1>

            <h1 class="flex text-sm font-bold text-white mt-2 text-center">Substituição Rápida e Eficiente:</h1>
            <h1 class="flex mb-2 text-lg font-extralight text-center text-white/55">
              Troca rápida e segura das resistências defeituosas,
               utilizando peças de alta qualidade para garantir o melhor
                desempenho dos seus equipamentos.
            </h1>

            <h1 class="flex text-sm font-bold text-white mt-2 text-center">Assistência Técnica Especializada:</h1>
            <h1 class="flex mb-2 text-lg font-extralight text-white/55 text-center">
              Orientação profissional sobre o uso correto e a manutenção de resistências elétricas, ajudando a evitar problemas futuros.
            </h1>

            <h1 class="flex text-sm font-bold text-white mt-2 text-center">Atendimento Residencial e Comercial:</h1>
            <h1 class="flex mb-2 text-lg font-extralight text-white/55 text-center">
              Serviço disponível tanto para residências
               quanto para estabelecimentos comerciais,
                garantindo que todos os seus equipamentos estejam sempre em perfeito estado de funcionamento
            </h1>

            <h1 class="flex mt-2 text-lg font-extralight text-indigo-400 shadow-xl p-1 px-10 transition-all bg-indigo-900/25
            hover:bg-indigo-900/50
             cursor-pointer rounded-md">Orçamento</h1>
          </h1>
        </div>
      </UModal>



      <div class="flex flex-row w-screen h-screen p-3 items-center justify-around max-sm:flex-col">
        <div class="font-bold text-sm text-indigo-950 max-sm:mb-4">2024 © OndinaTec</div>
        <div class="font-bold text-sm text-indigo-950 max-sm:mb-4">Contato: 71 9 8117-5859</div>

        
        <div class="flex flex-row">
          <UInput
            icon="i-heroicons-envelope-20-solid"
            size="sm"
            color=""
            :trailing="false"
            variant="none"
            class="font-semibold border-2 border-indigo-950 rounded-md text-indigo-950"
            placeholder="Receber Promoções"
          />
          <UButton class="flex ml-2 px-4 bg-indigo-950" color="" onclick="loading"><h1 
          class="font-semibold text-center text-yellow-400 text-sm">Receber</h1></UButton>
        </div>
      </div>


    </div>
  </div>
</template>

