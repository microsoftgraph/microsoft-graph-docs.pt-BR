# <a name="remove-owner"></a><span data-ttu-id="51bfb-101">Remover proprietário</span><span class="sxs-lookup"><span data-stu-id="51bfb-101">Remove owner</span></span>

<span data-ttu-id="51bfb-102">Use esta API para remover um proprietário de um grupo do Office 365, um grupo de segurança ou um grupo de segurança habilitado para email através da propriedade de navegação owners.</span><span class="sxs-lookup"><span data-stu-id="51bfb-102">Use this API to remove an owner from an Office 365 group, a security group or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51bfb-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="51bfb-103">Prerequisites</span></span>
<span data-ttu-id="51bfb-104">Um dos seguintes **escopos** é necessário para executar esta API: *Group.ReadWrite.All*, *Directory.ReadWrite.All* ou *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="51bfb-104">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="51bfb-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51bfb-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="51bfb-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51bfb-106">Request headers</span></span>
| <span data-ttu-id="51bfb-107">Nome</span><span class="sxs-lookup"><span data-stu-id="51bfb-107">Name</span></span>       | <span data-ttu-id="51bfb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="51bfb-108">Type</span></span> | <span data-ttu-id="51bfb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="51bfb-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="51bfb-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="51bfb-110">Authorization</span></span>  | <span data-ttu-id="51bfb-111">string</span><span class="sxs-lookup"><span data-stu-id="51bfb-111">string</span></span>  | <span data-ttu-id="51bfb-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51bfb-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51bfb-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51bfb-114">Request body</span></span>
<span data-ttu-id="51bfb-115">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="51bfb-115">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51bfb-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="51bfb-116">Response</span></span>

<span data-ttu-id="51bfb-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51bfb-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51bfb-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51bfb-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="51bfb-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51bfb-120">Request</span></span>
<span data-ttu-id="51bfb-121">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51bfb-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/owners/{id}/$ref
```
<span data-ttu-id="51bfb-122">Na solicitação, especifique a `id` do objeto diretório que deseja remover após o segmento $ref.</span><span class="sxs-lookup"><span data-stu-id="51bfb-122">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

##### <a name="response"></a><span data-ttu-id="51bfb-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="51bfb-123">Response</span></span>
<span data-ttu-id="51bfb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51bfb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
