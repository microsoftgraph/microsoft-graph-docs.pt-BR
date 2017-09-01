# <a name="rangesort-apply"></a><span data-ttu-id="ef4c3-101">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="ef4c3-101">RangeSort: apply</span></span>

<span data-ttu-id="ef4c3-102">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="ef4c3-102">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="ef4c3-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="ef4c3-103">Permissions</span></span>
<span data-ttu-id="ef4c3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ef4c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ef4c3-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef4c3-106">Permission type</span></span>      | <span data-ttu-id="ef4c3-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ef4c3-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef4c3-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef4c3-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ef4c3-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ef4c3-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ef4c3-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef4c3-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef4c3-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef4c3-111">Not supported.</span></span>    |
|<span data-ttu-id="ef4c3-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef4c3-112">Application</span></span> | <span data-ttu-id="ef4c3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef4c3-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef4c3-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef4c3-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/sort/apply
POST /workbook/worksheets/{id|name}/range(<address>)/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="ef4c3-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef4c3-115">Request headers</span></span>
| <span data-ttu-id="ef4c3-116">Nome</span><span class="sxs-lookup"><span data-stu-id="ef4c3-116">Name</span></span>       | <span data-ttu-id="ef4c3-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef4c3-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ef4c3-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef4c3-118">Authorization</span></span>  | <span data-ttu-id="ef4c3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef4c3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef4c3-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef4c3-121">Request body</span></span>
<span data-ttu-id="ef4c3-122">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef4c3-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ef4c3-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ef4c3-123">Parameter</span></span>    | <span data-ttu-id="ef4c3-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef4c3-124">Type</span></span>   |<span data-ttu-id="ef4c3-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef4c3-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef4c3-126">campos</span><span class="sxs-lookup"><span data-stu-id="ef4c3-126">fields</span></span>|<span data-ttu-id="ef4c3-127">SortField</span><span class="sxs-lookup"><span data-stu-id="ef4c3-127">SortField</span></span>|<span data-ttu-id="ef4c3-128">A lista de condições para a classificação.</span><span class="sxs-lookup"><span data-stu-id="ef4c3-128">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="ef4c3-129">matchCase</span><span class="sxs-lookup"><span data-stu-id="ef4c3-129">matchCase</span></span>|<span data-ttu-id="ef4c3-130">booliano</span><span class="sxs-lookup"><span data-stu-id="ef4c3-130">boolean</span></span>|<span data-ttu-id="ef4c3-p103">Opcional. Define se o uso de maiúsculas ou minúsculas afeta a ordenação da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="ef4c3-p103">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="ef4c3-133">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="ef4c3-133">hasHeaders</span></span>|<span data-ttu-id="ef4c3-134">booliano</span><span class="sxs-lookup"><span data-stu-id="ef4c3-134">boolean</span></span>|<span data-ttu-id="ef4c3-p104">Opcional. Se o intervalo tem um cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="ef4c3-p104">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="ef4c3-137">orientation</span><span class="sxs-lookup"><span data-stu-id="ef4c3-137">orientation</span></span>|<span data-ttu-id="ef4c3-138">string</span><span class="sxs-lookup"><span data-stu-id="ef4c3-138">string</span></span>|<span data-ttu-id="ef4c3-p105">Opcional. Se a operação classifica linhas ou colunas.  Os valores possíveis são: `Rows` e `Columns`.</span><span class="sxs-lookup"><span data-stu-id="ef4c3-p105">Optional. Whether the operation is sorting rows or columns.  Possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="ef4c3-142">método</span><span class="sxs-lookup"><span data-stu-id="ef4c3-142">method</span></span>|<span data-ttu-id="ef4c3-143">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef4c3-143">string</span></span>|<span data-ttu-id="ef4c3-p106">Opcional. O método de ordenação usado pelos caracteres chineses.  Os valores possíveis são: `PinYin` e `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="ef4c3-p106">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="ef4c3-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef4c3-147">Response</span></span>

<span data-ttu-id="ef4c3-p107">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef4c3-p107">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef4c3-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef4c3-150">Example</span></span>
<span data-ttu-id="ef4c3-151">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="ef4c3-151">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ef4c3-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef4c3-152">Request</span></span>
<span data-ttu-id="ef4c3-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef4c3-153">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="ef4c3-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef4c3-154">Response</span></span>
<span data-ttu-id="ef4c3-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef4c3-155">Here is an example of the response.</span></span> 
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