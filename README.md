<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NOVA NFI</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f9;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
        }
        h1 {
            margin-top: 20px;
            color: #333;
        }
        form {
            background: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            max-width: 600px;
            width: 100%;
        }
        label {
            display: block;
            margin: 15px 0 5px;
            color: #555;
        }
        input, textarea, select, button {
            width: 100%;
            padding: 10px;
            margin-bottom: 15px;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 1rem;
        }
        button {
            background-color: #007bff;
            color: #fff;
            border: none;
            cursor: pointer;
        }
        button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <h1>NOVA NFI</h1>
    <form id="nfiForm">
        <!-- Campos livres -->
        <label for="noiNumber">Qual o número da NOI?</label>
        <input type="text" id="noiNumber" name="noiNumber" required>

        <label for="revisionNumber">Qual o número da REVISÃO da NOI?</label>
        <input type="text" id="revisionNumber" name="revisionNumber" required>

        <label for="inspectorFirm">Qual a FIRMA INSPETORA?</label>
        <input type="text" id="inspectorFirm" name="inspectorFirm" required>

        <label for="projectName">Qual o nome do PROJETO?</label>
        <input type="text" id="projectName" name="projectName" required>

        <label for="clientName">Qual o nome do CLIENTE?</label>
        <input type="text" id="clientName" name="clientName" required>

        <!-- Local de Inspeção -->
        <label for="inspectionLocation">Qual o local de Inspeção?</label>
        <select id="inspectionLocation" name="inspectionLocation" required>
            <option value="">Selecione...</option>
            <option value="Jeceaba">Jeceaba</option>
            <option value="Barreiro">Barreiro</option>
            <option value="Porto">Porto</option>
            <option value="LCF">LCF</option>
            <option value="VTS">VTS</option>
        </select>

        <!-- Campos livres -->
        <label for="orderItem">Qual o PEDIDO / ITEM?</label>
        <input type="text" id="orderItem" name="orderItem" required>

        <!-- Datas -->
        <label for="startDate">Qual a DATA de INÍCIO de Inspeção?</label>
        <input type="date" id="startDate" name="startDate" required>

        <label for="endDate">Qual a DATA de TÉRMINO de Inspeção?</label>
        <input type="date" id="endDate" name="endDate" required>

        <!-- Etapas -->
        <label for="inspectionStage">Qual a ETAPA de inspeção?</label>
        <select id="inspectionStage" name="inspectionStage" required>
            <option value="">Selecione...</option>
            <option value="AC">AC</option>
            <option value="RM">RM</option>
            <option value="QT">QT</option>
            <option value="LAB">LAB</option>
            <option value="FAST">FAST</option>
            <option value="FLEX">FLEX</option>
            <option value="LUVAS">LUVAS</option>
            <option value="DPA">DPA</option>
            <option value="DOCs">DOCs</option>
            <option value="PORTO">PORTO</option>
        </select>

        <!-- Campos livres -->
        <label for="qpMip">Qual o QP/MIP?</label>
        <input type="text" id="qpMip" name="qpMip" required>

        <label for="otherFields">Outros campos</label>
        <textarea id="otherFields" name="otherFields" placeholder="Preencha com os demais detalhes..."></textarea>

        <button type="submit">Enviar</button>
    </form>
</body>
</html>
