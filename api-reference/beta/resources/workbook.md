---
title: tipo de recurso da pasta de trabalho
description: Contém objetos de pasta de trabalho relacionados, como planilhas, tabelas, intervalos e assim por diante.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 69d04f6ccd5e537c97854abcb1cf2a9c24820a87
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575704"
---
# <a name="workbook-resource-type"></a><span data-ttu-id="58bd3-103">tipo de recurso da pasta de trabalho</span><span class="sxs-lookup"><span data-stu-id="58bd3-103">workbook resource type</span></span>

<span data-ttu-id="58bd3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58bd3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="58bd3-105">Contém objetos de pasta de trabalho relacionados, como planilhas, tabelas, intervalos e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="58bd3-105">Contains related workbook objects such as worksheets, tables, ranges, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="58bd3-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="58bd3-106">Methods</span></span>

| <span data-ttu-id="58bd3-107">Método</span><span class="sxs-lookup"><span data-stu-id="58bd3-107">Method</span></span>       | <span data-ttu-id="58bd3-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="58bd3-108">Return Type</span></span>  |<span data-ttu-id="58bd3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="58bd3-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="58bd3-110">Criar sessão</span><span class="sxs-lookup"><span data-stu-id="58bd3-110">Create session</span></span>](../api/workbook-createsession.md) | [<span data-ttu-id="58bd3-111">workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="58bd3-111">workbookSessionInfo</span></span>](workbooksessioninfo.md) |<span data-ttu-id="58bd3-112">Crie uma sessão de pasta de trabalho para iniciar uma sessão persistente ou não persistente.</span><span class="sxs-lookup"><span data-stu-id="58bd3-112">Create a workbook session to start a persistent or non-persistent session.</span></span>|
|[<span data-ttu-id="58bd3-113">Fechar sessão</span><span class="sxs-lookup"><span data-stu-id="58bd3-113">Close session</span></span>](../api/workbook-closesession.md) | <span data-ttu-id="58bd3-114">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="58bd3-114">None</span></span> |<span data-ttu-id="58bd3-115">Fechar uma sessão existente.</span><span class="sxs-lookup"><span data-stu-id="58bd3-115">Close an existing session.</span></span>|
|[<span data-ttu-id="58bd3-116">Atualizar sessão</span><span class="sxs-lookup"><span data-stu-id="58bd3-116">Refresh session</span></span>](../api/workbook-refreshsession.md) | <span data-ttu-id="58bd3-117">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="58bd3-117">None</span></span> |<span data-ttu-id="58bd3-118">Atualizar uma sessão existente.</span><span class="sxs-lookup"><span data-stu-id="58bd3-118">Refresh an existing session.</span></span>|

## <a name="properties"></a><span data-ttu-id="58bd3-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="58bd3-119">Properties</span></span>
<span data-ttu-id="58bd3-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="58bd3-120">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="58bd3-121">Relações</span><span class="sxs-lookup"><span data-stu-id="58bd3-121">Relationships</span></span>
| <span data-ttu-id="58bd3-122">Relação</span><span class="sxs-lookup"><span data-stu-id="58bd3-122">Relationship</span></span> | <span data-ttu-id="58bd3-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="58bd3-123">Type</span></span>   |<span data-ttu-id="58bd3-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="58bd3-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58bd3-125">names</span><span class="sxs-lookup"><span data-stu-id="58bd3-125">names</span></span>|<span data-ttu-id="58bd3-126">coleção [workbookNamedItem](workbooknameditem.md)</span><span class="sxs-lookup"><span data-stu-id="58bd3-126">[workbookNamedItem](workbooknameditem.md) collection</span></span> |<span data-ttu-id="58bd3-p101">Representa uma coleção de itens denominados de escopo da pasta de trabalho (chamados intervalos e constantes). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="58bd3-p101">Represents a collection of workbook scoped named items (named ranges and constants). Read-only.</span></span>|
|<span data-ttu-id="58bd3-129">tables</span><span class="sxs-lookup"><span data-stu-id="58bd3-129">tables</span></span>|<span data-ttu-id="58bd3-130">coleção [WorkbookTable](workbooktable.md)</span><span class="sxs-lookup"><span data-stu-id="58bd3-130">[workbookTable](workbooktable.md) collection</span></span> |<span data-ttu-id="58bd3-p102">Representa uma coleção de tabelas associadas à pasta de trabalho. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="58bd3-p102">Represents a collection of tables associated with the workbook. Read-only.</span></span>|
|<span data-ttu-id="58bd3-133">worksheets</span><span class="sxs-lookup"><span data-stu-id="58bd3-133">worksheets</span></span>|<span data-ttu-id="58bd3-134">coleção [WorkbookWorksheet](workbookworksheet.md)</span><span class="sxs-lookup"><span data-stu-id="58bd3-134">[workbookWorksheet](workbookworksheet.md) collection</span></span> |<span data-ttu-id="58bd3-135">Representa uma coleção de planilhas associadas à pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="58bd3-135">Represents a collection of worksheets associated with the workbook.</span></span> <span data-ttu-id="58bd3-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="58bd3-136">Read-only.</span></span>|
|<span data-ttu-id="58bd3-137">workbbookApplication</span><span class="sxs-lookup"><span data-stu-id="58bd3-137">workbbookApplication</span></span>|[<span data-ttu-id="58bd3-138">workbookApplication</span><span class="sxs-lookup"><span data-stu-id="58bd3-138">workbookApplication</span></span>](workbookapplication.md) |<span data-ttu-id="58bd3-139">Representa a workbookApplication do Excel que gerencia a planilha.</span><span class="sxs-lookup"><span data-stu-id="58bd3-139">Represents the Excel workbookApplication that manages the workbook.</span></span>|
|<span data-ttu-id="58bd3-140">operações</span><span class="sxs-lookup"><span data-stu-id="58bd3-140">operations</span></span>|<span data-ttu-id="58bd3-141">coleção [workbookOperation](workbookoperation.md)</span><span class="sxs-lookup"><span data-stu-id="58bd3-141">[workbookOperation](workbookoperation.md) collection</span></span>|<span data-ttu-id="58bd3-142">O status das operações da Workbook.</span><span class="sxs-lookup"><span data-stu-id="58bd3-142">The status of Workbook operations.</span></span> <span data-ttu-id="58bd3-143">Não há suporte para a obtenção de uma coleção de operações, mas você pode obter o status de uma operação de longa execução se o cabeçalho `Location` retornar na resposta.</span><span class="sxs-lookup"><span data-stu-id="58bd3-143">Getting an operation collection is not supported, but you can get the status of a long-running operation if the `Location` header is returned in the response.</span></span> <span data-ttu-id="58bd3-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="58bd3-144">Read-only.</span></span> <span data-ttu-id="58bd3-145">Anulável.</span><span class="sxs-lookup"><span data-stu-id="58bd3-145">Nullable.</span></span>|

## <a name="functions"></a><span data-ttu-id="58bd3-146">Funções</span><span class="sxs-lookup"><span data-stu-id="58bd3-146">Functions</span></span>

<span data-ttu-id="58bd3-p105">[Funções do Excel](#functions): Invoque uma função de pasta de trabalho usando a sintaxe `POST /me/drive/root/workbook/functions/{function-name}` e fornecendo os argumentos de função no corpo usando um objeto JSON. O `value` resultante da função e quaisquer cadeias de caracteres `error` são retornados no objeto de resultado de função. O valor `error` de `null` indica a execução bem-sucedida da função.</span><span class="sxs-lookup"><span data-stu-id="58bd3-p105">[Excel functions](#functions): Invoke a workbook function using the syntax `POST /me/drive/root/workbook/functions/{function-name}` and providing the function argument(s) in the body using a JSON object. The function's resulting `value` and any `error` strings are returned in the function result object. The `error` value of `null` indicates successful execution of the function.</span></span> 

<span data-ttu-id="58bd3-p106">A lista completa de funções com suporte está listada [aqui](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Confira a assinatura de função para tipos de dados e nomes de parâmetro específicos.</span><span class="sxs-lookup"><span data-stu-id="58bd3-p106">The complete list of supported functions are listed [here](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Refer to the function signature for specific parameter names and data types.</span></span>

<span data-ttu-id="58bd3-152">_Observações importantes:_</span><span class="sxs-lookup"><span data-stu-id="58bd3-152">_Important notes:_</span></span> 
* <span data-ttu-id="58bd3-153">O parâmetro de entrada do intervalo é fornecido usando um objeto range, em vez da cadeia de caracteres de endereço do intervalo.</span><span class="sxs-lookup"><span data-stu-id="58bd3-153">The range input parameter is supplied using a range object instead of the range address string.</span></span>  
* <span data-ttu-id="58bd3-154">O parâmetro index é indexado como 1, diferentemente do índice 0 usado na maioria das APIs.</span><span class="sxs-lookup"><span data-stu-id="58bd3-154">The index parameter is 1-indexed unlike the 0-index used in most of the APIs.</span></span> 

<span data-ttu-id="58bd3-155">Exemplo: **vlookup**</span><span class="sxs-lookup"><span data-stu-id="58bd3-155">Example: **vlookup**</span></span>

<span data-ttu-id="58bd3-156">Em uma planilha do Excel, a função `vlookup` utiliza os seguintes argumentos:</span><span class="sxs-lookup"><span data-stu-id="58bd3-156">In an Excel spreadsheet, the `vlookup` function takes the following arguments:</span></span>

1. <span data-ttu-id="58bd3-157">O valor que você deseja pesquisar, também chamado de valor de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="58bd3-157">The value you want to look up, also called the lookup value.</span></span>
2. <span data-ttu-id="58bd3-158">O intervalo em que o valor de pesquisa está localizado.</span><span class="sxs-lookup"><span data-stu-id="58bd3-158">The range where the lookup value is located.</span></span> <span data-ttu-id="58bd3-159">Lembre-se de que o valor de pesquisa sempre deve estar na primeira coluna no intervalo para que o PROCV funcione corretamente.</span><span class="sxs-lookup"><span data-stu-id="58bd3-159">Remember that the lookup value should always be in the first column in the range for VLOOKUP to work correctly.</span></span> <span data-ttu-id="58bd3-160">Por exemplo, se o valor de pesquisa estiver na célula C2, o intervalo deve começar com C.</span><span class="sxs-lookup"><span data-stu-id="58bd3-160">For example, if your lookup value is in cell C2 then your range should start with C.</span></span>
3. <span data-ttu-id="58bd3-161">O número da coluna no intervalo que contém o valor de retorno.</span><span class="sxs-lookup"><span data-stu-id="58bd3-161">The column number in the range that contains the return value.</span></span> <span data-ttu-id="58bd3-162">Por exemplo, se você especificar B2: D11 como o intervalo, deverá contar B como a primeira coluna, C como a segunda e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="58bd3-162">For example, if you specify B2: D11 as the range, you should count B as the first column, C as the second, and so on.</span></span>
4. <span data-ttu-id="58bd3-163">Opcionalmente, você pode especificar TRUE se desejar uma correspondência aproximada ou FALSE se desejar uma correspondência exata do valor de retorno.</span><span class="sxs-lookup"><span data-stu-id="58bd3-163">Optionally, you can specify TRUE if you want an approximate match or FALSE if you want an exact match of the return value.</span></span> <span data-ttu-id="58bd3-164">Se você não especificar nada, o valor padrão sempre será TRUE ou uma correspondência aproximada.</span><span class="sxs-lookup"><span data-stu-id="58bd3-164">If you don't specify anything, the default value will always be TRUE or approximate match.</span></span>

<span data-ttu-id="58bd3-165">Dentro de uma célula, a função `vlookup` tem esta aparência:</span><span class="sxs-lookup"><span data-stu-id="58bd3-165">Inside a cell, the `vlookup` function looks like this:</span></span> 

<span data-ttu-id="58bd3-166">= PROCV(valor de pesquisa, intervalo que contém o valor de pesquisa, o número da coluna no intervalo que contém o valor de retorno, opcionalmente, TRUE para coincidência aproximada ou FALSE para uma correspondência exata)</span><span class="sxs-lookup"><span data-stu-id="58bd3-166">=VLOOKUP(lookup value, range containing the lookup value, the column number in the range containing the return value, optionally specify TRUE for approximate match or FALSE for an exact match)</span></span>

<span data-ttu-id="58bd3-167">(Confira a documentação para a função do Excel [PROCV](https://support.office.com/en-us/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1)).</span><span class="sxs-lookup"><span data-stu-id="58bd3-167">(See the documentation for the [VLOOKUP Excel function](https://support.office.com/en-us/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)</span></span>

<span data-ttu-id="58bd3-168">O exemplo abaixo mostra como chamar a função `vlookup` e passar esses parâmetros com a API REST do Excel.</span><span class="sxs-lookup"><span data-stu-id="58bd3-168">The example below shows how to call the `vlookup` function and pass these parameters with the Excel REST API.</span></span>
<span data-ttu-id="58bd3-169">Solicitação:</span><span class="sxs-lookup"><span data-stu-id="58bd3-169">Request:</span></span> 

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

<span data-ttu-id="58bd3-170">Resposta:</span><span class="sxs-lookup"><span data-stu-id="58bd3-170">Response:</span></span>

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

<span data-ttu-id="58bd3-171">Exemplo: `median`</span><span class="sxs-lookup"><span data-stu-id="58bd3-171">Example: `median`</span></span>

<span data-ttu-id="58bd3-172">Em uma planilha do Excel, a função `median` possui uma matriz de um ou mais intervalos de entrada.</span><span class="sxs-lookup"><span data-stu-id="58bd3-172">In an Excel spreadsheet, the `median` function takes an array of one or more input ranges.</span></span>

<span data-ttu-id="58bd3-173">Dentro de uma célula, a função `median` se parece com este exemplo:</span><span class="sxs-lookup"><span data-stu-id="58bd3-173">Inside a cell, the `median` function looks like this example:</span></span>

<span data-ttu-id="58bd3-174">=MED(A2:A6)</span><span class="sxs-lookup"><span data-stu-id="58bd3-174">=MEDIAN(A2:A6)</span></span>

<span data-ttu-id="58bd3-175">(Confira a documentação para a função [MED](https://support.office.com/en-us/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2)).</span><span class="sxs-lookup"><span data-stu-id="58bd3-175">(See the documentation for the [MEDIAN Excel function](https://support.office.com/en-us/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)</span></span>

<span data-ttu-id="58bd3-176">O exemplo abaixo mostra como chamar a função `median` e um ou mais intervalos de entrada com a API REST do Excel.</span><span class="sxs-lookup"><span data-stu-id="58bd3-176">The example below shows how to call the `median` function and one or more input ranges with the Excel REST API.</span></span> 

<span data-ttu-id="58bd3-177">Solicitação:</span><span class="sxs-lookup"><span data-stu-id="58bd3-177">Request:</span></span> 

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

<span data-ttu-id="58bd3-178">Resposta:</span><span class="sxs-lookup"><span data-stu-id="58bd3-178">Response:</span></span>

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
## <a name="json-representation"></a><span data-ttu-id="58bd3-179">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="58bd3-179">JSON representation</span></span>

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


