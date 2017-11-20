# <a name="rangesort-apply"></a><span data-ttu-id="2841b-101">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="2841b-101">RangeSort: apply</span></span>

<span data-ttu-id="2841b-102">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="2841b-102">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="2841b-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="2841b-103">Permissions</span></span>
<span data-ttu-id="2841b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2841b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2841b-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2841b-106">Permission type</span></span>      | <span data-ttu-id="2841b-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2841b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2841b-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2841b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2841b-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2841b-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2841b-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2841b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2841b-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2841b-111">Not supported.</span></span>    |
|<span data-ttu-id="2841b-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2841b-112">Application</span></span> | <span data-ttu-id="2841b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2841b-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2841b-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2841b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="2841b-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2841b-115">Request headers</span></span>
| <span data-ttu-id="2841b-116">Nome</span><span class="sxs-lookup"><span data-stu-id="2841b-116">Name</span></span>       | <span data-ttu-id="2841b-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="2841b-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2841b-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="2841b-118">Authorization</span></span>  | <span data-ttu-id="2841b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2841b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2841b-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2841b-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="2841b-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="2841b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2841b-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2841b-124">Request body</span></span>
<span data-ttu-id="2841b-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2841b-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2841b-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2841b-126">Parameter</span></span>    | <span data-ttu-id="2841b-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="2841b-127">Type</span></span>   |<span data-ttu-id="2841b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="2841b-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2841b-129">campos</span><span class="sxs-lookup"><span data-stu-id="2841b-129">fields</span></span>|<span data-ttu-id="2841b-130">SortField</span><span class="sxs-lookup"><span data-stu-id="2841b-130">SortField</span></span>|<span data-ttu-id="2841b-131">A lista de condições para a classificação.</span><span class="sxs-lookup"><span data-stu-id="2841b-131">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="2841b-132">matchCase</span><span class="sxs-lookup"><span data-stu-id="2841b-132">matchCase</span></span>|<span data-ttu-id="2841b-133">booliano</span><span class="sxs-lookup"><span data-stu-id="2841b-133">boolean</span></span>|<span data-ttu-id="2841b-p104">Opcional. Define se o uso de maiúsculas ou minúsculas afeta a ordenação da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="2841b-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="2841b-136">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="2841b-136">hasHeaders</span></span>|<span data-ttu-id="2841b-137">booliano</span><span class="sxs-lookup"><span data-stu-id="2841b-137">boolean</span></span>|<span data-ttu-id="2841b-p105">Opcional. Se o intervalo tem um cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="2841b-p105">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="2841b-140">orientation</span><span class="sxs-lookup"><span data-stu-id="2841b-140">orientation</span></span>|<span data-ttu-id="2841b-141">string</span><span class="sxs-lookup"><span data-stu-id="2841b-141">string</span></span>|<span data-ttu-id="2841b-p106">Opcional. Se a operação classifica linhas ou colunas.  Os valores possíveis são: `Rows` e `Columns`.</span><span class="sxs-lookup"><span data-stu-id="2841b-p106">Optional. Whether the operation is sorting rows or columns.  Possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="2841b-145">método</span><span class="sxs-lookup"><span data-stu-id="2841b-145">method</span></span>|<span data-ttu-id="2841b-146">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2841b-146">string</span></span>|<span data-ttu-id="2841b-p107">Opcional. O método de ordenação usado pelos caracteres chineses.  Os valores possíveis são: `PinYin` e `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="2841b-p107">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="2841b-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="2841b-150">Response</span></span>

<span data-ttu-id="2841b-p108">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2841b-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2841b-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2841b-153">Example</span></span>
<span data-ttu-id="2841b-154">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2841b-154">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2841b-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2841b-155">Request</span></span>
<span data-ttu-id="2841b-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2841b-156">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/sort/apply
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

##### <a name="response"></a><span data-ttu-id="2841b-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="2841b-157">Response</span></span>
<span data-ttu-id="2841b-158">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2841b-158">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
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