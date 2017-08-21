# <a name="remove-member"></a><span data-ttu-id="301d1-101">Remover membro</span><span class="sxs-lookup"><span data-stu-id="301d1-101">Remove member</span></span>

<span data-ttu-id="301d1-p101">Use esta API para remover um membro de um grupo do Office 365, um grupo de segurança ou um grupo de segurança habilitado para email através da propriedade de navegação **members**. É possível remover usuários ou outros grupos.</span><span class="sxs-lookup"><span data-stu-id="301d1-p101">Use this API to remove a member from an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property. You can remove users or other groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="301d1-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="301d1-104">Prerequisites</span></span>
<span data-ttu-id="301d1-105">Um dos seguintes **escopos** é necessário para executar esta API: *Group.ReadWrite.All*, *Directory.ReadWrite.All* ou *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="301d1-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="301d1-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="301d1-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="301d1-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="301d1-107">Request headers</span></span>
| <span data-ttu-id="301d1-108">Nome</span><span class="sxs-lookup"><span data-stu-id="301d1-108">Name</span></span>       | <span data-ttu-id="301d1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="301d1-109">Type</span></span> | <span data-ttu-id="301d1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="301d1-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="301d1-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="301d1-111">Authorization</span></span>  | <span data-ttu-id="301d1-112">string</span><span class="sxs-lookup"><span data-stu-id="301d1-112">string</span></span>  | <span data-ttu-id="301d1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="301d1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="301d1-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="301d1-115">Request body</span></span>
<span data-ttu-id="301d1-116">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="301d1-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="301d1-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="301d1-117">Response</span></span>

<span data-ttu-id="301d1-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="301d1-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="301d1-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="301d1-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="301d1-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="301d1-121">Request</span></span>
<span data-ttu-id="301d1-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="301d1-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="301d1-123">Na solicitação, especifique a `id` do objeto diretório que deseja remover após o segmento $ref.</span><span class="sxs-lookup"><span data-stu-id="301d1-123">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

##### <a name="response"></a><span data-ttu-id="301d1-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="301d1-124">Response</span></span>
<span data-ttu-id="301d1-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="301d1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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