# <a name="workbook-resource-type"></a><span data-ttu-id="deadd-101">Tipo de recurso de pasta de trabalho</span><span class="sxs-lookup"><span data-stu-id="deadd-101">Workbook resource type</span></span>

<span data-ttu-id="deadd-102">A pasta de trabalho é o objeto de nível superior que inclui os objetos workbook relacionados, como planilhas, tabelas, intervalos, etc.</span><span class="sxs-lookup"><span data-stu-id="deadd-102">Workbook is the top level object which contains related workbook objects such as worksheets, tables, ranges, etc.</span></span>

## <a name="properties"></a><span data-ttu-id="deadd-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="deadd-103">Properties</span></span>
<span data-ttu-id="deadd-104">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="deadd-104">None</span></span>

## <a name="methods"></a><span data-ttu-id="deadd-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="deadd-105">Methods</span></span>

| <span data-ttu-id="deadd-106">Método</span><span class="sxs-lookup"><span data-stu-id="deadd-106">Method</span></span>       | <span data-ttu-id="deadd-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="deadd-107">Return Type</span></span>  |<span data-ttu-id="deadd-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="deadd-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="deadd-109">Criar Sessão</span><span class="sxs-lookup"><span data-stu-id="deadd-109">Create Upload Session</span></span>](../api/workbook_createsession.md) | [<span data-ttu-id="deadd-110">workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="deadd-110">workbookSessionInfo</span></span>](workbooksessioninfo.md) |<span data-ttu-id="deadd-111">Crie uma sessão de pasta de trabalho para iniciar uma sessão persistente ou não persistente.</span><span class="sxs-lookup"><span data-stu-id="deadd-111">Create a workbook session to start a persistent or non-persistent session.</span></span>|
|[<span data-ttu-id="deadd-112">Fechar Sessão</span><span class="sxs-lookup"><span data-stu-id="deadd-112">Close Session</span></span>](../api/workbook_closesession.md) | <span data-ttu-id="deadd-113">None</span><span class="sxs-lookup"><span data-stu-id="deadd-113">None</span></span> |<span data-ttu-id="deadd-114">Fechar uma sessão existente.</span><span class="sxs-lookup"><span data-stu-id="deadd-114">Close an existing session.</span></span>|
|[<span data-ttu-id="deadd-115">Atualizar Sessão</span><span class="sxs-lookup"><span data-stu-id="deadd-115">Refresh Session</span></span>](../api/workbook_refreshsession.md) | <span data-ttu-id="deadd-116">None</span><span class="sxs-lookup"><span data-stu-id="deadd-116">None</span></span> |<span data-ttu-id="deadd-117">Atualizar uma sessão existente.</span><span class="sxs-lookup"><span data-stu-id="deadd-117">Refresh an existing session.</span></span>|


## <a name="relationships"></a><span data-ttu-id="deadd-118">Relações</span><span class="sxs-lookup"><span data-stu-id="deadd-118">Relationships</span></span>
| <span data-ttu-id="deadd-119">Relação</span><span class="sxs-lookup"><span data-stu-id="deadd-119">Relationship</span></span> | <span data-ttu-id="deadd-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="deadd-120">Type</span></span>   |<span data-ttu-id="deadd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="deadd-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="deadd-122">names</span><span class="sxs-lookup"><span data-stu-id="deadd-122">names</span></span>|<span data-ttu-id="deadd-123">Coleção [NamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="deadd-123">[NamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="deadd-p101">Representa uma coleção de itens denominados de escopo da pasta de trabalho (chamados intervalos e constantes). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="deadd-p101">Represents a collection of workbook scoped named items (named ranges and constants). Read-only.</span></span>|
|<span data-ttu-id="deadd-126">tabelas</span><span class="sxs-lookup"><span data-stu-id="deadd-126">tables</span></span>|<span data-ttu-id="deadd-127">Coleção [Table](table.md)</span><span class="sxs-lookup"><span data-stu-id="deadd-127">[Table](table.md) collection</span></span>|<span data-ttu-id="deadd-p102">Representa uma coleção de tabelas associadas à pasta de trabalho. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="deadd-p102">Represents a collection of tables associated with the workbook. Read-only.</span></span>|
|<span data-ttu-id="deadd-130">worksheets</span><span class="sxs-lookup"><span data-stu-id="deadd-130">worksheets</span></span>|<span data-ttu-id="deadd-131">Coleção [Worksheet](worksheet.md)</span><span class="sxs-lookup"><span data-stu-id="deadd-131">[Worksheet](worksheet.md) collection</span></span>|<span data-ttu-id="deadd-p103">Representa uma coleção de planilhas associadas à pasta de trabalho. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="deadd-p103">Represents a collection of worksheets associated with the workbook. Read-only.</span></span>|

## <a name="functions"></a><span data-ttu-id="deadd-134">Funções</span><span class="sxs-lookup"><span data-stu-id="deadd-134">Functions</span></span>

<span data-ttu-id="deadd-135">[Funções do Excel](#functions): Invoque uma função de pasta de trabalho usando a sintaxe `POST /workbook/functions/{function-name}` e fornecendo os argumentos de função no corpo usando um objeto JSON.</span><span class="sxs-lookup"><span data-stu-id="deadd-135">[Excel functions](#functions): Invoke a workbook function using the syntax `POST /workbook/functions/{function-name}` and providing the function argument(s) in the body using a JSON object. The function's resulting  and any  strings are returned in the function result object. The  value of  indicates successful execution of the function.</span></span> <span data-ttu-id="deadd-136">O `value` resultante da função e quaisquer cadeias de caracteres `error` são retornados no objeto de resultado de função.</span><span class="sxs-lookup"><span data-stu-id="deadd-136">The function's resulting `value` and any `error` strings are returned in the function result object.</span></span> <span data-ttu-id="deadd-137">O valor `error` de `null` indica a execução bem-sucedida da função.</span><span class="sxs-lookup"><span data-stu-id="deadd-137">The `error` value of `null` indicates successful execution of the function.</span></span> 

<span data-ttu-id="deadd-138">A lista completa de funções com suporte está listada [aqui](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188).</span><span class="sxs-lookup"><span data-stu-id="deadd-138">The complete list of supported functions are listed here. Refer to the function signature for specific parameter names and data types.</span></span> <span data-ttu-id="deadd-139">Confira a assinatura de função para tipos de dados e nomes de parâmetro específicos.</span><span class="sxs-lookup"><span data-stu-id="deadd-139">The complete list of supported functions are listed here. Refer to the function signature for specific parameter names and data types.</span></span>

<span data-ttu-id="deadd-140">_Observações importantes:_</span><span class="sxs-lookup"><span data-stu-id="deadd-140">_Important notes:_</span></span> 
* <span data-ttu-id="deadd-141">O parâmetro de entrada do intervalo é fornecido usando um objeto range, em vez da cadeia de caracteres de endereço do intervalo.</span><span class="sxs-lookup"><span data-stu-id="deadd-141">The range input parameter is supplied using a range object instead of the range address string.</span></span>  
* <span data-ttu-id="deadd-142">O parâmetro index é indexado como -1, diferentemente do índice 0 usado na maioria das APIs.</span><span class="sxs-lookup"><span data-stu-id="deadd-142">The index parameter is 1-indexed unlike the 0-index used in most of the APIs.</span></span> 

<span data-ttu-id="deadd-143">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="deadd-143">Example:</span></span> 

<span data-ttu-id="deadd-144">No exemplo abaixo, a função `vlookup` é chamada passando o valor de pesquisa, o intervalo de entrada e o valor a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="deadd-144">In the below example, `vlookup` function is called by passing lookup value, input range and the value to be returned.</span></span> 

<span data-ttu-id="deadd-145">Solicitação:</span><span class="sxs-lookup"><span data-stu-id="deadd-145">Request:</span></span> 

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

<span data-ttu-id="deadd-146">Resposta:</span><span class="sxs-lookup"><span data-stu-id="deadd-146">Response:</span></span>

```http
HTTP code: 200, OK
content-type: application/json;odata.metadata 

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#workbookFunctionResult",
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/workbook/functions/vlookup()",
    "error": null,
    "value": "28.3"
}
```

<span data-ttu-id="deadd-147">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="deadd-147">Example:</span></span> 

<span data-ttu-id="deadd-148">No exemplo abaixo, a função `median` é chamada passando o(s) intervalo(s) de entrada em uma matriz.</span><span class="sxs-lookup"><span data-stu-id="deadd-148">In the below example, `median` function is called by passing the input range(s) in an array.</span></span> 

<span data-ttu-id="deadd-149">Solicitação:</span><span class="sxs-lookup"><span data-stu-id="deadd-149">Request:</span></span> 

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

<span data-ttu-id="deadd-150">Resposta:</span><span class="sxs-lookup"><span data-stu-id="deadd-150">Response:</span></span>

```http
HTTP code: 200, OK
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
