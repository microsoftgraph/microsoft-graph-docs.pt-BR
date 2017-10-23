# <a name="delete-contact"></a><span data-ttu-id="a805d-101">Excluir contato</span><span class="sxs-lookup"><span data-stu-id="a805d-101">Delete contact</span></span>

<span data-ttu-id="a805d-102">Exclui um contato.</span><span class="sxs-lookup"><span data-stu-id="a805d-102">Delete a contact.</span></span>
## <a name="permissions"></a><span data-ttu-id="a805d-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="a805d-103">Permissions</span></span>
<span data-ttu-id="a805d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a805d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a805d-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a805d-106">Permission type</span></span>      | <span data-ttu-id="a805d-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a805d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a805d-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a805d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a805d-109">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a805d-109">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a805d-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a805d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a805d-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a805d-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a805d-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a805d-112">Application</span></span> | <span data-ttu-id="a805d-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a805d-113">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a805d-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a805d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a805d-115">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="a805d-115">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="a805d-116">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) de nível superior do usuário.</span><span class="sxs-lookup"><span data-stu-id="a805d-116">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="a805d-p102">Um [contact](../resources/contact.md) incluso em uma pasta filha de uma [contactFolder](../resources/mailfolder.md). O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="a805d-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a805d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a805d-119">Request headers</span></span>
| <span data-ttu-id="a805d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a805d-120">Header</span></span>       | <span data-ttu-id="a805d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a805d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a805d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a805d-122">Authorization</span></span>  | <span data-ttu-id="a805d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a805d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a805d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a805d-125">Request body</span></span>
<span data-ttu-id="a805d-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a805d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a805d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a805d-127">Response</span></span>

<span data-ttu-id="a805d-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a805d-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a805d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a805d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a805d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a805d-131">Request</span></span>
<span data-ttu-id="a805d-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a805d-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="a805d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a805d-133">Response</span></span>
<span data-ttu-id="a805d-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a805d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
