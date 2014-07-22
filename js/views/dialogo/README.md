DialogoConfirmacionView
=======================
Es una vista que muestra un diálogo modal.
Requiere del template situado en [templates/dialogo/dialogo-confirmacion.html](../../../templates/dialogo-confirmacion.html).

Este diálogo es una adaptación de [Backbone.BootstrapModal](https://github.com/powmedia/backbone.bootstrap-modal#backbonebootstrapmodal) (pull [#58](https://github.com/powmedia/backbone.bootstrap-modal/pull/58), por lo que el modo de uso es el mismo.

Versión
-------
0.1


Ejemplo de uso
--------------
```
var dialogoConfirmacionView = new DialogoConfirmacionView({
	title:  "Confirmación requerida",
	content: mensajeConfirmacion,
	okText: "Confirmar",
	cancelText: "Cancelar"
});

dialogoConfirmacionView.open();

dialogoConfirmacionView.on('ok', function() {
	//Do some validation etc.
	console.log("Diálogo aceptado");
});
```

La propia ventana se encargará de cerrarse