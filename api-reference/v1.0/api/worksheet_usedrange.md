# <a name="worksheet-usedrange"></a><span data-ttu-id="97a8b-101">Worksheet: UsedRange</span><span class="sxs-lookup"><span data-stu-id="97a8b-101">Worksheet: UsedRange</span></span>

<span data-ttu-id="97a8b-p101">O intervalo usado é o menor intervalo que abrange todas as células que têm um valor ou uma formatação atribuído a elas. Se a planilha estiver em branco, esta função retorna a célula superior esquerda.</span><span class="sxs-lookup"><span data-stu-id="97a8b-p101">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="97a8b-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="97a8b-104">Permissions</span></span>
<span data-ttu-id="97a8b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="97a8b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="97a8b-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97a8b-107">Permission type</span></span>      | <span data-ttu-id="97a8b-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97a8b-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97a8b-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97a8b-109">Delegated (work or school account)</span></span> | <span data-ttu-id="97a8b-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97a8b-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="97a8b-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97a8b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97a8b-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97a8b-112">Not supported.</span></span>    |
|<span data-ttu-id="97a8b-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97a8b-113">Application</span></span> | <span data-ttu-id="97a8b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97a8b-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="97a8b-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97a8b-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/usedRange

```

## <a name="function-parameters"></a><span data-ttu-id="97a8b-116">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="97a8b-116">Function parameters</span></span>
<span data-ttu-id="97a8b-117">Na URL da solicitação, você pode fornecer parâmetros opcionais.</span><span class="sxs-lookup"><span data-stu-id="97a8b-117">In the request URL you may provide optional parameters.</span></span>

| <span data-ttu-id="97a8b-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="97a8b-118">Parameter</span></span>    | <span data-ttu-id="97a8b-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="97a8b-119">Type</span></span>   |<span data-ttu-id="97a8b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="97a8b-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97a8b-121">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="97a8b-121">valuesOnly</span></span>|<span data-ttu-id="97a8b-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="97a8b-122">Boolean</span></span>|<span data-ttu-id="97a8b-p103">Opcional. Considera apenas as células com valores como células usadas (ignora a formatação).</span><span class="sxs-lookup"><span data-stu-id="97a8b-p103">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="97a8b-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97a8b-125">Request headers</span></span>
| <span data-ttu-id="97a8b-126">Nome</span><span class="sxs-lookup"><span data-stu-id="97a8b-126">Name</span></span>       | <span data-ttu-id="97a8b-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="97a8b-127">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="97a8b-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="97a8b-128">Authorization</span></span>  | <span data-ttu-id="97a8b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97a8b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="97a8b-131">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="97a8b-131">Workbook-Session-Id</span></span>  | <span data-ttu-id="97a8b-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="97a8b-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="97a8b-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97a8b-134">Request body</span></span>
<span data-ttu-id="97a8b-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="97a8b-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97a8b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="97a8b-136">Response</span></span>

<span data-ttu-id="97a8b-137">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97a8b-137">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97a8b-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97a8b-138">Example</span></span>
<span data-ttu-id="97a8b-139">Aqui está um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="97a8b-139">Here is an example that shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="97a8b-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97a8b-140">Request</span></span>
<span data-ttu-id="97a8b-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97a8b-141">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange
```

##### <a name="response"></a><span data-ttu-id="97a8b-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="97a8b-142">Response</span></span>
<span data-ttu-id="97a8b-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97a8b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value"
}
```

<span data-ttu-id="97a8b-146">Como alternativa, essa função pode ser chamada com o `valuesOnly` parâmetro opcional.</span><span class="sxs-lookup"><span data-stu-id="97a8b-146">Alternatively, this function can be called with the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="97a8b-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97a8b-147">Request</span></span>
<span data-ttu-id="97a8b-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97a8b-148">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="97a8b-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="97a8b-149">Response</span></span>
<span data-ttu-id="97a8b-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97a8b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
