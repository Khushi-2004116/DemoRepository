package com.example.demowebsite;

import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;
import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RestController;

@SpringBootApplication
public class DemoWebsiteApplication {
    public static void main(String[] args) {
        SpringApplication.run(DemoWebsiteApplication.class, args);
    }
}

@RestController
class HelloController {
    @GetMapping("/")
    public String home() {
        return "Welcome to the Demo Website!";
    }
}
