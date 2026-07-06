<template lang="pug">
  .curso-main-container.pb-3
    BannerInterno(icono="far fa-question-circle" titulo="Actividad didáctica")
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5
  
      #Actividad                
        <ActividadController :cuestionario="cuestionario"/>
  
  </template>

<script>
import ActividadController from '@ecored-sena/base-kit/plugin/components/actividad/ActividadController.vue'
export default {
  name: 'ActividadDidactica',
  components: {
    ActividadController,
  },
  data: () => ({
    cuestionario: {
      tema: 'La postventa',
      titulo: 'Cuestionario',
      introduccion:
        '<b> Objetivo:</b> verificar la comprensión de los conceptos fundamentales del servicio postventa en el contexto comercial.',
      titulo_aprobado: '¡BUEN TRABAJO!',
      titulo_reprobado: 'VUELVA A INTENTARLO',
      barajarPreguntas: true,
      preguntas: [
        {
          id: 1,
          texto: '¿Qué es la postventa?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Un proceso de fabricación de productos.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Conjunto de actividades realizadas después de la venta para garantizar la satisfacción del cliente.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Una estrategia de publicidad.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Un sistema de distribución.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la postventa.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo la postventa.',
        },
        {
          id: 2,
          texto: '¿Cuál es la principal importancia del servicio postventa?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Incrementar los costos operativos.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Reducir la comunicación con los clientes.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Fortalecer la satisfacción, fidelización y confianza del cliente.',
              esCorrecta: true,
            },
            { id: 'd', texto: 'Limitar las garantías.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la postventa.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo la postventa.',
        },
        {
          id: 3,
          texto: '¿Cuál de los siguientes corresponde a un servicio postventa?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Producción de bienes.', esCorrecta: false },
            { id: 'b', texto: 'Gestión contable.', esCorrecta: false },
            { id: 'c', texto: 'Soporte técnico.', esCorrecta: true },
            { id: 'd', texto: 'Selección de proveedores.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la postventa.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo la postventa.',
        },
        {
          id: 4,
          texto: '¿Qué se busca mediante la fidelización en la postventa?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Lograr que el cliente mantenga una relación duradera con la empresa.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Aumentar los precios de los productos.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Reducir los servicios ofrecidos.',
              esCorrecta: false,
            },
            { id: 'd', texto: 'Disminuir la comunicación.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la postventa.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo la postventa.',
        },
        {
          id: 5,
          texto: '¿Qué significa retener clientes?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Limitar sus opciones de compra.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Mantener a los clientes comprando y vinculados con la empresa.',
              esCorrecta: true,
            },
            { id: 'c', texto: 'Evitar nuevas ventas.', esCorrecta: false },
            { id: 'd', texto: 'Suspender la atención.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la postventa.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo la postventa.',
        },
        {
          id: 6,
          texto: '¿Cuál es una etapa de la postventa?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Producción.', esCorrecta: false },
            { id: 'b', texto: 'Distribución.', esCorrecta: false },
            { id: 'c', texto: 'Facturación.', esCorrecta: false },
            { id: 'd', texto: 'Fidelización.', esCorrecta: true },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la postventa.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo la postventa.',
        },
        {
          id: 7,
          texto: '¿Cuál es uno de los elementos de la postventa?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Fabricación de productos.', esCorrecta: false },
            { id: 'b', texto: 'Atención al cliente.', esCorrecta: true },
            { id: 'c', texto: 'Planeación financiera.', esCorrecta: false },
            { id: 'd', texto: 'Gestión tributaria.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la postventa.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo la postventa.',
        },
        {
          id: 8,
          texto: '¿Qué función cumple el seguimiento de la venta?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Eliminar el contacto con el cliente.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Reducir la satisfacción del usuario.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Verificar que el producto o servicio cumpla las expectativas del cliente.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Finalizar toda comunicación.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la postventa.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo la postventa.',
        },
        {
          id: 9,
          texto: '¿Qué son las devoluciones dentro de la postventa?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Estrategias publicitarias.', esCorrecta: false },
            { id: 'b', texto: 'Métodos de distribución.', esCorrecta: false },
            { id: 'c', texto: 'Técnicas de negociación.', esCorrecta: false },
            {
              id: 'd',
              texto:
                'Procesos mediante los cuales el cliente retorna un producto por inconformidad o defectos.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la postventa.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo la postventa.',
        },
        {
          id: 10,
          texto: '¿Qué beneficio genera la recompra?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Incrementa la rentabilidad y fortalece la relación con el cliente.',
              esCorrecta: true,
            },
            { id: 'b', texto: 'Disminuye la lealtad.', esCorrecta: false },
            {
              id: 'c',
              texto: 'Reduce las oportunidades de negocio.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Elimina la necesidad de atención.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la postventa.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo la postventa.',
        },
        {
          id: 11,
          texto: '¿Qué implica la gestión de compras en la postventa?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Diseñar campañas de publicidad.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Gestionar inventarios exclusivamente.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Atender procesos relacionados con adquisiciones y requerimientos posteriores del cliente.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Elaborar contratos laborales.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la postventa.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo la postventa.',
        },
        {
          id: 12,
          texto: '¿Cuál es la función de una garantía?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Incrementar el precio del producto.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Respaldar al cliente frente a defectos o fallas del producto o servicio.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Sustituir el servicio al cliente.',
              esCorrecta: false,
            },
            { id: 'd', texto: 'Eliminar las devoluciones.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la postventa.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo la postventa.',
        },
        {
          id: 13,
          texto: '¿Qué es el soporte técnico?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Una estrategia de ventas.', esCorrecta: false },
            { id: 'b', texto: 'Un método de promoción.', esCorrecta: false },
            {
              id: 'c',
              texto:
                'Asistencia especializada para solucionar problemas relacionados con un producto o servicio.',
              esCorrecta: true,
            },
            { id: 'd', texto: 'Un proceso de producción.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la postventa.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo la postventa.',
        },
        {
          id: 14,
          texto: '¿Qué es el feedback en la postventa?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Una devolución obligatoria.',
              esCorrecta: false,
            },
            { id: 'b', texto: 'Un descuento comercial.', esCorrecta: false },
            {
              id: 'c',
              texto:
                'La retroalimentación proporcionada por el cliente sobre su experiencia.',
              esCorrecta: true,
            },
            { id: 'd', texto: 'Una garantía extendida.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la postventa.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo la postventa.',
        },
        {
          id: 15,
          texto:
            '¿Qué propósito tienen los descuentos y promociones postventa?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Eliminar la competencia.', esCorrecta: false },
            {
              id: 'b',
              texto: 'Reducir la calidad del servicio.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Incrementar las reclamaciones.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Incentivar nuevas compras y fortalecer la fidelización.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la postventa.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo la postventa.',
        },
        {
          id: 16,
          texto:
            '¿Cuál es la primera etapa del proceso de calidad del servicio postventa?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Planificar.', esCorrecta: true },
            { id: 'b', texto: 'Implantar.', esCorrecta: false },
            { id: 'c', texto: 'Controlar.', esCorrecta: false },
            { id: 'd', texto: 'Mejorar.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la postventa.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo la postventa.',
        },
        {
          id: 17,
          texto:
            '¿Qué actividad corresponde a la fase de control en la calidad del servicio postventa?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Diseñar nuevos productos.', esCorrecta: false },
            {
              id: 'b',
              texto: 'Realizar campañas publicitarias.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Verificar el cumplimiento de los estándares establecidos.',
              esCorrecta: true,
            },
            { id: 'd', texto: 'Contratar personal.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la postventa.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo la postventa.',
        },
        {
          id: 18,
          texto: '¿Qué se busca en la fase de mejora del servicio postventa?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Mantener los mismos errores.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Reducir la satisfacción del cliente.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Implementar acciones correctivas y de optimización continua.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Eliminar los procesos de evaluación.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la postventa.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo la postventa.',
        },
        {
          id: 19,
          texto:
            '¿Cuál es el primer paso para estructurar un servicio postventa?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Ofrecer descuentos.', esCorrecta: false },
            {
              id: 'b',
              texto: 'Recepción y atención de incidencias.',
              esCorrecta: true,
            },
            { id: 'c', texto: 'Realizar promociones.', esCorrecta: false },
            {
              id: 'd',
              texto: 'Ejecutar campañas publicitarias.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la postventa.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo la postventa.',
        },
        {
          id: 20,
          texto: '¿Qué función cumple un servicio de asistencia técnica?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Gestionar la nómina de empleados.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Diseñar estrategias de mercadeo.',
              esCorrecta: false,
            },
            { id: 'c', texto: 'Administrar inventarios.', esCorrecta: false },
            {
              id: 'd',
              texto:
                'Resolver problemas técnicos relacionados con productos o servicios adquiridos.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la postventa.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo la postventa.',
        },
      ],
      mensaje_final_aprobado:
        '¡Felicidades! Correctas sus respuestas, significa que ha comprendido la importancia del servicio postventa y su impacto en la fidelización de clientes. ¡Siga aplicando estos conocimientos en la práctica!',
      mensaje_final_reprobado:
        'No ha superado la actividad. Le recomendamos volver a revisar el componente formativo e intentar nuevamente la actividad didáctica.',
    },
  }),
}
</script>
