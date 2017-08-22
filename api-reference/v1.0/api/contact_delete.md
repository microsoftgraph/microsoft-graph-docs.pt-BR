# <a name="delete-contact"></a><span data-ttu-id="32573-101">Excluir contato</span><span class="sxs-lookup"><span data-stu-id="32573-101">Delete contact</span></span>

<span data-ttu-id="32573-102">Exclui um contato.</span><span class="sxs-lookup"><span data-stu-id="32573-102">Delete a contact.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="32573-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="32573-103">Prerequisites</span></span>
<span data-ttu-id="32573-104">Um dos seguintes **escopos** é necessário para executar esta API: *Contacts.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="32573-104">One of the following **scopes** is required to execute this API: *Contacts.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="32573-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32573-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="32573-106">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="32573-106">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="32573-107">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) de nível superior do usuário.</span><span class="sxs-lookup"><span data-stu-id="32573-107">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="32573-p101">Um [contact](../resources/contact.md) incluso em uma pasta filha de uma [contactFolder](../resources/mailfolder.md). O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="32573-p101">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="32573-110">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32573-110">Request headers</span></span>
| <span data-ttu-id="32573-111">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="32573-111">Header</span></span>       | <span data-ttu-id="32573-112">Valor</span><span class="sxs-lookup"><span data-stu-id="32573-112">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="32573-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="32573-113">Authorization</span></span>  | <span data-ttu-id="32573-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32573-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="32573-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32573-116">Request body</span></span>
<span data-ttu-id="32573-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="32573-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32573-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="32573-118">Response</span></span>

<span data-ttu-id="32573-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32573-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32573-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32573-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="32573-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32573-122">Request</span></span>
<span data-ttu-id="32573-123">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="32573-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="32573-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="32573-124">Response</span></span>
<span data-ttu-id="32573-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32573-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
