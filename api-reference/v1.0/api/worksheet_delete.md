# <a name="worksheet-delete"></a><span data-ttu-id="7c266-101">Worksheet: delete</span><span class="sxs-lookup"><span data-stu-id="7c266-101">Worksheet: delete</span></span>

<span data-ttu-id="7c266-102">Exclui a planilha da pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="7c266-102">Deletes the worksheet from the workbook.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7c266-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7c266-103">Prerequisites</span></span>
<span data-ttu-id="7c266-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="7c266-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="7c266-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c266-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="7c266-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c266-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/delete

```
## <a name="request-headers"></a><span data-ttu-id="7c266-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c266-107">Request headers</span></span>
| <span data-ttu-id="7c266-108">Nome</span><span class="sxs-lookup"><span data-stu-id="7c266-108">Name</span></span>       | <span data-ttu-id="7c266-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c266-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7c266-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c266-110">Authorization</span></span>  | <span data-ttu-id="7c266-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c266-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="7c266-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c266-113">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7c266-114">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c266-114">Response</span></span>

<span data-ttu-id="7c266-p102">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c266-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c266-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c266-117">Example</span></span>
<span data-ttu-id="7c266-118">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7c266-118">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7c266-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c266-119">Request</span></span>
<span data-ttu-id="7c266-120">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c266-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/delete
```

##### <a name="response"></a><span data-ttu-id="7c266-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c266-121">Response</span></span>
<span data-ttu-id="7c266-122">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c266-122">Here is an example of the response.</span></span> 
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
  "description": "Worksheet: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->