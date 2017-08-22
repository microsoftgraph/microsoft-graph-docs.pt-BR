# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="2b03c-101">Excluir inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="2b03c-101">Delete inferenceClassificationOverride</span></span>

<span data-ttu-id="2b03c-102">Exclua uma substituição especificada de acordo com sua ID.</span><span class="sxs-lookup"><span data-stu-id="2b03c-102">Delete an override specified by its ID.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2b03c-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2b03c-103">Prerequisites</span></span>
<span data-ttu-id="2b03c-104">Os seguintes **escopos** são necessários para executar esta API: *Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="2b03c-104">The following **scopes** are required to execute this API: *Mail.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="2b03c-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b03c-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2b03c-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b03c-106">Request headers</span></span>
| <span data-ttu-id="2b03c-107">Nome</span><span class="sxs-lookup"><span data-stu-id="2b03c-107">Name</span></span>       | <span data-ttu-id="2b03c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b03c-108">Type</span></span> | <span data-ttu-id="2b03c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b03c-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2b03c-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b03c-110">Authorization</span></span>  | <span data-ttu-id="2b03c-111">string</span><span class="sxs-lookup"><span data-stu-id="2b03c-111">string</span></span>  | <span data-ttu-id="2b03c-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b03c-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b03c-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b03c-114">Request body</span></span>
<span data-ttu-id="2b03c-115">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2b03c-115">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b03c-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b03c-116">Response</span></span>

<span data-ttu-id="2b03c-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b03c-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b03c-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b03c-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b03c-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b03c-120">Request</span></span>
<span data-ttu-id="2b03c-121">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b03c-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
##### <a name="response"></a><span data-ttu-id="2b03c-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b03c-122">Response</span></span>
<span data-ttu-id="2b03c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2b03c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->