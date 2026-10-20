package com.servlet;

import java.io.IOException;
import jakarta.servlet.ServletException;
import jakarta.servlet.annotation.WebServlet;
import jakarta.servlet.http.*;

@WebServlet("/hello")
public class HelloServlet extends HttpServlet {

    @Override
    protected void doPost(HttpServletRequest request,
                          HttpServletResponse response)
            throws ServletException, IOException {

        request.setAttribute("name",
                request.getParameter("name"));

        request.setAttribute("email",
                request.getParameter("email"));

        request.setAttribute("course",
                request.getParameter("course"));

        request.setAttribute("age",
                request.getParameter("age"));

        request.getRequestDispatcher("result.jsp")
               .forward(request, response);
    }
}
