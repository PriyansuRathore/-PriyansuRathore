import { motion } from "framer-motion";
import { FaGithub, FaLinkedin, FaCode } from "react-icons/fa";
import { SiLeetcode } from "react-icons/si";

export default function AboutMe() {
  return (
    <section className="max-w-5xl mx-auto px-6 py-12 text-gray-100">
      {/* Heading */}
      <motion.h1
        initial={{ opacity: 0, y: -20 }}
        animate={{ opacity: 1, y: 0 }}
        transition={{ duration: 0.6 }}
        className="text-4xl font-bold mb-6 text-white"
      >
        👋 Hi, I'm <span className="text-blue-400">Priyansu Rathore</span>
      </motion.h1>

      {/* Intro */}
      <motion.p
        initial={{ opacity: 0 }}
        animate={{ opacity: 1 }}
        transition={{ duration: 0.8, delay: 0.2 }}
        className="text-lg leading-relaxed text-gray-300 mb-8 max-w-3xl"
      >
        A passionate{" "}
        <span className="font-semibold text-blue-400">Full-Stack Developer</span>{" "}
        and <span className="font-semibold text-blue-400">AI/ML enthusiast</span>.
        I build scalable web apps, intelligent systems, and seamless digital experiences.
        With <strong>400+ LeetCode problems</strong> solved, I bring strong problem-solving
        and clean engineering principles to everything I build.
      </motion.p>

      {/* Grid Section */}
      <div className="grid sm:grid-cols-2 gap-8">
        
        {/* Tech Stack Card */}
        <motion.div
          initial={{ opacity: 0, y: 30 }}
          whileInView={{ opacity: 1, y: 0 }}
          viewport={{ once: true }}
          transition={{ duration: 0.6 }}
          className="bg-gray-900/60 rounded-2xl p-6 shadow-lg border border-gray-800"
        >
          <h2 className="text-2xl font-semibold mb-4 text-blue-400">Tech Stack</h2>
          <ul className="space-y-2 text-gray-300">
            <li>⚡ React.js, Next.js, JavaScript, TypeScript</li>
            <li>🎨 Tailwind CSS, HTML5, CSS3, Redux Toolkit</li>
            <li>🛠 Node.js, Express.js, REST APIs</li>
            <li>🗄 MongoDB, MySQL, SQLite, Firebase</li>
            <li>🤖 Python, OpenCV, scikit-learn, NLP</li>
            <li>🧰 Git, GitHub, Postman, Vercel</li>
          </ul>
        </motion.div>

        {/* Languages Card */}
        <motion.div
          initial={{ opacity: 0, y: 30 }}
          whileInView={{ opacity: 1, y: 0 }}
          viewport={{ once: true }}
          transition={{ duration: 0.6 }}
          className="bg-gray-900/60 rounded-2xl p-6 shadow-lg border border-gray-800"
        >
          <h2 className="text-2xl font-semibold mb-4 text-blue-400">Languages</h2>
          <ul className="space-y-2 text-gray-300">
            <li>✔ JavaScript & TypeScript</li>
            <li>✔ Python</li>
            <li>✔ C++</li>
            <li>✔ SQL</li>
            <li>✔ HTML & CSS</li>
          </ul>
        </motion.div>
      </div>

      {/* Links Card */}
      <motion.div
        initial={{ opacity: 0, y: 30 }}
        whileInView={{ opacity: 1, y: 0 }}
        viewport={{ once: true }}
        transition={{ duration: 0.6, delay: 0.2 }}
        className="mt-10 bg-gray-900/60 rounded-2xl p-6 shadow-lg border border-gray-800"
      >
        <h2 className="text-2xl font-semibold mb-4 text-blue-400">Connect With Me</h2>
        <div className="flex items-center gap-6 text-2xl">
          <a href="https://github.com/PriyansuRathore" className="text-gray-300 hover:text-white">
            <FaGithub />
          </a>
          <a href="https://leetcode.com/u/Priyansu_Rathore7576/" className="text-gray-300 hover:text-yellow-400">
            <SiLeetcode />
          </a>
          <a href="https://www.linkedin.com/in/priyansu-rathore-43bb47253/" className="text-gray-300 hover:text-blue-500">
            <FaLinkedin />
          </a>
        </div>
      </motion.div>
    </section>
  );
}
