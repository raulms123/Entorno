import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.io.IOException;
import java.io.PrintWriter;


public class MayorServlet extends HttpServlet {
    private static final long serialVersionUID = 1L;

    protected void doPost(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        String strNumero1 = request.getParameter("numero1");
        String strNumero2 = request.getParameter("numero2");
        String strNumero3 = request.getParameter("numero3");

        int numero1 = Integer.parseInt(strNumero1);
        int numero2 = Integer.parseInt(strNumero2);
        int numero3 = Integer.parseInt(strNumero3);

        int mayor = numero1;

        if (numero2 > mayor) {
            mayor = numero2;
        }

        if (numero3 > mayor) {
            mayor = numero3;
        }

        response.setContentType("text/html");
        PrintWriter out = response.getWriter();

        out.println("<html><body>");
        out.println("<h2>El número mayor es: " + mayor + "</h2>");
        out.println("</body></html>");
    }
}
