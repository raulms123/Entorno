import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.io.IOException;
import java.io.PrintWriter;


public class TablaMultiplicarServlet extends HttpServlet {
    private static final long serialVersionUID = 1L;

    protected void doPost(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        String strNumero = request.getParameter("numero");
        int numero = Integer.parseInt(strNumero);

        response.setContentType("text/html");
        PrintWriter out = response.getWriter();

        out.println("<html><body>");
        out.println("<h2>Tabla de Multiplicar del " + numero + ":</h2>");
        out.println("<ul>");

        for (int i = 1; i <= 10; i++) {
            int resultado = numero * i;
            out.println("<li>" + numero + " x " + i + " = " + resultado + "</li>");
        }

        out.println("</ul>");
        out.println("</body></html>");
    }
}
