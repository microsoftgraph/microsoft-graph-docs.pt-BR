---
title: Usar funções de pasta de trabalho do Excel com o Microsoft Graph
description: 'Você pode usar qualquer função de pasta de trabalho com a seguinte sintaxe: `POST /me/drive/root/workbook/functions/{function-name}`. Forneça o(s) argumento(s) de função no corpo usando um objeto JSON. O `value` resultante da função e quaisquer cadeias de caracteres `error` são retornados no objeto de resultado da função. O valor `error` de `null` indica a execução bem-sucedida da função.'
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 6ba9c94f78325fe855ec6f0c4b2a0dcff8de559a
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491037"
---
# <a name="use-workbook-functions-in-excel-with-microsoft-graph"></a><span data-ttu-id="b0dd0-106">Usar funções de pasta de trabalho do Excel com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b0dd0-106">Use workbook functions in Excel with Microsoft Graph</span></span>

<span data-ttu-id="b0dd0-107">Você pode usar qualquer função de pasta de trabalho com a seguinte sintaxe: `POST /me/drive/root/workbook/functions/{function-name}`.</span><span class="sxs-lookup"><span data-stu-id="b0dd0-107">You can invoke any workbook function by using the following syntax: `POST /me/drive/root/workbook/functions/{function-name}`.</span></span> <span data-ttu-id="b0dd0-108">Forneça o(s) argumento(s) de função no corpo usando um objeto JSON.</span><span class="sxs-lookup"><span data-stu-id="b0dd0-108">You provide the function argument(s) in the body using a JSON object.</span></span> <span data-ttu-id="b0dd0-109">O `value` resultante da função e quaisquer cadeias de caracteres `error` são retornados no objeto de resultado da função.</span><span class="sxs-lookup"><span data-stu-id="b0dd0-109">The function's resulting `value` and any `error` strings are returned in the function result object.</span></span> <span data-ttu-id="b0dd0-110">O valor `error` de `null` indica a execução bem-sucedida da função.</span><span class="sxs-lookup"><span data-stu-id="b0dd0-110">The `error` value of `null` indicates successful execution of the function.</span></span>

<span data-ttu-id="b0dd0-111">Para ver uma lista completa de funções com suporte, consulte [a classe Excel.Functions.](/javascript/api/excel/excel.functions?view=excel-js-preview)</span><span class="sxs-lookup"><span data-stu-id="b0dd0-111">For a complete list of supported functions, see [Excel.Functions class](/javascript/api/excel/excel.functions?view=excel-js-preview).</span></span> <span data-ttu-id="b0dd0-112">Confira a assinatura de função para tipos de dados e nomes de parâmetro específicos.</span><span class="sxs-lookup"><span data-stu-id="b0dd0-112">Refer to the function signature for specific parameter names and data types.</span></span>

<span data-ttu-id="b0dd0-113">_Observações importantes:_</span><span class="sxs-lookup"><span data-stu-id="b0dd0-113">_Important notes:_</span></span>
* <span data-ttu-id="b0dd0-114">O parâmetro de entrada do intervalo é fornecido usando um objeto range, em vez da cadeia de caracteres de endereço do intervalo.</span><span class="sxs-lookup"><span data-stu-id="b0dd0-114">The range input parameter is supplied using a range object instead of the range address string.</span></span>  
* <span data-ttu-id="b0dd0-115">O parâmetro index é indexado como 1, diferentemente do índice 0 usado na maioria das APIs.</span><span class="sxs-lookup"><span data-stu-id="b0dd0-115">The index parameter is 1-indexed unlike the 0-index used in most of the APIs.</span></span>

<span data-ttu-id="b0dd0-116">Exemplo: **vlookup**</span><span class="sxs-lookup"><span data-stu-id="b0dd0-116">Example: **vlookup**</span></span>

<span data-ttu-id="b0dd0-117">Em uma planilha do Excel, a função `vlookup` utiliza os seguintes argumentos:</span><span class="sxs-lookup"><span data-stu-id="b0dd0-117">In an Excel spreadsheet, the `vlookup` function takes the following arguments:</span></span>

1. <span data-ttu-id="b0dd0-118">**valor_proc** (obrigatório): o valor que você deseja pesquisar.</span><span class="sxs-lookup"><span data-stu-id="b0dd0-118">**lookup_value** (required) The value you want to look up.</span></span>
2. <span data-ttu-id="b0dd0-119">**matriz_tabela** (obrigatório): o intervalo de células em que se encontra o valor a pesquisar.</span><span class="sxs-lookup"><span data-stu-id="b0dd0-119">**table_array** (required) The range of cells where the lookup value is located.</span></span> <span data-ttu-id="b0dd0-120">Lembre-se de que o valor de pesquisa sempre deve estar na primeira coluna no intervalo para que o PROCV funcione corretamente.</span><span class="sxs-lookup"><span data-stu-id="b0dd0-120">Remember that the lookup value should always be in the first column in the range for VLOOKUP to work correctly.</span></span> <span data-ttu-id="b0dd0-121">Por exemplo, se o valor de pesquisa estiver na célula C2, o intervalo deve começar com C.</span><span class="sxs-lookup"><span data-stu-id="b0dd0-121">For example, if your lookup value is in cell C2 then your range should start with C.</span></span>
3. <span data-ttu-id="b0dd0-122">**núm_índice_coluna** (obrigatório): o número da coluna no intervalo que contém o valor de retorno.</span><span class="sxs-lookup"><span data-stu-id="b0dd0-122">**col_index_num** (required) The column number in the range that contains the return value.</span></span> <span data-ttu-id="b0dd0-123">Por exemplo, se você especificar B2: D11 como o intervalo, deverá contar B como a primeira coluna, C como a segunda e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="b0dd0-123">For example, if you specify B2: D11 as the range, you should count B as the first column, C as the second, and so on.</span></span>
4. <span data-ttu-id="b0dd0-124">**procurar_intervalo** (opcional): o valor lógico que especifica se você deseja que **PROCV** localize uma correspondência exata ou aproximada.</span><span class="sxs-lookup"><span data-stu-id="b0dd0-124">**range_lookup** (optional) The logical value that specifies whether you want **VLOOKUP** to find an approximate or an exact match.</span></span> <span data-ttu-id="b0dd0-125">Especifique **VERDADEIRO** se desejar uma correspondência aproximada ou **FALSO** se desejar uma correspondência exata do valor de retorno.</span><span class="sxs-lookup"><span data-stu-id="b0dd0-125">Specify **TRUE** if you want an approximate match or **FALSE** if you want an exact match of the return value.</span></span> <span data-ttu-id="b0dd0-126">Se você não especificar nada, o valor padrão sempre será TRUE ou uma correspondência aproximada.</span><span class="sxs-lookup"><span data-stu-id="b0dd0-126">If you don't specify anything, the default value will always be TRUE or approximate match.</span></span>

<span data-ttu-id="b0dd0-127">Dentro de uma célula, a função `vlookup` tem esta aparência:</span><span class="sxs-lookup"><span data-stu-id="b0dd0-127">Inside a cell, the `vlookup` function looks like this:</span></span>

<span data-ttu-id="b0dd0-128">= PROCV(valor de pesquisa, intervalo que contém o valor de pesquisa, o número da coluna no intervalo que contém o valor de retorno, opcionalmente, TRUE para coincidência aproximada ou FALSE para uma correspondência exata)</span><span class="sxs-lookup"><span data-stu-id="b0dd0-128">=VLOOKUP(lookup value, range containing the lookup value, the column number in the range containing the return value, optionally specify TRUE for approximate match or FALSE for an exact match)</span></span>

<span data-ttu-id="b0dd0-129">(Confira a documentação para a função do Excel [PROCV](https://support.office.com/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1)).</span><span class="sxs-lookup"><span data-stu-id="b0dd0-129">(See the documentation for the [VLOOKUP Excel function](https://support.office.com/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)</span></span>


##### <a name="request"></a><span data-ttu-id="b0dd0-130">Solicitação:</span><span class="sxs-lookup"><span data-stu-id="b0dd0-130">Request:</span></span>
<span data-ttu-id="b0dd0-131">O seguinte exemplo mostra como chamar a função `vlookup` e passar esses parâmetros com a API REST do Excel.</span><span class="sxs-lookup"><span data-stu-id="b0dd0-131">The following example shows how to call the `vlookup` function and pass these parameters with the Excel REST API.</span></span>

```http
POST https://graph.microsoft.com/beta/me/drive/root:/book1.xlsx:/workbook/functions/vlookup
content-type: Application/Json
authorization: Bearer {access-token}
workbook-session-id: {session-id}

{
    "lookupValue": "Temperature",
    "tableArray": { "Address": "Sheet1!E1:G5" },
    "colIndexNum": 2,
    "rangeLookup": false
}
```

##### <a name="response"></a><span data-ttu-id="b0dd0-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0dd0-132">Response</span></span>

```http
HTTP code: 200 OK
content-type: application/json;odata.metadata

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#workbookFunctionResult",
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/workbook/functions/vlookup()",
    "error": null,
    "value": "28.3"
}
```

<span data-ttu-id="b0dd0-133">Exemplo: `median`</span><span class="sxs-lookup"><span data-stu-id="b0dd0-133">Example: `median`</span></span>

<span data-ttu-id="b0dd0-134">Em uma planilha do Excel, a função `median` possui uma matriz de um ou mais intervalos de entrada.</span><span class="sxs-lookup"><span data-stu-id="b0dd0-134">In an Excel spreadsheet, the `median` function takes an array of one or more input ranges.</span></span>

<span data-ttu-id="b0dd0-135">Dentro de uma célula, a função `median` se parece com este exemplo:</span><span class="sxs-lookup"><span data-stu-id="b0dd0-135">Inside a cell, the `median` function looks like this example:</span></span>

<span data-ttu-id="b0dd0-136">=MED(A2:A6)</span><span class="sxs-lookup"><span data-stu-id="b0dd0-136">=MEDIAN(A2:A6)</span></span>

<span data-ttu-id="b0dd0-137">(Confira a documentação para a função [MED](https://support.office.com/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2)).</span><span class="sxs-lookup"><span data-stu-id="b0dd0-137">(See the documentation for the [MEDIAN Excel function](https://support.office.com/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)</span></span>

##### <a name="request"></a><span data-ttu-id="b0dd0-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0dd0-138">Request</span></span>
<span data-ttu-id="b0dd0-139">O seguinte exemplo mostra como chamar a função `median` e um ou mais intervalos de entrada com a API REST do Excel.</span><span class="sxs-lookup"><span data-stu-id="b0dd0-139">The following example shows how to call the `median` function and one or more input ranges with the Excel REST API.</span></span>

```http
POST https://graph.microsoft.com/beta/me/drive/root:/book1.xlsx:/workbook/functions/median
content-type: Application/Json
authorization: Bearer {access-token}
workbook-session-id: {session-id}

{
"values" :  [
        { "address": "Sheet2!A1:A5" },
        { "address": "Sheet2!B1:B5" },
      ]
}
```

##### <a name="response"></a><span data-ttu-id="b0dd0-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0dd0-140">Response</span></span>

```http
HTTP code: 200 OK
content-type: application/json;odata.metadata

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#workbookFunctionResult",
  "@odata.type": "#microsoft.graph.workbookFunctionResult",
  "@odata.id": "/users('2abcad6a-2fca-4b6e-9577-e358a757d77d')/drive/root/workbook/functions/median()",
  "error": null,
  "value": 30
}
```

## <a name="see-also"></a><span data-ttu-id="b0dd0-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="b0dd0-141">See also</span></span>
* [<span data-ttu-id="b0dd0-142">Gerenciar sessões do Excel usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b0dd0-142">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="b0dd0-143">Gravar em uma pasta de trabalho do Excel usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b0dd0-143">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="b0dd0-144">Atualizar um formato de intervalo no Excel com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b0dd0-144">Update a range’s format in Excel with Microsoft Graph</span></span>](excel-update-range-format.md)
* [<span data-ttu-id="b0dd0-145">Exibir uma imagem do gráfico do Excel com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b0dd0-145">Display a chart image in Excel with Microsoft Graph</span></span>](excel-display-chart-image.md)
* [<span data-ttu-id="b0dd0-146">Usar a API REST do Excel</span><span class="sxs-lookup"><span data-stu-id="b0dd0-146">Use the Excel REST API</span></span>](/graph/api/resources/excel?view=graph-rest-1.0)
