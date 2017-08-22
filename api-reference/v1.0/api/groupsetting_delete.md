# <a name="delete-a-group-setting"></a><span data-ttu-id="34737-101">Excluir uma configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="34737-101">Delete a group setting</span></span>

<span data-ttu-id="34737-102">Excluir uma configuração de grupo.</span><span class="sxs-lookup"><span data-stu-id="34737-102">Delete a group setting.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34737-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="34737-103">Prerequisites</span></span>

<span data-ttu-id="34737-104">Um dos seguintes **escopos** é obrigatório para executar esta API: *Directory.ReadWrite.All* ou *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="34737-104">One of the following **scopes** is required to execute this API: *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

> <span data-ttu-id="34737-105">Observação: Somente os administradores do locatário têm permissões para executar operações de criação, atualização e exclusão.</span><span class="sxs-lookup"><span data-stu-id="34737-105">Note: Only tenant admins have permissions to perform create, update, and delete operations.</span></span>

## <a name="http-request"></a><span data-ttu-id="34737-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34737-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupSettings/{id}
DELETE /groups/{id}/settings/{id}

```

## <a name="request-headers"></a><span data-ttu-id="34737-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34737-107">Request headers</span></span>

| <span data-ttu-id="34737-108">Nome</span><span class="sxs-lookup"><span data-stu-id="34737-108">Name</span></span> | <span data-ttu-id="34737-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="34737-109">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="34737-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="34737-110">Authorization</span></span>  | <span data-ttu-id="34737-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34737-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="34737-113">Content-Type</span><span class="sxs-lookup"><span data-stu-id="34737-113">Content-Type</span></span>  | <span data-ttu-id="34737-114">application/json</span><span class="sxs-lookup"><span data-stu-id="34737-114">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="34737-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34737-115">Request body</span></span>
<span data-ttu-id="34737-116">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="34737-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34737-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="34737-117">Response</span></span>

<span data-ttu-id="34737-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34737-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34737-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34737-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="34737-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34737-121">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_groupsetting"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a><span data-ttu-id="34737-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="34737-122">Response</span></span>
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
  "description": "Delete groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->