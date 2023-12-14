import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.io.IOException;
import java.io.PrintWriter;


public class DiaSemanaServlet extends HttpServlet {
    private static final long serialVersionUID = 1L;

    protected void doPost(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        String strNumero = request.getParameter("numero");
        int numero = Integer.parseInt(strNumero);

        String[] diasSemana = {"", "Lunes", "Martes", "Miércoles", "Jueves", "Viernes", "Sábado", "Domingo"};

        response.setContentType("text/html");
        PrintWriter out = response.getWriter();

        out.println("<html><body>");
        if (numero >= 1 && numero <= 7) {
            out.println("<h2>El día correspondiente es: " + diasSemana[numero] + "</h2>");
        } else {
            out.println("<h2>Por favor, ingrese un número del 1 al 7.</h2>");
        }
        out.println("</body></html>");
    }
}
