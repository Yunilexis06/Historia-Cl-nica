class Paciente {
    String CI;
    String nombre;
    String apellidos;
    Date fechaNacimiento;
    String sexo;
    double peso;
    double estatura;
    String direccion;
    List<Imagen> imagenes;
    List<Enfermedad> enfermedades;
    
    void buscarPaciente(String CI) {}
    void obtenerPacientesMayorEstatura() {}
    void obtenerPacientesFemeninoDengue() {}
    void ordenarPacientesPorNombre() {}
    void ordenarPacientesPorPeso() {}
    void agregarPaciente() {}
    void eliminarPaciente() {}
    void modificarPaciente() {}
}

class Imagen {
    String tipo;
    Date fechaRealizacion;
    String descripcion;
    
    void agregarImagen() {}
    void eliminarImagen() {}
    void modificarImagen() {}
}

class Enfermedad {
    String nombre;
    Date fechaDiagnostico;
    String tratamiento;
    
    void agregarEnfermedad() {}
    void eliminarEnfermedad() {}
    void modificarEnfermedad() {}
}

class Hospital {
    List<Paciente> pacientes;
    
    void buscarPaciente(String CI) {}
    void obtenerPacientesMayorEstatura() {}
    void obtenerPacientesFemeninoDengue() {}
    void ordenarPacientesPorNombre() {}
    void ordenarPacientesPorPeso() {}
    void agregarPaciente(Paciente p) {}
    void eliminarPaciente(String CI) {}
    void modificarPaciente(Paciente p) {}
}
Paciente "1" -- "0..*" Imagen : tiene >
Paciente "1" -- "0..*" Enfermedad : tiene >
Hospital "1" -- "0..*" Paciente : tiene >

@enduml
