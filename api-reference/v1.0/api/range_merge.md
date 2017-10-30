# <a name="range-merge"></a><span data-ttu-id="ac617-101">Range: merge</span><span class="sxs-lookup"><span data-stu-id="ac617-101">Range: merge</span></span>

<span data-ttu-id="ac617-102">Mescla as células do intervalo em uma região da planilha.</span><span class="sxs-lookup"><span data-stu-id="ac617-102">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="ac617-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="ac617-103">Permissions</span></span>
<span data-ttu-id="ac617-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ac617-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ac617-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac617-106">Permission type</span></span>      | <span data-ttu-id="ac617-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ac617-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac617-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac617-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ac617-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ac617-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ac617-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac617-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac617-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac617-111">Not supported.</span></span>    |
|<span data-ttu-id="ac617-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac617-112">Application</span></span> | <span data-ttu-id="ac617-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac617-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac617-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac617-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/merge
POST /workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="ac617-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac617-115">Request headers</span></span>
| <span data-ttu-id="ac617-116">Nome</span><span class="sxs-lookup"><span data-stu-id="ac617-116">Name</span></span>       | <span data-ttu-id="ac617-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac617-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ac617-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac617-118">Authorization</span></span>  | <span data-ttu-id="ac617-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac617-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac617-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac617-121">Request body</span></span>
<span data-ttu-id="ac617-122">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac617-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ac617-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ac617-123">Parameter</span></span>    | <span data-ttu-id="ac617-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac617-124">Type</span></span>   |<span data-ttu-id="ac617-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac617-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac617-126">across</span><span class="sxs-lookup"><span data-stu-id="ac617-126">across</span></span>|<span data-ttu-id="ac617-127">booliano</span><span class="sxs-lookup"><span data-stu-id="ac617-127">boolean</span></span>|<span data-ttu-id="ac617-p103">Opcional. Defina true para mesclar células em todas as linhas do intervalo especificado como células mescladas separadamente. O valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="ac617-p103">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="ac617-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac617-131">Response</span></span>

<span data-ttu-id="ac617-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac617-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac617-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac617-134">Example</span></span>
<span data-ttu-id="ac617-135">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="ac617-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ac617-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac617-136">Request</span></span>
<span data-ttu-id="ac617-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac617-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
}
```

##### <a name="response"></a><span data-ttu-id="ac617-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac617-138">Response</span></span>
<span data-ttu-id="ac617-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac617-139">Here is an example of the response.</span></span> 
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
  "description": "Range: merge",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->