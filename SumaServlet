import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.io.IOException;
import java.io.PrintWriter;


public class SumaAcumulativaServlet extends HttpServlet {
    private static final long serialVersionUID = 1L;

    protected void doPost(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        String strNumeroN = request.getParameter("numeroN");
        int numeroN = Integer.parseInt(strNumeroN);

        int sumaAcumulativa = 0;

        for (int i = 1; i <= numeroN; i++) {
            sumaAcumulativa += i;
        }

        response.setContentType("text/html");
        PrintWriter out = response.getWriter();

        out.println("<html><body>");
        out.println("<h2>La suma acumulativa hasta " + numeroN + " es: " + sumaAcumulativa + "</h2>");
        out.println("</body></html>");
    }
}
