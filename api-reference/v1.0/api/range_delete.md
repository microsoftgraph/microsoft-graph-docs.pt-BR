# <a name="range-delete"></a><span data-ttu-id="03e67-101">Range: delete</span><span class="sxs-lookup"><span data-stu-id="03e67-101">Range: delete</span></span>

<span data-ttu-id="03e67-102">Exclui as células associadas ao intervalo.</span><span class="sxs-lookup"><span data-stu-id="03e67-102">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="03e67-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="03e67-103">Permissions</span></span>
<span data-ttu-id="03e67-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="03e67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="03e67-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03e67-106">Permission type</span></span>      | <span data-ttu-id="03e67-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="03e67-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03e67-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03e67-108">Delegated (work or school account)</span></span> | <span data-ttu-id="03e67-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03e67-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="03e67-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03e67-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03e67-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03e67-111">Not supported.</span></span>    |
|<span data-ttu-id="03e67-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03e67-112">Application</span></span> | <span data-ttu-id="03e67-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03e67-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="03e67-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03e67-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/delete
POST /workbook/worksheets/{id|name}/range(<address>)/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="03e67-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03e67-115">Request headers</span></span>
| <span data-ttu-id="03e67-116">Nome</span><span class="sxs-lookup"><span data-stu-id="03e67-116">Name</span></span>       | <span data-ttu-id="03e67-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="03e67-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="03e67-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="03e67-118">Authorization</span></span>  | <span data-ttu-id="03e67-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03e67-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="03e67-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03e67-121">Request body</span></span>
<span data-ttu-id="03e67-122">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="03e67-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="03e67-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="03e67-123">Parameter</span></span>    | <span data-ttu-id="03e67-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="03e67-124">Type</span></span>   |<span data-ttu-id="03e67-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="03e67-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03e67-126">shift</span><span class="sxs-lookup"><span data-stu-id="03e67-126">shift</span></span>|<span data-ttu-id="03e67-127">string</span><span class="sxs-lookup"><span data-stu-id="03e67-127">string</span></span>|<span data-ttu-id="03e67-p103">Especifica como deslocar as células.  Os valores possíveis são: `Up` e `Left`.</span><span class="sxs-lookup"><span data-stu-id="03e67-p103">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="03e67-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="03e67-130">Response</span></span>

<span data-ttu-id="03e67-p104">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03e67-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03e67-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03e67-133">Example</span></span>
<span data-ttu-id="03e67-134">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="03e67-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="03e67-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03e67-135">Request</span></span>
<span data-ttu-id="03e67-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="03e67-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="03e67-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="03e67-137">Response</span></span>
<span data-ttu-id="03e67-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03e67-138">Here is an example of the response.</span></span> 
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
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->