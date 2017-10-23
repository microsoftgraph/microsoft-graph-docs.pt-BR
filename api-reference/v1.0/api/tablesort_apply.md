# <a name="tablesort-apply"></a><span data-ttu-id="94277-101">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="94277-101">TableSort: apply</span></span>

<span data-ttu-id="94277-102">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="94277-102">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="94277-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="94277-103">Permissions</span></span>
<span data-ttu-id="94277-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="94277-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="94277-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94277-106">Permission type</span></span>      | <span data-ttu-id="94277-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94277-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94277-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94277-108">Delegated (work or school account)</span></span> | <span data-ttu-id="94277-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94277-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="94277-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94277-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94277-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94277-111">Not supported.</span></span>    |
|<span data-ttu-id="94277-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94277-112">Application</span></span> | <span data-ttu-id="94277-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94277-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="94277-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94277-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="94277-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94277-115">Request headers</span></span>
| <span data-ttu-id="94277-116">Nome</span><span class="sxs-lookup"><span data-stu-id="94277-116">Name</span></span>       | <span data-ttu-id="94277-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="94277-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="94277-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="94277-118">Authorization</span></span>  | <span data-ttu-id="94277-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94277-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94277-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94277-121">Request body</span></span>
<span data-ttu-id="94277-122">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94277-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="94277-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="94277-123">Parameter</span></span>    | <span data-ttu-id="94277-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="94277-124">Type</span></span>   |<span data-ttu-id="94277-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="94277-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94277-126">campos</span><span class="sxs-lookup"><span data-stu-id="94277-126">fields</span></span>|<span data-ttu-id="94277-127">SortField</span><span class="sxs-lookup"><span data-stu-id="94277-127">SortField</span></span>|<span data-ttu-id="94277-128">A lista de condições para a classificação.</span><span class="sxs-lookup"><span data-stu-id="94277-128">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="94277-129">matchCase</span><span class="sxs-lookup"><span data-stu-id="94277-129">matchCase</span></span>|<span data-ttu-id="94277-130">booliano</span><span class="sxs-lookup"><span data-stu-id="94277-130">boolean</span></span>|<span data-ttu-id="94277-p103">Opcional. Define se o uso de maiúsculas ou minúsculas afeta a ordenação da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="94277-p103">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="94277-133">method</span><span class="sxs-lookup"><span data-stu-id="94277-133">method</span></span>|<span data-ttu-id="94277-134">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94277-134">string</span></span>|<span data-ttu-id="94277-p104">Opcional. O método de ordenação usado pelos caracteres chineses.  Os valores possíveis são: `PinYin` e `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="94277-p104">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="94277-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="94277-138">Response</span></span>

<span data-ttu-id="94277-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94277-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94277-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94277-141">Example</span></span>
<span data-ttu-id="94277-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="94277-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="94277-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94277-143">Request</span></span>
<span data-ttu-id="94277-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94277-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply
Content-type: application/json
Content-length: 298

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
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="94277-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="94277-145">Response</span></span>
<span data-ttu-id="94277-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94277-146">Here is an example of the response.</span></span> 
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
  "description": "TableSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->