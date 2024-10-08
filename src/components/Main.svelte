<script>
    import Step from "./Step.svelte";

    let steps = [
        {
            name: "Exam Portal",
            icon: "fa-solid fa-laptop-code",
            description:
                "The Exam Portal, a Full Stack application built with Spring Boot and React JS, serves as a comprehensive solution for universities to manage online examinations for students. The system consists of three main modules: Admin, Teacher, and Student.",
            link: "https://examportalonline.netlify.app/"
        },
        {
            name: "Algorithm Visualizer",
            icon: "fa-solid fa-chart-column",
            description:
                "Algorithm Visualizer is an interactive web application designed to help users understand and visualize the functioning of various algorithms.",
            link: "https://algvisual.netlify.app/"
        },
        {
            name: "IntervjuPiO",
            icon: "fa-solid fa-clipboard-question",
            description:
                "IntervjuPiO, a Full Stack application built with Spring Boot and React JS, allows viewing and downloading documents with questions and answers for interviews.",
            link: "https://intervjupio.netlify.app/"
        },
        {
            name: "Book Advisor",
            icon: "fa-solid fa-book-open-reader",
            description:
                "The system consists of both frontend and backend components, with the frontend built using React.js and the backend powered by Flask.",
            link: "https://bookadvisor.netlify.app/"
        },
    ];

    let benefits = [
        {
            metric: "10x",
            name: "a self taught developer",
            description:
                "I embarked on a journey of self-learning, delving into the world of coding with a focus on Java, Spring Boot, and MySQL for backend development. Alongside, I acquired proficiency in Python and familiarity with React for frontend development. Through dedicated practice and exploration, I've cultivated a deep understanding of building robust digital infrastructures. Eager to expand my expertise, I aspire to delve into cloud computing, driven by a passion for innovation and continuous growth.",
        },
        {
            name: "a programming enthusiast",
            description:
                "I'm fueled by my passion for coding and the endless possibilities it offers. Embracing each challenge as an opportunity to grow, I'm enthusiastic about mastering new languages and technologies. ",
        },
        {
            name: "an excellent communicator",
            description:
                "Communication is key and it's a paramount value of mine. I believe in transparency and constructive communication above all else. This helps me develop deep relationships and ensures my effectiveness and productivity in any work space with any team.",
        },
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <section
        id="introPage"
        class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
    >
        <div
            class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10"
        >
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm <span class="poppins text-violet-400">Nikola</span> Knezevic
                <br />Software
                <span class="poppins text-violet-400">Developer</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                My <span class="text-violet-400"> favorite tech</span> includes Java
                (Spring Boot), Python, React & MySql
                or MongoDB!
            </p>
            <a
                class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl 
                poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950
                cursor-pointer"
                href="#footer"
                >
                <div
                    class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
                />
                <h4 class="relative z-9">Get in touch &rarr;</h4>
            </a>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img
                src={"images/profile.png"}
                alt="Zetane Engine"
                class="object-cover z-[2] max-h-[70vh]"
            />
        </div>
           
    </section>
    <section class="py-20 lg:py-32 flex flex-col gap-24" id="projects">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-large sm:text-xl md:text-2xl">
                A few of my creative endeavors.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class="poppins text-violet-400">see</span> my work?
            </h3>
        </div>
     
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            <Step step={steps[0]}>
                <p>
                    The Exam Portal is a Full Stack application built with <strong
                        class="text-violet-400"
                        >Spring Boot, React JS, MySql and Docker!</strong
                    > The Exam Portal using Spring Boot & React JS is a Full Stack application that can be used by any University to handle the Student Online Examination. For testing you can use Role: Admin, User: admin@demo.com, Password: admin1234.
                </p>
            </Step>
            <Step step={steps[1]}>
                <p>
                    Algorithm Visualizer is an interactive web application designed to help users understand and 
                    visualize the functioning of various algorithms. 
                    Built with a modern tech stack including <strong class="text-violet-400">Spring Boot</strong> and
                    <strong class="text-violet-400" >React</strong>, this project serves as a 
                    comprehensive educational tool and a showcase of efficient software architecture.
                </p>
            </Step>
            <Step step={steps[2]}>
                <p>
                    IntervjuPiO is an application that allows viewing and downloading documents with questions and answers for interviews. 
                    The application consists of a <strong
                        class="text-violet-400"
                        >Spring Boot, React and MongoDB.</strong
                    > This is a simple application to assist with learning for technical interviews. The files are available in both Serbian and English.
                </p>
            </Step>
            <Step step={steps[3]}>
                <p>
                    Book Advisor is a Full Stack <strong
                        class="text-violet-400">Python-Flask</strong
                    >,
                    <strong class="text-violet-400">React.js</strong
                    >
                    & <strong class="text-violet-400">MongoDB</strong> web application that offers personalized book recommendations based on users reading preferences.
                    Leveraging data from the New York Times Bestseller lists and integrating with the Google Books API, Book Advisor provides a seamless experience for discovering new reads. For testing you can use User: admin, Password: Admin-123.
                </p>
            </Step>
        </div>
    </section>
    <section
        id="about"
        class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
    >
        <div
            class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
        >
            <h6 class="text-large sm:text-xl md:text-2xl">
                Want to know more?
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                A bit <span class="poppins text-violet-400">about</span> me.
            </h3>
        </div>
        <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
            I am . . .
        </p>
        <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index}
                <div class="flex gap-6 sm:gap-8">
                    <p
                        class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold"
                    >
                        0{index + 1}
                    </p>
                    <div class="flex flex-col gap-6 sm:gap-8">
                        <h3 class="text-2xl sm:text-3xl md:text-5xl">
                            {benefit.name}
                        </h3>
                        <p>{benefit.description}</p>
                    </div>
                </div>
            {/each}
        </div>
        <!--
        <h5 class={" text-2xl sm:text-3xl font-semibold text-center poppins "}>
            The <span class="text-violet-400">Complete</span> Package
        </h5>
        <div
            class="flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full"
        >
            <table class="bg-white text-slate-700 rounded text-center">
                <thead class={"border-b border-solid border-slate-200  "}>
                    <tr class="">
                        <th />
                        <th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
                        <th
                            class="bg-violet-700 text-white whitespace-nowrap p-4 px-8"
                            >Me</th
                        >
                    </tr>
                </thead>
                <tbody>
                    <tr class="border-b border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Dedication</td
                        >
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr class="border-b border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Critical Thought</td
                        >
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr>
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Interpersonal Skills</td
                        >
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr class="border-t border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Progamming Ability</td
                        >
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                </tbody>
            </table>
        </div>
        <div class="mx-auto -mt-12 italic sm:hidden opacity-50">
            <p>Scroll to see more &rarr;</p>
        </div>
        <p class="mx-auto">So why not invest?</p>
    -->
    </section>
</main>
