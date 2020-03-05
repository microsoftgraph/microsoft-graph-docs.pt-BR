---
title: tipo de recurso Workbook
description: Contém objetos Workbook relacionados, como planilhas, tabelas, intervalos e assim por diante.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 47a0a9cc517bad5ad005a23b1de94a38992da44e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519418"
---
# <a name="workbook-resource-type"></a><span data-ttu-id="b5e79-103">tipo de recurso Workbook</span><span class="sxs-lookup"><span data-stu-id="b5e79-103">workbook resource type</span></span>

<span data-ttu-id="b5e79-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b5e79-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b5e79-105">Contém objetos Workbook relacionados, como planilhas, tabelas, intervalos e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="b5e79-105">Contains related workbook objects such as worksheets, tables, ranges, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="b5e79-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="b5e79-106">Methods</span></span>

| <span data-ttu-id="b5e79-107">Método</span><span class="sxs-lookup"><span data-stu-id="b5e79-107">Method</span></span>       | <span data-ttu-id="b5e79-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b5e79-108">Return Type</span></span>  |<span data-ttu-id="b5e79-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5e79-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b5e79-110">Criar sessão</span><span class="sxs-lookup"><span data-stu-id="b5e79-110">Create session</span></span>](../api/workbook-createsession.md) | [<span data-ttu-id="b5e79-111">workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="b5e79-111">workbookSessionInfo</span></span>](workbooksessioninfo.md) |<span data-ttu-id="b5e79-112">Crie uma sessão de pasta de trabalho para iniciar uma sessão persistente ou não persistente.</span><span class="sxs-lookup"><span data-stu-id="b5e79-112">Create a workbook session to start a persistent or non-persistent session.</span></span>|
|[<span data-ttu-id="b5e79-113">Fechar sessão</span><span class="sxs-lookup"><span data-stu-id="b5e79-113">Close session</span></span>](../api/workbook-closesession.md) | <span data-ttu-id="b5e79-114">None</span><span class="sxs-lookup"><span data-stu-id="b5e79-114">None</span></span> |<span data-ttu-id="b5e79-115">Fechar uma sessão existente.</span><span class="sxs-lookup"><span data-stu-id="b5e79-115">Close an existing session.</span></span>|
|[<span data-ttu-id="b5e79-116">Atualizar sessão</span><span class="sxs-lookup"><span data-stu-id="b5e79-116">Refresh session</span></span>](../api/workbook-refreshsession.md) | <span data-ttu-id="b5e79-117">None</span><span class="sxs-lookup"><span data-stu-id="b5e79-117">None</span></span> |<span data-ttu-id="b5e79-118">Atualizar uma sessão existente.</span><span class="sxs-lookup"><span data-stu-id="b5e79-118">Refresh an existing session.</span></span>|

## <a name="properties"></a><span data-ttu-id="b5e79-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b5e79-119">Properties</span></span>
<span data-ttu-id="b5e79-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b5e79-120">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="b5e79-121">Relações</span><span class="sxs-lookup"><span data-stu-id="b5e79-121">Relationships</span></span>
| <span data-ttu-id="b5e79-122">Relação</span><span class="sxs-lookup"><span data-stu-id="b5e79-122">Relationship</span></span> | <span data-ttu-id="b5e79-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5e79-123">Type</span></span>   |<span data-ttu-id="b5e79-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5e79-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5e79-125">names</span><span class="sxs-lookup"><span data-stu-id="b5e79-125">names</span></span>|<span data-ttu-id="b5e79-126">coleção [workbookNamedItem](workbooknameditem.md)</span><span class="sxs-lookup"><span data-stu-id="b5e79-126">[workbookNamedItem](workbooknameditem.md) collection</span></span> |<span data-ttu-id="b5e79-p101">Representa uma coleção de itens denominados de escopo da pasta de trabalho (chamados intervalos e constantes). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b5e79-p101">Represents a collection of workbook scoped named items (named ranges and constants). Read-only.</span></span>|
|<span data-ttu-id="b5e79-129">tables</span><span class="sxs-lookup"><span data-stu-id="b5e79-129">tables</span></span>|<span data-ttu-id="b5e79-130">coleção [workbooktable](workbooktable.md)</span><span class="sxs-lookup"><span data-stu-id="b5e79-130">[workbookTable](workbooktable.md) collection</span></span> |<span data-ttu-id="b5e79-p102">Representa uma coleção de tabelas associadas à pasta de trabalho. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b5e79-p102">Represents a collection of tables associated with the workbook. Read-only.</span></span>|
|<span data-ttu-id="b5e79-133">worksheets</span><span class="sxs-lookup"><span data-stu-id="b5e79-133">worksheets</span></span>|<span data-ttu-id="b5e79-134">coleção [workbookWorksheet](workbookworksheet.md)</span><span class="sxs-lookup"><span data-stu-id="b5e79-134">[workbookWorksheet](workbookworksheet.md) collection</span></span> |<span data-ttu-id="b5e79-135">Representa uma coleção de planilhas associadas à pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="b5e79-135">Represents a collection of worksheets associated with the workbook.</span></span> <span data-ttu-id="b5e79-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b5e79-136">Read-only.</span></span>|
|<span data-ttu-id="b5e79-137">workbbookApplication</span><span class="sxs-lookup"><span data-stu-id="b5e79-137">workbbookApplication</span></span>|[<span data-ttu-id="b5e79-138">workbookApplication</span><span class="sxs-lookup"><span data-stu-id="b5e79-138">workbookApplication</span></span>](workbookapplication.md) |<span data-ttu-id="b5e79-139">Representa o workbookApplication do Excel que gerencia a pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="b5e79-139">Represents the Excel workbookApplication that manages the workbook.</span></span>|

## <a name="functions"></a><span data-ttu-id="b5e79-140">Funções</span><span class="sxs-lookup"><span data-stu-id="b5e79-140">Functions</span></span>

<span data-ttu-id="b5e79-p104">[Funções do Excel](#functions): Invoque uma função de pasta de trabalho usando a sintaxe `POST /workbook/functions/{function-name}` e fornecendo os argumentos de função no corpo usando um objeto JSON. O `value` resultante da função e quaisquer cadeias de caracteres `error` são retornados no objeto de resultado de função. O valor `error` de `null` indica a execução bem-sucedida da função.</span><span class="sxs-lookup"><span data-stu-id="b5e79-p104">[Excel functions](#functions): Invoke a workbook function using the syntax `POST /workbook/functions/{function-name}` and providing the function argument(s) in the body using a JSON object. The function's resulting `value` and any `error` strings are returned in the function result object. The `error` value of `null` indicates successful execution of the function.</span></span> 

<span data-ttu-id="b5e79-p105">A lista completa de funções com suporte está listada [aqui](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Confira a assinatura de função para tipos de dados e nomes de parâmetro específicos.</span><span class="sxs-lookup"><span data-stu-id="b5e79-p105">The complete list of supported functions are listed [here](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Refer to the function signature for specific parameter names and data types.</span></span>

<span data-ttu-id="b5e79-146">_Observações importantes:_</span><span class="sxs-lookup"><span data-stu-id="b5e79-146">_Important notes:_</span></span> 
* <span data-ttu-id="b5e79-147">O parâmetro de entrada do intervalo é fornecido usando um objeto range, em vez da cadeia de caracteres de endereço do intervalo.</span><span class="sxs-lookup"><span data-stu-id="b5e79-147">The range input parameter is supplied using a range object instead of the range address string.</span></span>  
* <span data-ttu-id="b5e79-148">O parâmetro index é indexado como 1, diferentemente do índice 0 usado na maioria das APIs.</span><span class="sxs-lookup"><span data-stu-id="b5e79-148">The index parameter is 1-indexed unlike the 0-index used in most of the APIs.</span></span> 

<span data-ttu-id="b5e79-149">Exemplo: **vlookup**</span><span class="sxs-lookup"><span data-stu-id="b5e79-149">Example: **vlookup**</span></span>

<span data-ttu-id="b5e79-150">Em uma planilha do Excel, a função `vlookup` utiliza os seguintes argumentos:</span><span class="sxs-lookup"><span data-stu-id="b5e79-150">In an Excel spreadsheet, the `vlookup` function takes the following arguments:</span></span>

1. <span data-ttu-id="b5e79-151">O valor que você deseja pesquisar, também chamado de valor de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="b5e79-151">The value you want to look up, also called the lookup value.</span></span>
2. <span data-ttu-id="b5e79-152">O intervalo em que o valor de pesquisa está localizado.</span><span class="sxs-lookup"><span data-stu-id="b5e79-152">The range where the lookup value is located.</span></span> <span data-ttu-id="b5e79-153">Lembre-se de que o valor de pesquisa sempre deve estar na primeira coluna no intervalo para que o PROCV funcione corretamente.</span><span class="sxs-lookup"><span data-stu-id="b5e79-153">Remember that the lookup value should always be in the first column in the range for VLOOKUP to work correctly.</span></span> <span data-ttu-id="b5e79-154">Por exemplo, se o valor de pesquisa estiver na célula C2, o intervalo deve começar com C.</span><span class="sxs-lookup"><span data-stu-id="b5e79-154">For example, if your lookup value is in cell C2 then your range should start with C.</span></span>
3. <span data-ttu-id="b5e79-155">O número da coluna no intervalo que contém o valor de retorno.</span><span class="sxs-lookup"><span data-stu-id="b5e79-155">The column number in the range that contains the return value.</span></span> <span data-ttu-id="b5e79-156">Por exemplo, se você especificar B2: D11 como o intervalo, deverá contar B como a primeira coluna, C como a segunda e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="b5e79-156">For example, if you specify B2: D11 as the range, you should count B as the first column, C as the second, and so on.</span></span>
4. <span data-ttu-id="b5e79-157">Opcionalmente, você pode especificar TRUE se desejar uma correspondência aproximada ou FALSE se desejar uma correspondência exata do valor de retorno.</span><span class="sxs-lookup"><span data-stu-id="b5e79-157">Optionally, you can specify TRUE if you want an approximate match or FALSE if you want an exact match of the return value.</span></span> <span data-ttu-id="b5e79-158">Se você não especificar nada, o valor padrão sempre será TRUE ou uma correspondência aproximada.</span><span class="sxs-lookup"><span data-stu-id="b5e79-158">If you don't specify anything, the default value will always be TRUE or approximate match.</span></span>

<span data-ttu-id="b5e79-159">Dentro de uma célula, a função `vlookup` tem esta aparência:</span><span class="sxs-lookup"><span data-stu-id="b5e79-159">Inside a cell, the `vlookup` function looks like this:</span></span> 

<span data-ttu-id="b5e79-160">= PROCV(valor de pesquisa, intervalo que contém o valor de pesquisa, o número da coluna no intervalo que contém o valor de retorno, opcionalmente, TRUE para coincidência aproximada ou FALSE para uma correspondência exata)</span><span class="sxs-lookup"><span data-stu-id="b5e79-160">=VLOOKUP(lookup value, range containing the lookup value, the column number in the range containing the return value, optionally specify TRUE for approximate match or FALSE for an exact match)</span></span>

<span data-ttu-id="b5e79-161">(Confira a documentação para a função do Excel [PROCV](https://support.office.com/en-us/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1)).</span><span class="sxs-lookup"><span data-stu-id="b5e79-161">(See the documentation for the [VLOOKUP Excel function](https://support.office.com/en-us/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)</span></span>

<span data-ttu-id="b5e79-162">O exemplo abaixo mostra como chamar a função `vlookup` e passar esses parâmetros com a API REST do Excel.</span><span class="sxs-lookup"><span data-stu-id="b5e79-162">The example below shows how to call the `vlookup` function and pass these parameters with the Excel REST API.</span></span>
<span data-ttu-id="b5e79-163">Solicitação:</span><span class="sxs-lookup"><span data-stu-id="b5e79-163">Request:</span></span> 

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

<span data-ttu-id="b5e79-164">Resposta:</span><span class="sxs-lookup"><span data-stu-id="b5e79-164">Response:</span></span>

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

<span data-ttu-id="b5e79-165">Exemplo: `median`</span><span class="sxs-lookup"><span data-stu-id="b5e79-165">Example: `median`</span></span>

<span data-ttu-id="b5e79-166">Em uma planilha do Excel, a função `median` possui uma matriz de um ou mais intervalos de entrada.</span><span class="sxs-lookup"><span data-stu-id="b5e79-166">In an Excel spreadsheet, the `median` function takes an array of one or more input ranges.</span></span>

<span data-ttu-id="b5e79-167">Dentro de uma célula, a função `median` se parece com este exemplo:</span><span class="sxs-lookup"><span data-stu-id="b5e79-167">Inside a cell, the `median` function looks like this example:</span></span>

<span data-ttu-id="b5e79-168">=MED(A2:A6)</span><span class="sxs-lookup"><span data-stu-id="b5e79-168">=MEDIAN(A2:A6)</span></span>

<span data-ttu-id="b5e79-169">(Confira a documentação para a função [MED](https://support.office.com/en-us/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2)).</span><span class="sxs-lookup"><span data-stu-id="b5e79-169">(See the documentation for the [MEDIAN Excel function](https://support.office.com/en-us/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)</span></span>

<span data-ttu-id="b5e79-170">O exemplo abaixo mostra como chamar a função `median` e um ou mais intervalos de entrada com a API REST do Excel.</span><span class="sxs-lookup"><span data-stu-id="b5e79-170">The example below shows how to call the `median` function and one or more input ranges with the Excel REST API.</span></span> 

<span data-ttu-id="b5e79-171">Solicitação:</span><span class="sxs-lookup"><span data-stu-id="b5e79-171">Request:</span></span> 

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

<span data-ttu-id="b5e79-172">Resposta:</span><span class="sxs-lookup"><span data-stu-id="b5e79-172">Response:</span></span>

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
## <a name="json-representation"></a><span data-ttu-id="b5e79-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b5e79-173">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.workbook"
}-->
``` json
{
    "id": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Workbook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
