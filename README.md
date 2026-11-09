# UT5 · Seguimiento de clases

Repositorio de la **Unidad de Trabajo 5 (UT5)** con material de clase, códigos de ejemplo, prácticas y actividades.

## 🎯 Objetivos
* Organizar y centralizar el material de clase.
* Facilitar el estudio mediante ejemplos y ejercicios.
* Aprender el flujo de trabajo con **Git** y **GitHub** (forks, clonación, sincronización).

## 📁 Organización
* **Sesiones de clase:** Material y código desarrollado por sesiones.
* **Ejercicios:** Prácticas y actividades evaluables.

```text
UT5/
├── Sesiones de clase/
└── Ejercicios/
```

---

## 1. Crear tu copia (Fork)
1. Accede al repositorio original: [https://github.com/luis-gongom/UT5](https://github.com/luis-gongom/UT5)
2. Inicia sesión en GitHub y haz clic en **Fork** (arriba a la derecha) para copiarlo a tu cuenta personal.

---

## 2. Descargar en tu ordenador
1. Copia la URL HTTPS de tu fork (`https://github.com/TU-USUARIO/UT5.git`).
2. Abre la terminal en Visual Studio Code y clona el repositorio:
   ```bash
   git clone https://github.com/TU-USUARIO/UT5.git
   ```
3. Entra a la carpeta y abre el proyecto:
   ```bash
   cd UT5
   code .
   ```

---

## 3. Configurar el repositorio del profesor (`upstream`)
Vincula tu copia local con el repositorio original para recibir actualizaciones futuras:
```bash
git remote add upstream https://github.com/luis-gongom/UT5.git
git remote -v
```

---

## 4. Actualizar el material
Para incorporar nuevos contenidos publicados por el profesor:
```bash
git status
git add . && git commit -m "Guardar cambios locales" # (Opcional si tienes cambios propios)
git fetch upstream
git switch main
git merge upstream/main
git push origin main
```

---

## 5. Trabajar en varios equipos
Al terminar de trabajar en un equipo, sube siempre tus progresos a GitHub:
```bash
git add .
git commit -m "Describe los cambios realizados"
git push origin main
```
