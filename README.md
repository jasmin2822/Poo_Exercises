using System;

namespace Practica2
{
    class Libro
    {
        public string Titulo { get; set; }
        public string Autor { get; set; }
        public int Paginas { get; set; }

        public Libro(string titulo, string autor, int paginas)
        {
            this.Titulo = titulo;
            this.Autor = autor;
            this.Paginas = paginas;
        }

        public void MostrarInformacion()
        {
            Console.WriteLine("Título: " + Titulo);
            Console.WriteLine("Autor: " + Autor);
            Console.WriteLine("Páginas: " + Paginas);
        }
    }

    class Program
    {
        static void Main(string[] args)
        {
            Libro miLibro = new Libro("El arte de la guerra", "Sun Tzu", 300);

            miLibro.MostrarInformacion();
        }
    }
}
