package com.bolsadeideas.springboot.di.app.controllers;

import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.stereotype.Controller;
import org.springframework.ui.Model;
import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RequestMapping;

import com.bolsadeideas.springboot.di.app.models.service.MiServicio;

@Controller
@RequestMapping("")
public class IndexController {
	
	//Para inyectar, metodo hollywood
	@Autowired 
	private MiServicio servicio;
	
	@GetMapping({"/","","/index"})
	public String index(Model model) {
		model.addAttribute("objeto",servicio.operacion());		
		return "index";
	}
	
}
