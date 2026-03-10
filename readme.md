// ============================================
// PROYECTO SEMANA 02: Ficha de Datos del Dominio
// ============================================
//
// 🎯 OBJETIVO: Crear una ficha de datos en consola
//    usando variables, tipos y conversiones.
//
// 📋 TU DOMINIO: Reemplaza cada TODO con datos
//    coherentes con el dominio que te fue asignado.
//
// ⚠️  POLÍTICA ANTICOPIA: Tu implementación debe ser
//    única y coherente con tu dominio asignado.
//    Implementaciones copiadas serán detectadas.
//
// Adapta cada TODO al contexto de tu dominio asignado.
// Los ejemplos en este archivo usan dominios NO asignables.
// ============================================

// ============================================
// SECCIÓN 1: DATOS PRINCIPALES
// ============================================

// TODO: Reemplaza "sistema de gestion bibliotecas publicas" con el nombre de tu dominio
const DOMAIN_NAME = "sistema de gestion para bibiliotecas publicas";
//
// 📋 TU DOMINIO: Gestión de Préstamos Biblioteca Jhoan
// ============================================

// ============================================
// SECCIÓN 1: DATOS PRINCIPALES
// ============================================

const DOMAIN_NAME = "Gestión de Préstamos - Biblioteca Jhoan";

// Nombre del ejemplar (Libro/Recurso)
const itemName = "Clean Code: A Handbook of Agile Software Craftsmanship"; 

// Categoría del material
const itemCategory = "Programación - Desarrollo de Software";

// Peso del archivo digital en Megabytes (o número de páginas si es físico)
const itemQuantity = 464.5; 

// ¿Está el libro disponible para préstamo inmediato?
const isItemAvailable = false; 

// Estado de devolución (se inicia como null hasta que el bibliotecario lo asigne)
let returnStatus = null; 


// ============================================
// SECCIÓN 2: MOSTRAR FICHA DE DATOS
// ============================================
console.log("=========================================");
console.log(`FICHA DE DATOS: ${DOMAIN_NAME}`);
console.log("=========================================");
console.log("");

console.log(`Recurso:      ${itemName}`);
console.log(`Categoría:    ${itemCategory}`);
console.log(`Extensión:    ${itemQuantity} pp/MB`);
console.log(`Disponible:   ${isItemAvailable ? "Sí" : "No"}`);
console.log("");


// ============================================
// SECCIÓN 3: VERIFICACIÓN DE TIPOS CON typeof
// ============================================
console.log("--- Tipos de datos ---");

console.log("typeof itemName:        ", typeof itemName);
console.log("typeof itemQuantity:    ", typeof itemQuantity);
console.log("typeof isItemAvailable: ", typeof isItemAvailable);
console.log("");


// ============================================
// SECCIÓN 4: CONVERSIONES EXPLÍCITAS
// ============================================
console.log("--- Conversiones ---");

// Convertimos la extensión (Number) a String para generar una etiqueta de inventario
const sizeAsText = String(itemQuantity);
console.log("Extensión como texto para reporte:", sizeAsText);
console.log("typeof (convertido):", typeof sizeAsText);

// Ejemplo de conversión de String a Number (Simulando entrada de ID de estantería)
const stringShelf = "102";
const shelfAsNumber = Number(stringShelf);
console.log(`Ubicación convertida (Estantería): # ${shelfAsNumber}`);

console.log("");


// ============================================
// SECCIÓN 5: VALOR NULL
// ============================================
console.log("--- Valor nulo ---");

console.log("Estado de devolución pendiente:", returnStatus);
// Recordatorio: typeof null devuelve "object" por un comportamiento histórico de JS
console.log("typeof returnStatus:", typeof returnStatus); 
console.log("¿El estado es nulo?:", returnStatus === null); 

console.log("");


// ============================================
// CIERRE
// ============================================
console.log("=========================================");
console.log("FIN DE FICHA - SISTEMA JHOAN-DEV");
console.log("=========================================");
