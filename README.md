<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Solicitud de Alquiler</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
            padding: 0;
            background-color: #f9f9f9;
        }
        form {
            max-width: 600px;
            margin: auto;
            padding: 20px;
            background: #fff;
            border: 1px solid #ddd;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }
        h1 {
            text-align: center;
        }
        .form-section {
            margin-bottom: 20px;
        }
        label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
        }
        input, textarea, select {
            width: 100%;
            padding: 8px;
            margin-bottom: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        .checkbox-group {
            margin-bottom: 15px;
        }
        .checkbox-group input {
            margin-right: 5px;
        }
        .submit-btn {
            display: block;
            width: 100%;
            padding: 10px;
            background-color: #28a745;
            color: #fff;
            font-size: 16px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        .submit-btn:hover {
            background-color: #218838;
        }
    </style>
</head>
<body>
    <form>
        <h1>Solicitud de Alquiler</h1>

        <div class="form-section">
            <h2>Propiedad</h2>
            <label for="propiedad">Propiedad</label>
            <input type="text" id="propiedad" name="propiedad" required>

            <label for="destino">Destino</label>
            <input type="text" id="destino" name="destino" required>

            <label for="direccion">Dirección</label>
            <input type="text" id="direccion" name="direccion" required>

            <label for="ciudad">Ciudad</label>
            <input type="text" id="ciudad" name="ciudad" required>

            <label for="precio">Precio (Gs.)</label>
            <input type="number" id="precio" name="precio" required>
        </div>

        <div class="form-section">
            <h2>Datos del Locatario/a</h2>
            <label for="nombre">Nombre y Apellido</label>
            <input type="text" id="nombre" name="nombre" required>

            <label for="nacionalidad">Nacionalidad</label>
            <input type="text" id="nacionalidad" name="nacionalidad" required>

            <label for="ruc">RUC</label>
            <input type="text" id="ruc" name="ruc">

            <label for="domicilio">Domicilio</label>
            <input type="text" id="domicilio" name="domicilio" required>

            <label for="ciudad-locatario">Ciudad</label>
            <input type="text" id="ciudad-locatario" name="ciudad-locatario" required>

            <label for="celular">Celular</label>
            <input type="text" id="celular" name="celular" required>

            <label for="actividad">Actividad</label>
            <input type="text" id="actividad" name="actividad" required>

            <label for="ingresos">Ingresos Mensuales</label>
            <input type="number" id="ingresos" name="ingresos" required>
        </div>

        <div class="form-section">
            <h2>Datos del Co-deudor/a</h2>
            <label for="nombre-codeudor">Nombre y Apellido</label>
            <input type="text" id="nombre-codeudor" name="nombre-codeudor" required>

            <label for="nacionalidad-codeudor">Nacionalidad</label>
            <input type="text" id="nacionalidad-codeudor" name="nacionalidad-codeudor" required>

            <label for="ci-codeudor">C.I. N.º</label>
            <input type="text" id="ci-codeudor" name="ci-codeudor" required>

            <label for="domicilio-codeudor">Domicilio Particular</label>
            <input type="text" id="domicilio-codeudor" name="domicilio-codeudor" required>

            <label for="ciudad-codeudor">Ciudad</label>
            <input type="text" id="ciudad-codeudor" name="ciudad-codeudor" required>

            <label for="celular-codeudor">Celular</label>
            <input type="text" id="celular-codeudor" name="celular-codeudor" required>
        </div>

        <div class="form-section">
            <h2>Condiciones del Alquiler</h2>
            <label for="alquiler-adelantado">Un mes de Alquiler Adelantado (Gs.)</label>
            <input type="number" id="alquiler-adelantado" name="alquiler-adelantado" required>

            <label for="deposito">Depósito de Garantía (Gs.)</label>
            <input type="number" id="deposito" name="deposito" required>

            <label for="gastos">Gastos de la Inmobiliaria (Gs.)</label>
            <input type="number" id="gastos" name="gastos" required>
        </div>

        <div class="form-section">
            <h2>Documentación Requerida</h2>
            <div class="checkbox-group">
                <input type="checkbox" id="cedula" name="documentos" value="cedula">
                <label for="cedula">Fotocopia de Cédula de Identidad y RUC</label>
            </div>

            <div class="checkbox-group">
                <input type="checkbox" id="certificado" name="documentos" value="certificado">
                <label for="certificado">Certificado de Trabajo y/o justificativo de ingresos</label>
            </div>
        </div>

        <div class="form-section">
            <h2>Consentimiento</h2>
            <textarea id="consentimiento" rows="8" readonly>
Por el presente instrumento les autorizo en forma expresa e irrevocable... (Incluye aquí el texto completo de la cláusula legal)
            </textarea>
            <div class="checkbox-group">
                <input type="checkbox" id="aceptar" name="aceptar" required>
                <label for="aceptar">Acepto las condiciones descritas anteriormente.</label>
            </div>
        </div>

        <button type="submit" class="submit-btn">Enviar Solicitud</button>
    </form>
</body>
</html>
