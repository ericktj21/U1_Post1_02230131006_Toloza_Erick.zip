Violación de SRP (Single Responsibility): La clase OrderManager hace demasiadas cosas: crea pedidos, calcula descuentos, guarda en archivos de texto y envía notificaciones simuladas .

Violación de OCP (Open/Closed): Los descuentos están "quemados" en el código con if (total > 1000) e if (total > 5000) . Si quisieras agregar un descuento por Navidad, tendrías que modificar esta clase.

Violación de DIP (Dependency Inversion): La clase depende directamente de la implementación concreta java.io.FileWriter  en lugar de depender de una abstracción o interfaz para guardar los datos.

Violación de SRP / Acoplamiento: La notificación por correo está forzada usando un System.out.println directamente dentro del método de creación.
