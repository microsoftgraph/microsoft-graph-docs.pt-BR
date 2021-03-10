---
title: tipo de recurso da pasta de trabalho
description: O objeto de nível superior que contém objetos da pasta de trabalho relacionados, como planilhas, tabelas e intervalos.
localization_priority: Priority
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ec413303365d97a2683997939e20820ed9205f84
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577825"
---
# <a name="workbook-resource-type"></a><span data-ttu-id="78804-103">tipo de recurso da pasta de trabalho</span><span class="sxs-lookup"><span data-stu-id="78804-103">workbook resource type</span></span>

<span data-ttu-id="78804-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78804-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="78804-105">O objeto de nível superior que contém objetos da pasta de trabalho relacionados, como planilhas, tabelas e intervalos.</span><span class="sxs-lookup"><span data-stu-id="78804-105">The top-level object that contains related workbook objects such as worksheets, tables, and ranges.</span></span>

## <a name="methods"></a><span data-ttu-id="78804-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="78804-106">Methods</span></span>

| <span data-ttu-id="78804-107">Método</span><span class="sxs-lookup"><span data-stu-id="78804-107">Method</span></span>       | <span data-ttu-id="78804-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="78804-108">Return Type</span></span>  |<span data-ttu-id="78804-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="78804-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="78804-110">Criar sessão</span><span class="sxs-lookup"><span data-stu-id="78804-110">Create session</span></span>](../api/workbook-createsession.md) | [<span data-ttu-id="78804-111">workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="78804-111">workbookSessionInfo</span></span>](workbooksessioninfo.md) |<span data-ttu-id="78804-112">Crie uma sessão de pasta de trabalho para iniciar uma sessão persistente ou não persistente.</span><span class="sxs-lookup"><span data-stu-id="78804-112">Create a workbook session to start a persistent or non-persistent session.</span></span>|
|[<span data-ttu-id="78804-113">Fechar sessão</span><span class="sxs-lookup"><span data-stu-id="78804-113">Close session</span></span>](../api/workbook-closesession.md) | <span data-ttu-id="78804-114">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="78804-114">None</span></span> |<span data-ttu-id="78804-115">Fechar uma sessão existente.</span><span class="sxs-lookup"><span data-stu-id="78804-115">Close an existing session.</span></span>|
|[<span data-ttu-id="78804-116">Atualizar sessão</span><span class="sxs-lookup"><span data-stu-id="78804-116">Refresh session</span></span>](../api/workbook-refreshsession.md) | <span data-ttu-id="78804-117">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="78804-117">None</span></span> |<span data-ttu-id="78804-118">Atualizar uma sessão existente.</span><span class="sxs-lookup"><span data-stu-id="78804-118">Refresh an existing session.</span></span>|

## <a name="properties"></a><span data-ttu-id="78804-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="78804-119">Properties</span></span>
<span data-ttu-id="78804-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="78804-120">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="78804-121">Relações</span><span class="sxs-lookup"><span data-stu-id="78804-121">Relationships</span></span>
| <span data-ttu-id="78804-122">Relação</span><span class="sxs-lookup"><span data-stu-id="78804-122">Relationship</span></span> | <span data-ttu-id="78804-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="78804-123">Type</span></span>   |<span data-ttu-id="78804-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="78804-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78804-125">names</span><span class="sxs-lookup"><span data-stu-id="78804-125">names</span></span>|<span data-ttu-id="78804-126">coleção [workbookNamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="78804-126">[workbookNamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="78804-p101">Representa uma coleção de itens denominados de escopo da pasta de trabalho (chamados intervalos e constantes). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78804-p101">Represents a collection of workbook scoped named items (named ranges and constants). Read-only.</span></span>|
|<span data-ttu-id="78804-129">tables</span><span class="sxs-lookup"><span data-stu-id="78804-129">tables</span></span>|<span data-ttu-id="78804-130">coleção [WorkbookTable](table.md)</span><span class="sxs-lookup"><span data-stu-id="78804-130">[workbookTable](table.md) collection</span></span>|<span data-ttu-id="78804-p102">Representa uma coleção de tabelas associadas à pasta de trabalho. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78804-p102">Represents a collection of tables associated with the workbook. Read-only.</span></span>|
|<span data-ttu-id="78804-133">worksheets</span><span class="sxs-lookup"><span data-stu-id="78804-133">worksheets</span></span>|<span data-ttu-id="78804-134">coleção [WorkbookWorksheet](worksheet.md)</span><span class="sxs-lookup"><span data-stu-id="78804-134">[workbookWorksheet](worksheet.md) collection</span></span>|<span data-ttu-id="78804-135">Representa uma coleção de planilhas associadas à pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="78804-135">Represents a collection of worksheets associated with the workbook.</span></span> <span data-ttu-id="78804-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78804-136">Read-only.</span></span>|
|<span data-ttu-id="78804-137">operações</span><span class="sxs-lookup"><span data-stu-id="78804-137">operations</span></span>|<span data-ttu-id="78804-138">coleção [workbookOperation](workbookoperation.md)</span><span class="sxs-lookup"><span data-stu-id="78804-138">[workbookOperation](workbookoperation.md) collection</span></span>|<span data-ttu-id="78804-139">O status das operações da pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="78804-139">The status of workbook operations.</span></span> <span data-ttu-id="78804-140">Não há suporte para a obtenção de uma coleção de operações, mas você pode obter o status de uma operação de longa execução se o cabeçalho `Location` retornar na resposta.</span><span class="sxs-lookup"><span data-stu-id="78804-140">Getting an operation collection is not supported, but you can get the status of a long-running operation if the `Location` header is returned in the response.</span></span> <span data-ttu-id="78804-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78804-141">Read-only.</span></span>|

## <a name="functions"></a><span data-ttu-id="78804-142">Funções</span><span class="sxs-lookup"><span data-stu-id="78804-142">Functions</span></span>

<span data-ttu-id="78804-p105">[Funções do Excel](#functions): Invoque uma função de pasta de trabalho usando a sintaxe `POST /me/drive/root/workbook/functions/{function-name}` e fornecendo os argumentos de função no corpo usando um objeto JSON. O `value` resultante da função e quaisquer cadeias de caracteres `error` são retornados no objeto de resultado de função. O valor `error` de `null` indica a execução bem-sucedida da função.</span><span class="sxs-lookup"><span data-stu-id="78804-p105">[Excel functions](#functions): Invoke a workbook function using the syntax `POST /me/drive/root/workbook/functions/{function-name}` and providing the function argument(s) in the body using a JSON object. The function's resulting `value` and any `error` strings are returned in the function result object. The `error` value of `null` indicates successful execution of the function.</span></span> 

<span data-ttu-id="78804-p106">A lista completa de funções com suporte está listada [aqui](https://support.office.com/pt-BR/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Confira a assinatura de função para tipos de dados e nomes de parâmetro específicos.</span><span class="sxs-lookup"><span data-stu-id="78804-p106">The complete list of supported functions are listed [here](https://support.office.com/pt-BR/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Refer to the function signature for specific parameter names and data types.</span></span>

<span data-ttu-id="78804-148">_Observações importantes:_</span><span class="sxs-lookup"><span data-stu-id="78804-148">_Important notes:_</span></span> 
* <span data-ttu-id="78804-149">O parâmetro de entrada do intervalo é fornecido usando um objeto range, em vez da cadeia de caracteres de endereço do intervalo.</span><span class="sxs-lookup"><span data-stu-id="78804-149">The range input parameter is supplied using a range object instead of the range address string.</span></span>  
* <span data-ttu-id="78804-150">O parâmetro index é indexado como 1, diferentemente do índice 0 usado na maioria das APIs.</span><span class="sxs-lookup"><span data-stu-id="78804-150">The index parameter is 1-indexed unlike the 0-index used in most of the APIs.</span></span> 

<span data-ttu-id="78804-151">Exemplo: **vlookup**</span><span class="sxs-lookup"><span data-stu-id="78804-151">Example: **vlookup**</span></span>

<span data-ttu-id="78804-152">Em uma planilha do Excel, a função `vlookup` utiliza os seguintes argumentos:</span><span class="sxs-lookup"><span data-stu-id="78804-152">In an Excel spreadsheet, the `vlookup` function takes the following arguments:</span></span>

1. <span data-ttu-id="78804-153">O valor que você deseja pesquisar, também chamado de valor de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="78804-153">The value you want to look up, also called the lookup value.</span></span>
2. <span data-ttu-id="78804-154">O intervalo em que o valor de pesquisa está localizado.</span><span class="sxs-lookup"><span data-stu-id="78804-154">The range where the lookup value is located.</span></span> <span data-ttu-id="78804-155">Lembre-se de que o valor de pesquisa sempre deve estar na primeira coluna no intervalo para que o PROCV funcione corretamente.</span><span class="sxs-lookup"><span data-stu-id="78804-155">Remember that the lookup value should always be in the first column in the range for VLOOKUP to work correctly.</span></span> <span data-ttu-id="78804-156">Por exemplo, se o valor de pesquisa estiver na célula C2, o intervalo deve começar com C.</span><span class="sxs-lookup"><span data-stu-id="78804-156">For example, if your lookup value is in cell C2 then your range should start with C.</span></span>
3. <span data-ttu-id="78804-157">O número da coluna no intervalo que contém o valor de retorno.</span><span class="sxs-lookup"><span data-stu-id="78804-157">The column number in the range that contains the return value.</span></span> <span data-ttu-id="78804-158">Por exemplo, se você especificar B2: D11 como o intervalo, deverá contar B como a primeira coluna, C como a segunda e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="78804-158">For example, if you specify B2: D11 as the range, you should count B as the first column, C as the second, and so on.</span></span>
4. <span data-ttu-id="78804-159">Opcionalmente, você pode especificar TRUE se desejar uma correspondência aproximada ou FALSE se desejar uma correspondência exata do valor de retorno.</span><span class="sxs-lookup"><span data-stu-id="78804-159">Optionally, you can specify TRUE if you want an approximate match or FALSE if you want an exact match of the return value.</span></span> <span data-ttu-id="78804-160">Se você não especificar nada, o valor padrão sempre será TRUE ou uma correspondência aproximada.</span><span class="sxs-lookup"><span data-stu-id="78804-160">If you don't specify anything, the default value will always be TRUE or approximate match.</span></span>

<span data-ttu-id="78804-161">Dentro de uma célula, a função `vlookup` tem esta aparência:</span><span class="sxs-lookup"><span data-stu-id="78804-161">Inside a cell, the `vlookup` function looks like this:</span></span> 

<span data-ttu-id="78804-162">= PROCV(valor de pesquisa, intervalo que contém o valor de pesquisa, o número da coluna no intervalo que contém o valor de retorno, opcionalmente, TRUE para coincidência aproximada ou FALSE para uma correspondência exata)</span><span class="sxs-lookup"><span data-stu-id="78804-162">=VLOOKUP(lookup value, range containing the lookup value, the column number in the range containing the return value, optionally specify TRUE for approximate match or FALSE for an exact match)</span></span>

<span data-ttu-id="78804-163">(Confira a documentação para a função do Excel [PROCV](https://support.office.com/pt-BR/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1)).</span><span class="sxs-lookup"><span data-stu-id="78804-163">(See the documentation for the [VLOOKUP Excel function](https://support.office.com/pt-BR/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)</span></span>

<span data-ttu-id="78804-164">O exemplo abaixo mostra como chamar a função `vlookup` e passar esses parâmetros com a API REST do Excel.</span><span class="sxs-lookup"><span data-stu-id="78804-164">The example below shows how to call the `vlookup` function and pass these parameters with the Excel REST API.</span></span>

<span data-ttu-id="78804-165">Solicitação:</span><span class="sxs-lookup"><span data-stu-id="78804-165">Request:</span></span> 

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

<span data-ttu-id="78804-166">Resposta:</span><span class="sxs-lookup"><span data-stu-id="78804-166">Response:</span></span>

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

<span data-ttu-id="78804-167">Exemplo: `median`</span><span class="sxs-lookup"><span data-stu-id="78804-167">Example: `median`</span></span>

<span data-ttu-id="78804-168">Em uma planilha do Excel, a função `median` possui uma matriz de um ou mais intervalos de entrada.</span><span class="sxs-lookup"><span data-stu-id="78804-168">In an Excel spreadsheet, the `median` function takes an array of one or more input ranges.</span></span>

<span data-ttu-id="78804-169">Dentro de uma célula, a função `median` se parece com este exemplo:</span><span class="sxs-lookup"><span data-stu-id="78804-169">Inside a cell, the `median` function looks like this example:</span></span>

<span data-ttu-id="78804-170">=MED(A2:A6)</span><span class="sxs-lookup"><span data-stu-id="78804-170">=MEDIAN(A2:A6)</span></span>

<span data-ttu-id="78804-171">(Confira a documentação para a função [MED](https://support.office.com/pt-BR/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2)).</span><span class="sxs-lookup"><span data-stu-id="78804-171">(See the documentation for the [MEDIAN Excel function](https://support.office.com/pt-BR/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)</span></span>

<span data-ttu-id="78804-172">O exemplo abaixo mostra como chamar a função `median` e um ou mais intervalos de entrada com a API REST do Excel.</span><span class="sxs-lookup"><span data-stu-id="78804-172">The example below shows how to call the `median` function and one or more input ranges with the Excel REST API.</span></span> 

<span data-ttu-id="78804-173">Solicitação:</span><span class="sxs-lookup"><span data-stu-id="78804-173">Request:</span></span> 

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

<span data-ttu-id="78804-174">Resposta:</span><span class="sxs-lookup"><span data-stu-id="78804-174">Response:</span></span>

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
## <a name="json-representation"></a><span data-ttu-id="78804-175">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="78804-175">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbook"
}-->

```json
{
  "names": [{"@odata.type": "microsoft.graph.workbookNamedItem"}],
  "tables": [{"@odata.type": "microsoft.graph.workbookTable"}],
  "worksheets": [{"@odata.type": "microsoft.graph.workbookWorksheet"}]
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

