# <a name="workbook-resource-type"></a><span data-ttu-id="dcdb0-101">Tipo de recurso de pasta de trabalho</span><span class="sxs-lookup"><span data-stu-id="dcdb0-101">Workbook resource type</span></span>

<span data-ttu-id="dcdb0-102">A pasta de trabalho é o objeto de nível superior que inclui os objetos workbook relacionados, como planilhas, tabelas, intervalos, etc.</span><span class="sxs-lookup"><span data-stu-id="dcdb0-102">Workbook is the top level object which contains related workbook objects such as worksheets, tables, ranges, etc.</span></span>

## <a name="properties"></a><span data-ttu-id="dcdb0-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dcdb0-103">Properties</span></span>
<span data-ttu-id="dcdb0-104">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="dcdb0-104">None</span></span>

## <a name="methods"></a><span data-ttu-id="dcdb0-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="dcdb0-105">Methods</span></span>

| <span data-ttu-id="dcdb0-106">Método</span><span class="sxs-lookup"><span data-stu-id="dcdb0-106">Method</span></span>       | <span data-ttu-id="dcdb0-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dcdb0-107">Return Type</span></span>  |<span data-ttu-id="dcdb0-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcdb0-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dcdb0-109">Criar Sessão</span><span class="sxs-lookup"><span data-stu-id="dcdb0-109">Create Session</span></span>](../api/workbook_createsession.md) | [<span data-ttu-id="dcdb0-110">workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="dcdb0-110">workbookSessionInfo</span></span>](workbooksessioninfo.md) |<span data-ttu-id="dcdb0-111">Crie uma sessão de pasta de trabalho para iniciar uma sessão persistente ou não persistente.</span><span class="sxs-lookup"><span data-stu-id="dcdb0-111">Create a workbook session to start a persistent or non-persistent session.</span></span>|
|[<span data-ttu-id="dcdb0-112">Fechar Sessão</span><span class="sxs-lookup"><span data-stu-id="dcdb0-112">Close Session</span></span>](../api/workbook_closesession.md) | <span data-ttu-id="dcdb0-113">None</span><span class="sxs-lookup"><span data-stu-id="dcdb0-113">None</span></span> |<span data-ttu-id="dcdb0-114">Fechar uma sessão existente.</span><span class="sxs-lookup"><span data-stu-id="dcdb0-114">Close an existing session.</span></span>|
|[<span data-ttu-id="dcdb0-115">Atualizar Sessão</span><span class="sxs-lookup"><span data-stu-id="dcdb0-115">Refresh Session</span></span>](../api/workbook_refreshsession.md) | <span data-ttu-id="dcdb0-116">None</span><span class="sxs-lookup"><span data-stu-id="dcdb0-116">None</span></span> |<span data-ttu-id="dcdb0-117">Atualizar uma sessão existente.</span><span class="sxs-lookup"><span data-stu-id="dcdb0-117">Refresh an existing session.</span></span>|


## <a name="relationships"></a><span data-ttu-id="dcdb0-118">Relações</span><span class="sxs-lookup"><span data-stu-id="dcdb0-118">Relationships</span></span>
| <span data-ttu-id="dcdb0-119">Relação</span><span class="sxs-lookup"><span data-stu-id="dcdb0-119">Relationship</span></span> | <span data-ttu-id="dcdb0-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="dcdb0-120">Type</span></span>   |<span data-ttu-id="dcdb0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcdb0-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dcdb0-122">names</span><span class="sxs-lookup"><span data-stu-id="dcdb0-122">names</span></span>|<span data-ttu-id="dcdb0-123">Coleção [NamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="dcdb0-123">[NamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="dcdb0-p101">Representa uma coleção de itens denominados de escopo da pasta de trabalho (chamados intervalos e constantes). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dcdb0-p101">Represents a collection of workbook scoped named items (named ranges and constants). Read-only.</span></span>|
|<span data-ttu-id="dcdb0-126">tables</span><span class="sxs-lookup"><span data-stu-id="dcdb0-126">tables</span></span>|<span data-ttu-id="dcdb0-127">Coleção [Table](table.md)</span><span class="sxs-lookup"><span data-stu-id="dcdb0-127">[Table](table.md) collection</span></span>|<span data-ttu-id="dcdb0-p102">Representa uma coleção de tabelas associadas à pasta de trabalho. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dcdb0-p102">Represents a collection of tables associated with the workbook. Read-only.</span></span>|
|<span data-ttu-id="dcdb0-130">worksheets</span><span class="sxs-lookup"><span data-stu-id="dcdb0-130">worksheets</span></span>|<span data-ttu-id="dcdb0-131">Coleção [Worksheet](worksheet.md)</span><span class="sxs-lookup"><span data-stu-id="dcdb0-131">[Worksheet](worksheet.md) collection</span></span>|<span data-ttu-id="dcdb0-p103">Representa uma coleção de planilhas associadas à pasta de trabalho. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dcdb0-p103">Represents a collection of worksheets associated with the workbook. Read-only.</span></span>|

## <a name="functions"></a><span data-ttu-id="dcdb0-134">Funções</span><span class="sxs-lookup"><span data-stu-id="dcdb0-134">Functions</span></span>

<span data-ttu-id="dcdb0-135">[Funções do Excel](#functions): Invoque uma função de pasta de trabalho usando a sintaxe `POST /workbook/functions/{function-name}` e fornecendo os argumentos de função no corpo usando um objeto JSON.</span><span class="sxs-lookup"><span data-stu-id="dcdb0-135">[Excel functions](#functions): Invoke a workbook function using the syntax `POST /workbook/functions/{function-name}` and providing the function argument(s) in the body using a JSON object.</span></span> <span data-ttu-id="dcdb0-136">O `value` resultante da função e quaisquer cadeias de caracteres `error` são retornados no objeto de resultado de função.</span><span class="sxs-lookup"><span data-stu-id="dcdb0-136">The function's resulting `value` and any `error` strings are returned in the function result object.</span></span> <span data-ttu-id="dcdb0-137">O valor `error` de `null` indica a execução bem-sucedida da função.</span><span class="sxs-lookup"><span data-stu-id="dcdb0-137">The `error` value of `null` indicates successful execution of the function.</span></span> 

<span data-ttu-id="dcdb0-138">A lista completa de funções com suporte está listada [aqui](https://support.office.com/pt-BR/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188).</span><span class="sxs-lookup"><span data-stu-id="dcdb0-138">The complete list of supported functions are listed [here](https://support.office.com/pt-BR/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188).</span></span> <span data-ttu-id="dcdb0-139">Confira a assinatura de função para tipos de dados e nomes de parâmetro específicos.</span><span class="sxs-lookup"><span data-stu-id="dcdb0-139">Refer to the function signature for specific parameter names and data types.</span></span>

<span data-ttu-id="dcdb0-140">_Observações importantes:_</span><span class="sxs-lookup"><span data-stu-id="dcdb0-140">_Important notes:_</span></span> 
* <span data-ttu-id="dcdb0-141">O parâmetro de entrada do intervalo é fornecido usando um objeto range, em vez da cadeia de caracteres de endereço do intervalo.</span><span class="sxs-lookup"><span data-stu-id="dcdb0-141">The range input parameter is supplied using a range object instead of the range address string.</span></span>  
* <span data-ttu-id="dcdb0-142">O parâmetro index é indexado como 1, diferentemente do índice 0 usado na maioria das APIs.</span><span class="sxs-lookup"><span data-stu-id="dcdb0-142">The index parameter is 1-indexed unlike the 0-index used in most of the APIs.</span></span> 

<span data-ttu-id="dcdb0-143">Exemplo: **vlookup**</span><span class="sxs-lookup"><span data-stu-id="dcdb0-143">Example: **vlookup**</span></span>

<span data-ttu-id="dcdb0-144">Em uma planilha do Excel, a função `vlookup` utiliza os seguintes argumentos:</span><span class="sxs-lookup"><span data-stu-id="dcdb0-144">In an Excel spreadsheet, the `vlookup` function takes the following arguments:</span></span>

1. <span data-ttu-id="dcdb0-145">O valor que você deseja pesquisar, também chamado de valor de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="dcdb0-145">The value you want to look up, also called the lookup value.</span></span>
2. <span data-ttu-id="dcdb0-146">O intervalo em que o valor de pesquisa está localizado.</span><span class="sxs-lookup"><span data-stu-id="dcdb0-146">The range where the lookup value is located.</span></span> <span data-ttu-id="dcdb0-147">Lembre-se de que o valor de pesquisa sempre deve estar na primeira coluna no intervalo para que o PROCV funcione corretamente.</span><span class="sxs-lookup"><span data-stu-id="dcdb0-147">Remember that the lookup value should always be in the first column in the range for VLOOKUP to work correctly.</span></span> <span data-ttu-id="dcdb0-148">Por exemplo, se o valor de pesquisa estiver na célula C2, o intervalo deve começar com C.</span><span class="sxs-lookup"><span data-stu-id="dcdb0-148">For example, if your lookup value is in cell C2 then your range should start with C.</span></span>
3. <span data-ttu-id="dcdb0-149">O número da coluna no intervalo que contém o valor de retorno.</span><span class="sxs-lookup"><span data-stu-id="dcdb0-149">The column number in the range that contains the return value.</span></span> <span data-ttu-id="dcdb0-150">Por exemplo, se você especificar B2: D11 como o intervalo, deverá contar B como a primeira coluna, C como a segunda e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="dcdb0-150">For example, if you specify B2: D11 as the range, you should count B as the first column, C as the second, and so on.</span></span>
4. <span data-ttu-id="dcdb0-151">Opcionalmente, você pode especificar TRUE se desejar uma correspondência aproximada ou FALSE se desejar uma correspondência exata do valor de retorno.</span><span class="sxs-lookup"><span data-stu-id="dcdb0-151">Optionally, you can specify TRUE if you want an approximate match or FALSE if you want an exact match of the return value.</span></span> <span data-ttu-id="dcdb0-152">Se você não especificar nada, o valor padrão sempre será TRUE ou uma correspondência aproximada.</span><span class="sxs-lookup"><span data-stu-id="dcdb0-152">If you don't specify anything, the default value will always be TRUE or approximate match.</span></span>

<span data-ttu-id="dcdb0-153">Dentro de uma célula, a função `vlookup` tem esta aparência:</span><span class="sxs-lookup"><span data-stu-id="dcdb0-153">Inside a cell, the `vlookup` function looks like this:</span></span> 

<span data-ttu-id="dcdb0-154">= PROCV(valor de pesquisa, intervalo que contém o valor de pesquisa, o número da coluna no intervalo que contém o valor de retorno, opcionalmente, TRUE para coincidência aproximada ou FALSE para uma correspondência exata)</span><span class="sxs-lookup"><span data-stu-id="dcdb0-154">=VLOOKUP(lookup value, range containing the lookup value, the column number in the range containing the return value, optionally specify TRUE for approximate match or FALSE for an exact match)</span></span>

<span data-ttu-id="dcdb0-155">(Confira a documentação para a função do Excel [PROCV](https://support.office.com/pt-BR/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1)).</span><span class="sxs-lookup"><span data-stu-id="dcdb0-155">(See the documentation for the [VLOOKUP Excel function](https://support.office.com/pt-BR/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)</span></span>

<span data-ttu-id="dcdb0-156">O exemplo abaixo mostra como chamar a função `vlookup` e passar esses parâmetros com a API REST do Excel.</span><span class="sxs-lookup"><span data-stu-id="dcdb0-156">The example below shows how to call the `vlookup` function and pass these parameters with the Excel REST API.</span></span>

<span data-ttu-id="dcdb0-157">Solicitação:</span><span class="sxs-lookup"><span data-stu-id="dcdb0-157">Request:</span></span> 

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

<span data-ttu-id="dcdb0-158">Resposta:</span><span class="sxs-lookup"><span data-stu-id="dcdb0-158">Response:</span></span>

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

<span data-ttu-id="dcdb0-159">Exemplo: `median`</span><span class="sxs-lookup"><span data-stu-id="dcdb0-159">Example: `median`</span></span>

<span data-ttu-id="dcdb0-160">Em uma planilha do Excel, a função `median` possui uma matriz de um ou mais intervalos de entrada.</span><span class="sxs-lookup"><span data-stu-id="dcdb0-160">In an Excel spreadsheet, the `median` function takes an array of one or more input ranges.</span></span>

<span data-ttu-id="dcdb0-161">Dentro de uma célula, a função `median` se parece com este exemplo:</span><span class="sxs-lookup"><span data-stu-id="dcdb0-161">Inside a cell, the `median` function looks like this example:</span></span>

<span data-ttu-id="dcdb0-162">=MED(A2:A6)</span><span class="sxs-lookup"><span data-stu-id="dcdb0-162">=MEDIAN(A2:A6)</span></span>

<span data-ttu-id="dcdb0-163">(Confira a documentação para a função [MED](https://support.office.com/pt-BR/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2)).</span><span class="sxs-lookup"><span data-stu-id="dcdb0-163">(See the documentation for the [MEDIAN Excel function](https://support.office.com/pt-BR/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)</span></span>

<span data-ttu-id="dcdb0-164">O exemplo abaixo mostra como chamar a função `median` e um ou mais intervalos de entrada com a API REST do Excel.</span><span class="sxs-lookup"><span data-stu-id="dcdb0-164">The example below shows how to call the `median` function and one or more input ranges with the Excel REST API.</span></span> 

<span data-ttu-id="dcdb0-165">Solicitação:</span><span class="sxs-lookup"><span data-stu-id="dcdb0-165">Request:</span></span> 

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

<span data-ttu-id="dcdb0-166">Resposta:</span><span class="sxs-lookup"><span data-stu-id="dcdb0-166">Response:</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Workbook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
