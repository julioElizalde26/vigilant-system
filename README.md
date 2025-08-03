import React from 'react';
import { Lightbulb, TrendingUp, Users, Mail, Phone } from 'lucide-react';

// MIT License
//
// Copyright (c) 2024 Your Name Here
//
// Permission is hereby granted, free of charge, to any person obtaining a copy
// of this software and associated documentation files (the "Software"), to deal
// in the Software without restriction, including without limitation the rights
// to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
// copies of the Software, and to permit persons to whom the Software is
// furnished to do so, subject to the following conditions:
//
// The above copyright notice and this permission notice shall be included in all
// copies or substantial portions of the Software.
//
// THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
// IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
// FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
// AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
// LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
// OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
// SOFTWARE.

// Main App component
const App = () => {
  return (
    <div className="min-h-screen bg-gray-50 font-sans text-gray-800 relative overflow-hidden">
      {/* Colorful background shapes */}
      <div className="shape shape-1 bg-purple-400 opacity-20"></div>
      <div className="shape shape-2 bg-pink-400 opacity-20"></div>
      <div className="shape shape-3 bg-blue-400 opacity-20"></div>
      <div className="shape shape-4 bg-yellow-400 opacity-20"></div>
      <div className="shape shape-5 bg-green-400 opacity-20"></div>

      {/* Navbar */}
      <header className="bg-white shadow-sm p-4 sticky top-0 z-50">
        <nav className="container mx-auto flex justify-between items-center">
          <div className="text-2xl font-bold text-indigo-600">
            TuMarcaDigital
          </div>
          <div className="hidden md:flex space-x-6">
            <a href="#inicio" className="text-gray-600 hover:text-indigo-600 transition-colors">Inicio</a>
            <a href="#nosotros" className="text-gray-600 hover:text-indigo-600 transition-colors">Nosotros</a>
            <a href="#servicios" className="text-gray-600 hover:text-indigo-600 transition-colors">Servicios</a>
            <a href="#contacto" className="text-gray-600 hover:text-indigo-600 transition-colors">Contacto</a>
          </div>
          {/* Mobile menu button - placeholder for now */}
          <button className="md:hidden text-gray-600 hover:text-indigo-600">
            <svg className="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
              <path strokeLinecap="round" strokeLinejoin="round" strokeWidth="2" d="M4 6h16M4 12h16M4 18h16"></path>
            </svg>
          </button>
        </nav>
      </header>

      {/* Hero Section */}
      <section id="inicio" className="relative bg-gradient-to-r from-indigo-500 to-purple-600 text-white py-20 md:py-32 overflow-hidden">
        {/* Triangular diffused shapes */}
        <div className="triangle-diffuse top-left"></div>
        <div className="triangle-diffuse bottom-right"></div>

        <div className="container mx-auto px-4 text-center relative z-10">
          <h1 className="text-4xl md:text-6xl font-extrabold leading-tight mb-6 animate-fade-in-up">
            Impulsa tu Negocio con <span className="text-yellow-300">Marketing Digital Innovador</span>
          </h1>
          <p className="text-lg md:text-xl mb-10 max-w-3xl mx-auto animate-fade-in-up delay-200">
            Somos una startup que transforma la visibilidad de PYMES en ventas reales a través de estrategias digitales de vanguardia.
          </p>
          <a
            href="#contacto"
            className="inline-block bg-white text-indigo-600 font-bold py-3 px-8 rounded-full shadow-lg hover:bg-gray-100 transition-transform transform hover:scale-105 animate-fade-in-up delay-400"
          >
            ¡Hablemos de tu crecimiento!
          </a>
        </div>
      </section>

      {/* About Us Section */}
      <section id="nosotros" className="relative py-16 md:py-24 bg-white overflow-hidden">
        <div className="container mx-auto px-4 flex flex-col md:flex-row items-center gap-12 animate-fade-in-up relative z-10">
          <div className="md:w-1/2">
            <h2 className="text-3xl md:text-4xl font-bold text-indigo-700 mb-6">
              Nuestra Misión: Innovar para tu Éxito
            </h2>
            <p className="text-lg text-gray-700 mb-4">
              En <span className="font-semibold">TuMarcaDigital</span>, nacimos como una startup con la visión de revolucionar el marketing para pequeñas y medianas empresas. Entendemos los desafíos que enfrentan y por eso, nos dedicamos a ofrecer soluciones digitales creativas y efectivas.
            </p>
            <p className="text-lg text-gray-700">
              Nuestro equipo está compuesto por expertos apasionados por la innovación y el crecimiento. Buscamos constantemente las últimas tendencias y tecnologías para asegurar que tu negocio no solo sea visible, sino que también prospere en el competitivo mundo digital.
            </p>
          </div>
          <div className="md:w-1/2 flex justify-center items-center">
            <Lightbulb className="w-32 h-32 text-indigo-500 animate-bounce-slow" />
          </div>
        </div>
      </section>

      {/* Services Section */}
      <section id="servicios" className="py-16 md:py-24 bg-gray-100">
        <div className="container mx-auto px-4 text-center">
          <h2 className="text-3xl md:text-4xl font-bold text-indigo-700 mb-12 animate-fade-in-up">
            Nuestros Servicios de Marketing Digital
          </h2>
          <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 animate-fade-in-up delay-200">
            {/* Service Card 1: Estrategias SEO Avanzadas */}
            <div className="service-card-container">
              <div className="service-card-inner">
                <div className="service-card-front bg-white p-8 rounded-xl shadow-md">
                  <TrendingUp className="w-16 h-16 text-indigo-500 mx-auto mb-6" />
                  <h3 className="text-xl font-semibold text-gray-900 mb-4">Estrategias SEO Avanzadas</h3>
                </div>
                <div className="service-card-back bg-white p-8 rounded-xl shadow-md">
                  <h3 className="text-xl font-semibold text-gray-900 mb-4">Estrategias SEO Avanzadas</h3>
                  <p className="text-gray-600">
                    Implementamos estrategias de SEO avanzadas, como el **Link Building**, para mejorar el posicionamiento de tu página o empresa en buscadores, asegurando una mayor visibilidad y alcance para tu público objetivo.
                  </p>
                </div>
              </div>
            </div>
            {/* Service Card 2: Gestión de Redes Sociales */}
            <div className="service-card-container">
              <div className="service-card-inner">
                <div className="service-card-front bg-white p-8 rounded-xl shadow-md">
                  <Users className="w-16 h-16 text-green-500 mx-auto mb-6" />
                  <h3 className="text-xl font-semibold text-gray-900 mb-4">Gestión de Redes Sociales</h3>
                </div>
                <div className="service-card-back bg-white p-8 rounded-xl shadow-md">
                  <h3 className="text-xl font-semibold text-gray-900 mb-4">Gestión de Redes Sociales</h3>
                  <p className="text-gray-600">
                    Ofrecemos un servicio completo de gestión de redes sociales a través de la creación y publicación de **contenido estratégico y atractivo**, fomentando la interacción y el crecimiento de tu comunidad online.
                  </p>
                </div>
              </div>
            </div>
            {/* Service Card 3: Publicidad Digital (SEM) */}
            <div className="service-card-container">
              <div className="service-card-inner">
                <div className="service-card-front bg-white p-8 rounded-xl shadow-md">
                  <Lightbulb className="w-16 h-16 text-yellow-500 mx-auto mb-6" />
                  <h3 className="text-xl font-semibold text-gray-900 mb-4">Publicidad Digital (SEM)</h3>
                </div>
                <div className="service-card-back bg-white p-8 rounded-xl shadow-md">
                  <h3 className="text-xl font-semibold text-gray-900 mb-4">Publicidad Digital (SEM)</h3>
                  <p className="text-gray-600">
                    Llevamos a cabo la **gestión de campañas de comerciales** y publicidad pagada a través de aplicaciones de búsqueda como **Google Ads**, garantizando resultados rápidos y una visibilidad inmediata para tu marca.
                  </p>
                </div>
              </div>
            </div>
            {/* Service Card 4: Email Marketing */}
            <div className="service-card-container">
              <div className="service-card-inner">
                <div className="service-card-front bg-white p-8 rounded-xl shadow-md">
                  <Mail className="w-16 h-16 text-red-500 mx-auto mb-6" />
                  <h3 className="text-xl font-semibold text-gray-900 mb-4">Email Marketing</h3>
                </div>
                <div className="service-card-back bg-white p-8 rounded-xl shadow-md">
                  <h3 className="text-xl font-semibold text-gray-900 mb-4">Email Marketing</h3>
                  <p className="text-gray-600">
                    Diseñamos y ejecutamos **campañas de email marketing personalizadas** para enviar recordatorios o promociones a tus clientes en momentos estratégicos, optimizando la fidelización y las conversiones.
                  </p>
                </div>
              </div>
            </div>
            {/* Service Card 5: Desarrollo Web & Landing Pages */}
            <div className="service-card-container">
              <div className="service-card-inner">
                <div className="service-card-front bg-white p-8 rounded-xl shadow-md">
                  <Phone className="w-16 h-16 text-blue-500 mx-auto mb-6" />
                  <h3 className="text-xl font-semibold text-gray-900 mb-4">Desarrollo Web & Landing Pages</h3>
                </div>
                <div className="service-card-back bg-white p-8 rounded-xl shadow-md">
                  <h3 className="text-xl font-semibold text-gray-900 mb-4">Desarrollo Web & Landing Pages</h3>
                  <p className="text-gray-600">
                    Creamos **páginas web y landing pages personalizadas** desde cero, implementando las estrategias de marketing digital antes mencionadas para asegurar una presencia online robusta y orientada a resultados.
                  </p>
                </div>
              </div>
            </div>
            {/* Service Card 6: Marketing de Contenidos */}
            <div className="service-card-container">
              <div className="service-card-inner">
                <div className="service-card-front bg-white p-8 rounded-xl shadow-md">
                  <Lightbulb className="w-16 h-16 text-purple-500 mx-auto mb-6" />
                  <h3 className="text-xl font-semibold text-gray-900 mb-4">Marketing de Contenidos</h3>
                </div>
                <div className="service-card-back bg-white p-8 rounded-xl shadow-md">
                  <h3 className="text-xl font-semibold text-gray-900 mb-4">Marketing de Contenidos</h3>
                  <p className="text-gray-600">
                    Desarrollamos **contenido de alta calidad y relevante** directamente relacionado con la marca en cuestión, diseñado para atraer y captar la atención de clientes interesados, impulsando el engagement y la lealtad.
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* Call to Action Section */}
      <section className="bg-indigo-600 text-white py-16 md:py-20 text-center">
        <div className="container mx-auto px-4 animate-fade-in-up">
          <h2 className="text-3xl md:text-4xl font-bold mb-6">
            ¿Listo para llevar tu negocio al siguiente nivel?
          </h2>
          <p className="text-lg md:text-xl mb-8 max-w-2xl mx-auto">
            Contacta con nosotros hoy mismo para una consulta gratuita y descubre cómo podemos ayudarte a crecer.
          </p>
          <a
            href="#contacto"
            className="inline-block bg-white text-indigo-600 font-bold py-3 px-8 rounded-full shadow-lg hover:bg-gray-100 transition-transform transform hover:scale-105"
          >
            ¡Contáctanos Ahora!
          </a>
        </div>
      </section>

      {/* Contact Section */}
      <section id="contacto" className="py-16 md:py-24 bg-white">
        <div className="container mx-auto px-4">
          <h2 className="text-3xl md:text-4xl font-bold text-indigo-700 text-center mb-12 animate-fade-in-up">
            Ponte en Contacto
          </h2>
          <div className="flex flex-col md:flex-row gap-12 items-center animate-fade-in-up delay-200">
            <div className="md:w-1/2 bg-gray-50 p-8 rounded-xl shadow-md">
              <form className="space-y-6">
                <div>
                  <label htmlFor="name" className="block text-sm font-medium text-gray-700">Nombre Completo</label>
                  <input
                    type="text"
                    id="name"
                    name="name"
                    className="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500"
                    placeholder="Tu Nombre"
                  />
                </div>
                <div>
                  <label htmlFor="email" className="block text-sm font-medium text-gray-700">Correo Electrónico</label>
                  <input
                    type="email"
                    id="email"
                    name="email"
                    className="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500"
                    placeholder="tu.correo@ejemplo.com"
                  />
                </div>
                <div>
                  <label htmlFor="message" className="block text-sm font-medium text-gray-700">Mensaje</label>
                  <textarea
                    id="message"
                    name="message"
                    rows="4"
                    className="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500"
                    placeholder="Cuéntanos sobre tu proyecto..."
                  ></textarea>
                </div>
                <button
                  type="submit"
                  className="w-full bg-indigo-600 text-white font-bold py-3 px-6 rounded-md shadow-lg hover:bg-indigo-700 transition-colors transform hover:scale-105"
                >
                  Enviar Mensaje
                </button>
              </form>
            </div>
            <div className="md:w-1/2 space-y-8 text-center md:text-left">
              {/* Phone Number */}
              <div className="flex items-center justify-center md:justify-start space-x-4">
                <Phone className="w-8 h-8 text-indigo-600" />
                <span className="text-lg text-gray-700">+52 6681468067</span>
              </div>
              {/* Email Address */}
              <div className="flex items-center justify-center md:justify-start space-x-4">
                <Mail className="w-8 h-8 text-indigo-600" />
                <span className="text-lg text-gray-700">visionatuempresa@gmail.com</span>
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* Footer */}
      <footer className="bg-gray-800 text-white py-8">
        <div className="container mx-auto px-4 text-center text-sm">
          <p>&copy; {new Date().getFullYear()} TuMarcaDigital. Todos los derechos reservados.</p>
          <div className="mt-4 space-x-4">
            <a href="#" className="hover:text-indigo-400 transition-colors">Política de Privacidad</a>
            <a href="#" className="hover:text-indigo-400 transition-colors">Términos de Servicio</a>
          </div>
        </div>
      </footer>

      {/* Tailwind CSS CDN and custom styles */}
      <style>{`
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&display=swap');
        body {
          font-family: 'Inter', sans-serif;
        }
        .bg-pattern {
          /* This was removed as per user request for more abstract shapes */
        }
        @keyframes fade-in-up {
          from {
            opacity: 0;
            transform: translateY(20px);
          }
          to {
            opacity: 1;
            transform: translateY(0);
          }
        }
        .animate-fade-in-up {
          animation: fade-in-up 0.8s ease-out forwards;
          opacity: 0; /* Start hidden */
        }
        .animate-fade-in-up.delay-200 { animation-delay: 0.2s; }
        .animate-fade-in-up.delay-400 { animation-delay: 0.4s; }

        @keyframes bounce-slow {
          0%, 100% {
            transform: translateY(0);
          }
          50% {
            transform: translateY(-10px);
          }
        }
        .animate-bounce-slow {
          animation: bounce-slow 3s infinite ease-in-out;
        }

        /* Card Flip Styles */
        .service-card-container {
          perspective: 1000px; /* Needed for 3D effect */
          height: 250px; /* Fixed height to prevent layout shift */
          width: 100%; /* Ensure it takes full width of grid column */
          cursor: pointer; /* Indicate it's interactive */
          transition: transform 0.3s ease-in-out, box-shadow 0.3s ease-in-out; /* Add transition for lift and shadow */
        }

        .service-card-container:hover {
          transform: translateY(-5px); /* Lift slightly on hover */
          box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2); /* More pronounced shadow */
        }

        .service-card-inner {
          position: relative;
          width: 100%;
          height: 100%;
          text-align: center;
          transition: transform 0.6s; /* Smooth transition for flip */
          transform-style: preserve-3d; /* Keep children in 3D space */
        }

        .service-card-container:hover .service-card-inner {
          transform: rotateY(180deg); /* Flip on hover */
        }

        .service-card-front, .service-card-back {
          position: absolute;
          width: 100%;
          height: 100%;
          -webkit-backface-visibility: hidden; /* Hide back of the element when facing away */
          backface-visibility: hidden;
          display: flex;
          flex-direction: column;
          justify-content: center;
          align-items: center;
          padding: 2rem; /* Consistent padding */
          box-sizing: border-box; /* Include padding in width/height */
          border-radius: 0.75rem; /* Ensure rounded corners on both sides */
        }

        .service-card-front {
          background-color: #ffffff; /* Explicitly white for front */
        }

        .service-card-back {
          transform: rotateY(180deg); /* Initially rotated to be hidden */
          background-color: #e0e7ff; /* A lighter indigo/blue for contrast (Tailwind indigo-100) */
          color: #3730a3; /* Darker indigo text for readability (Tailwind indigo-800) */
        }

        /* Colorful Shapes */
        .shape {
          position: absolute;
          border-radius: 50%; /* Default to circle */
          filter: blur(80px); /* Soft blur effect */
          z-index: 0; /* Ensure they are behind content */
          animation: float 10s infinite ease-in-out alternate; /* Subtle floating animation */
        }

        .shape-1 {
          width: 200px;
          height: 200px;
          top: 10%;
          left: -5%;
          animation-duration: 12s;
        }
        .shape-2 {
          width: 150px;
          height: 150px;
          top: 40%;
          right: -5%;
          animation-duration: 10s;
        }
        .shape-3 {
          width: 250px;
          height: 250px;
          bottom: 5%;
          left: 20%;
          animation-duration: 14s;
          border-radius: 30%; /* More square-like */
          transform: rotate(45deg);
        }
        .shape-4 {
          width: 100px;
          height: 100px;
          top: 25%;
          right: 15%;
          animation-duration: 8s;
          border-radius: 60% 40% 30% 70% / 60% 30% 70% 40%; /* Blob-like shape */
        }
        .shape-5 {
          width: 180px;
          height: 180px;
          bottom: 15%;
          right: 10%;
          animation-duration: 11s;
          border-radius: 40% 60% 70% 30% / 50% 60% 40% 50%; /* Another blob */
        }

        @keyframes float {
          0% { transform: translate(0, 0) rotate(0deg); }
          25% { transform: translate(10px, -10px) rotate(5deg); }
          50% { transform: translate(0, 10px) rotate(0deg); }
          75% { transform: translate(-10px, -5px) rotate(-5deg); }
          100% { transform: translate(0, 0) rotate(0deg); }
        }

        /* Triangular Diffused Shapes for Hero Section */
        .triangle-diffuse {
          position: absolute;
          width: 300px; /* Adjust size as needed */
          height: 300px; /* Adjust size as needed */
          background: linear-gradient(to bottom right, rgba(139, 92, 246, 0.6), rgba(167, 139, 250, 0)); /* Purple gradient */
          filter: blur(100px); /* Strong blur for diffusion */
          z-index: 0; /* Behind content */
        }

        .triangle-diffuse.top-left {
          top: -100px;
          left: -100px;
          transform: rotate(45deg); /* Rotate to form a corner triangle */
          clip-path: polygon(0 0, 100% 0, 0 100%); /* Top-left triangle */
        }

        .triangle-diffuse.bottom-right {
          bottom: -100px;
          right: -100px;
          transform: rotate(45deg); /* Rotate to form a corner triangle */
          clip-path: polygon(100% 0, 100% 100%, 0 100%); /* Bottom-right triangle */
        }
      `}</style>
      <script src="https://cdn.tailwindcss.com"></script>
    </div>
  );
};

export default App;
