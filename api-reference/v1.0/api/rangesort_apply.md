# <a name="rangesort-apply"></a><span data-ttu-id="0024b-101">RangeSort: aplicar</span><span class="sxs-lookup"><span data-stu-id="0024b-101">RangeSort: apply</span></span>

<span data-ttu-id="0024b-102">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="0024b-102">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="0024b-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="0024b-103">Permissions</span></span>
<span data-ttu-id="0024b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0024b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0024b-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0024b-106">Permission type</span></span>      | <span data-ttu-id="0024b-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0024b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0024b-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0024b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="0024b-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0024b-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0024b-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0024b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0024b-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0024b-111">Not supported.</span></span>    |
|<span data-ttu-id="0024b-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0024b-112">Application</span></span> | <span data-ttu-id="0024b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0024b-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0024b-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0024b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="0024b-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0024b-115">Request headers</span></span>
| <span data-ttu-id="0024b-116">Nome</span><span class="sxs-lookup"><span data-stu-id="0024b-116">Name</span></span>       | <span data-ttu-id="0024b-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="0024b-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0024b-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="0024b-118">Authorization</span></span>  | <span data-ttu-id="0024b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0024b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0024b-121">Pasta de trabalho-Sessão-Id</span><span class="sxs-lookup"><span data-stu-id="0024b-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="0024b-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="0024b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0024b-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0024b-124">Request body</span></span>
<span data-ttu-id="0024b-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0024b-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0024b-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0024b-126">Parameter</span></span>    | <span data-ttu-id="0024b-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="0024b-127">Type</span></span>   |<span data-ttu-id="0024b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="0024b-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0024b-129">campos</span><span class="sxs-lookup"><span data-stu-id="0024b-129">fields</span></span>|<span data-ttu-id="0024b-130">Coleção WorkbookSortField</span><span class="sxs-lookup"><span data-stu-id="0024b-130">WorkbookSortField collection</span></span>|<span data-ttu-id="0024b-131">A lista de condições para a classificação.</span><span class="sxs-lookup"><span data-stu-id="0024b-131">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="0024b-132">matchCase</span><span class="sxs-lookup"><span data-stu-id="0024b-132">matchCase</span></span>|<span data-ttu-id="0024b-133">booliano</span><span class="sxs-lookup"><span data-stu-id="0024b-133">boolean</span></span>|<span data-ttu-id="0024b-p104">Opcional. Define se o uso de maiúsculas ou minúsculas afeta a ordenação da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="0024b-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="0024b-136">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="0024b-136">hasHeaders</span></span>|<span data-ttu-id="0024b-137">booliano</span><span class="sxs-lookup"><span data-stu-id="0024b-137">boolean</span></span>|<span data-ttu-id="0024b-p105">Opcional. Se o intervalo tem um cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="0024b-p105">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="0024b-140">orientação</span><span class="sxs-lookup"><span data-stu-id="0024b-140">orientation</span></span>|<span data-ttu-id="0024b-141">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="0024b-141">string</span></span>|<span data-ttu-id="0024b-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0024b-142">Optional.</span></span> <span data-ttu-id="0024b-143">Se a operação está classificando linhas ou colunas.</span><span class="sxs-lookup"><span data-stu-id="0024b-143">Optional. Whether the operation is sorting rows or columns.  Possible values are: , .</span></span>  <span data-ttu-id="0024b-144">Os valores possíveis são: `Rows`, `Columns`.</span><span class="sxs-lookup"><span data-stu-id="0024b-144">The possible values are:</span></span>|
|<span data-ttu-id="0024b-145">método</span><span class="sxs-lookup"><span data-stu-id="0024b-145">method</span></span>|<span data-ttu-id="0024b-146">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="0024b-146">string</span></span>|<span data-ttu-id="0024b-147">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0024b-147">Optional.</span></span> <span data-ttu-id="0024b-148">O método de ordenação usado para caracteres chineses.</span><span class="sxs-lookup"><span data-stu-id="0024b-148">Optional. The ordering method used for Chinese characters.  Possible values are: , .</span></span>  <span data-ttu-id="0024b-149">Os valores possíveis são: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="0024b-149">The possible values are:</span></span>|

## <a name="response"></a><span data-ttu-id="0024b-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="0024b-150">Response</span></span>

<span data-ttu-id="0024b-p108">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0024b-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0024b-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0024b-153">Example</span></span>
<span data-ttu-id="0024b-154">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0024b-154">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0024b-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0024b-155">Request</span></span>
<span data-ttu-id="0024b-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0024b-156">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort/apply
Content-type: application/json
Content-length: 358

{
  "fields": [
    {
      "key": 99,
      "sortOn": "sortOn-value",
      "ascending": true,
      "color": "color-value",
      "dataOption": "dataOption-value",
      "icon": {
        "set": "set-value",
        "index": 99
      }
    }
  ],
  "matchCase": true,
  "hasHeaders": true,
  "orientation": "orientation-value",
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="0024b-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="0024b-157">Response</span></span>
<span data-ttu-id="0024b-158">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0024b-158">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->