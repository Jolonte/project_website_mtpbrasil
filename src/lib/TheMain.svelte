<script lang="ts">
    // imports
    import TheButton from "../components/TheButton.svelte";
    import Services from "../components/Services.svelte";
    import TheChip from "../components/TheChip.svelte";
    import TheForm from "../components/TheForm.svelte";
    import TheQuestions from "../components/TheQuestions.svelte";
    import ThePosts from "../components/ThePosts.svelte";

    // Services data
    const SERVICES = [
        {
            icon: 'workspace_premium',
            title: 'Garantia da qualidade',
            desc: 'Atuamos em todas as fases da atividade comercial de software, desde o desenvolvimento até a garantia de qualidade, visando uma melhoria contínua.'
        },
        {
            icon: 'touch_app',
            title: 'Experiência do usuário',
            desc: 'Desenvolvimento de software completo, da criação à garantia de qualidade, para melhoria contínua em todas as etapas comerciais.'
        },
        {
            icon: 'shield',
            title: 'Segurança',
            desc: 'A MTP oferece soluções e práticas em segurança cibernética, detectando e prevenindo vulnerabilidades em aplicativos de organizações.'
        },
        {
            icon: 'cycle',
            title: 'DevOps',
            desc: 'Cobertura completa do ciclo de vida do software em iniciativas digitais, incluindo aplicativos móveis e de e-business para vários dispositivos.'
        }
    ]

    // Questions data
    const QUESTIONS = [
        {
            title: 'Há quanto tempo a empresa está no mercado?',
            answer: 'A MTP está há 25 anos no mercado, atuando na prestação de serviços em tecnologia da informação.'
        },
        {
            title: 'Quais são os principais serviços que a empresa oferece?',
            answer: 'A empresa oferece serviços de garantia da qualidade, experiência do usuário, segurança cibernética e DevOps para organizações que buscam melhorias contínuas em seus produtos e serviços.'
        },
        {
            title: 'Quais são as vantagens competitivas da empresa em relação aos concorrentes?',
            answer: 'As vantagens competitivas da empresa incluem sua experiência no mercado, conhecimento em tecnologias emergentes e compromisso em oferecer serviços de qualidade e segurança aos clientes.'
        },
        {
            title: 'Quais são os clientes atuais da empresa e qual é o nível de satisfação deles com os serviços prestados?',
            answer: 'A empresa tem uma carteira de clientes diversificada e mantém um alto nível de satisfação dos clientes em relação aos serviços prestados.'
        },
        {
            title: 'Como a empresa garante a qualidade dos serviços prestados?',
            answer: 'A empresa garante a qualidade dos serviços prestados através da adoção de metodologias e práticas de qualidade reconhecidas no mercado, além de uma equipe de profissionais altamente capacitados.'
        },
        {
            title: 'Qual é a abordagem da empresa em relação à inovação e atualização tecnológica?',
            answer: 'A empresa tem uma abordagem proativa em relação à inovação e atualização tecnológica, buscando sempre oferecer serviços que estejam alinhados com as necessidades do mercado.'
        },
        {
            title: 'A empresa possui algum tipo de política de privacidade e segurança da informação?',
            answer: 'A empresa possui uma política de privacidade e segurança da informação para garantir a proteção de dados de seus clientes.'
        },
        {
            title: 'Como a empresa lida com a proteção de dados de seus clientes?',
            answer: 'A empresa mantém políticas rígidas de segurança da informação para garantir a proteção de dados dos clientes, em conformidade com as regulamentações nacionais e internacionais aplicáveis.'
        },
        {
            title: 'A empresa possui alguma certificação ou reconhecimento em sua área de atuação?',
            answer: 'A empresa possui certificações em suas áreas de atuação, incluindo a certificação ISO 27001:2013 em segurança da informação.'
        },
        {
            title: 'Como a empresa está preparada para lidar com imprevistos e situações de crise?',
            answer: 'A empresa está preparada para lidar com imprevistos e situações de crise, mantendo um plano de contingência bem estruturado e equipes de suporte disponíveis para atuar em qualquer eventualidade.'
        },
    ]
</script>

<main>
    <div class="flex flex-col items-center py-[3.5rem] gap-[2.5rem] bg-[#2f2e41]">
        <h2 class="text-3xl font-semibold text-white">Trabalhamos com as melhores empresas</h2>
        <div class="flex justify-center gap-[3.25rem]">
            <img class="h-20" src="/coca_cola.png" alt="Coca-Cola">
            <img class="h-20" src="/avon.png" alt="Avon">
            <img class="h-20" src="/enel.png" alt="Enel">
            <img class="h-20" src="/bayern.png" alt="Bayern">
        </div>
        <p class="font-bold text-blue-600">Conheça todos os nossos clientes ></p>
    </div>
    <div class="flex flex-col py-[9.5rem]">
        <section class="flex flex-col items-center text-center gap-[4.5rem] mb-[11.688rem]">
            <div class="flex flex-col items-center gap-[1.438rem]">
                <h2 class="text-4xl font-bold capitalize text-[#2f2e41]"><span class="text-blue-600">Potencializando</span> seu <span class="text-blue-600">sucesso</span> com nossos serviços</h2>
                <p class="w-2/4">A MTP é líder em Serviços de Garantia Digital, com 25 anos de experiência global. Seu compromisso com a qualidade, inovação e adaptação às mudanças do mercado é integrado ao ambiente de Digital Business Assurance.</p>
            </div>
            <div class="grid grid-cols-2 grid-rows-2 justify-center gap-[2.688rem]">
                {#each SERVICES as service}
                    <Services propIcon="{service.icon}" propTitle="{service.title}" propDesc="{service.desc}" />
                {/each}
            </div>
            <TheButton propTitle="Mais informações" />
        </section>
        <section class="flex flex-col items-center py-[11.688rem] px-[12.25rem] bg-[#2f2e41] mb-[7.5rem] gap-[2rem]">
            <div class="flex flex-col items-center gap-[2rem]">
                <h2 class="text-4xl font-semibold text-white">Entre em contato</h2>
                <div class="flex justify-center gap-[1.5rem]">
                    <TheChip propTitle="Brasil" />
                    <TheChip propTitle="Espanha" />
                    <TheChip propTitle="Mexico" />
                </div>
            </div>
            <div class="flex flex-col w-[55rem] rounded-[0.938rem] drop-shadow-xl">
                <div class="flex flex-col w-full p-[2rem] gap-[2rem] rounded-[0.938rem] bg-[#dfe6e9]">
                    <div class="flex justify-center flex-wrap gap-[0.5rem]">
                        <!-- reatividade -->
                        <button class="w-[8rem] text-white py-[0.625rem] px-[1.125rem] rounded-[0.938rem] border-[0.1rem] bg-[#2f2e41]">Madrid</button>
                        <button class="w-[8rem] text-[#2f2e41] py-[0.625rem] px-[1.125rem] rounded-[0.938rem] border-[0.1rem] border-[#2f2e41]">Alicante</button>
                        <button class="w-[8rem] text-[#2f2e41] py-[0.625rem] px-[1.125rem] rounded-[0.938rem] border-[0.1rem] border-[#2f2e41]">Sevilla</button>
                        <button class="w-[8rem] text-[#2f2e41] py-[0.625rem] px-[1.125rem] rounded-[0.938rem] border-[0.1rem] border-[#2f2e41]">Almería</button>
                        <button class="w-[8rem] text-[#2f2e41] py-[0.625rem] px-[1.125rem] rounded-[0.938rem] border-[0.1rem] border-[#2f2e41]">Barcelona</button>
                    </div>
                    <div class="h-[20rem] w-full rounded-[0.938rem] bg-slate-400"></div>
                    <div class="flex flex-col gap-[0.5rem]">
                        <!-- reatividade -->
                        <p>Endereço: Rua Correia Dias, 337 - 4º Andar Paraíso. CEP: 04104-901</p>
                        <p>Telefone: +55 (11) 5525-0650</p>
                        <p>E-mail: contato@mtp.com.br</p>
                    </div>
                    <h3 class="font-bold text-2xl">Fale conosco</h3>
                    <TheForm />
                </div>
            </div>
        </section>
        <!-- objeto com "props" que da para por html dentro -->
        <section class="flex flex-col items-center text-center gap-[4.5rem] mb-[7.5rem]">
            <div class="flex flex-col items-center gap-[1.438rem]">
                <h2 class="text-4xl font-bold capitalize text-[#2f2e41]">Nossas certificações</h2>
                <p class="w-2/4">Buscamos constantemente certificações e aprimoramento de qualidade atestando a conformidade do nosso sistema aos mais rigorosos padrões internacionais.</p>
            </div>
            <div class="flex gap-[4.5rem]">
                <img class="h-48" src="/certification1.png" alt="Great place to work">
                <img class="h-48" src="/certification2.png" alt="ISO 9001">
                <img class="h-48" src="/certification3.png" alt="ISO 27001">
            </div>
        </section>
        <section class="flex flex-col gap-[2rem] px-[12.25rem] mb-[7.5rem]">
            <div class="flex flex-col items-start gap-[1rem]">
                <h2 class="text-4xl font-bold capitalize text-[#2f2e41]">Últimas postagens</h2>
                <p class="font-bold text-blue-600">Ver blog completo ></p>
            </div>
            <div class="flex justify-evenly gap-[2rem]">
                <ThePosts />
                <ThePosts />
                <ThePosts />
            </div>
        </section>
        <section class="flex flex-col gap-[3.5rem] px-[12.25rem] mb-[7.5rem]">
            <div class="flex flex-col items-start gap-[1rem]">
                <h2 class="text-4xl font-bold capitalize text-[#2f2e41]">Perguntas frequentes</h2>
            </div>
            <div class="flex flex-col gap-[2rem]">
                {#each QUESTIONS as question}
                    <TheQuestions propTitle="{question.title}" />
                {/each}
            </div>
        </section>
    </div>
</main>
