---
title: Listar contatos
description: Obter uma coleção de contatos da pasta padrão de contatos do usuário conectado.
author: kevinbellinger
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1d5d12fc90bd713ec4df1f96d69a9bf0c74e880b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050217"
---
# <a name="list-contacts"></a><span data-ttu-id="d725f-103">Listar contatos</span><span class="sxs-lookup"><span data-stu-id="d725f-103">List contacts</span></span>

<span data-ttu-id="d725f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d725f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d725f-105">Obter uma coleção de contatos da pasta padrão de contatos do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="d725f-105">Get a contact collection from the default contacts folder of the signed-in user.</span></span>

<span data-ttu-id="d725f-106">Há duas situações em que um aplicativo pode obter contatos na pasta de contatos de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="d725f-106">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="d725f-107">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="d725f-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="d725f-108">Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário, e outro usuário tiver compartilhado uma pasta de contatos com esse usuário, ou tiver concedido acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="d725f-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="d725f-109">Confira [detalhes e um exemplo](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="d725f-109">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="d725f-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="d725f-110">Permissions</span></span>
<span data-ttu-id="d725f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d725f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d725f-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d725f-113">Permission type</span></span>      | <span data-ttu-id="d725f-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d725f-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d725f-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d725f-115">Delegated (work or school account)</span></span> | <span data-ttu-id="d725f-116">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d725f-116">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="d725f-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d725f-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d725f-118">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d725f-118">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="d725f-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d725f-119">Application</span></span> | <span data-ttu-id="d725f-120">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d725f-120">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d725f-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d725f-121">HTTP request</span></span>

<span data-ttu-id="d725f-122">Para obter todos os contatos na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="d725f-122">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="d725f-123">Para obter os contatos em uma pasta específica na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="d725f-123">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolders/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d725f-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d725f-124">Optional query parameters</span></span>
<span data-ttu-id="d725f-125">Você pode usar o `$filter`parâmetro de consulta para filtrar contatos com base em seus endereços de email:</span><span class="sxs-lookup"><span data-stu-id="d725f-125">You can use the `$filter` query parameter to filter contacts based on their email addresses:</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

<span data-ttu-id="d725f-126">Observe que você pode usar `$filter`, `any`, e o `eq` operador apenas na subpropriedade de **endereço** das instâncias em uma coleção **emailAddresses**.</span><span class="sxs-lookup"><span data-stu-id="d725f-126">Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection.</span></span> <span data-ttu-id="d725f-127">Ou seja, você não pode filtrar o **nome** ou qualquer outra subpropriedade de uma instância de **emailAddresses**, nem pode aplicar qualquer outro operador ou função com `filter`, como `ne`, `le` e `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="d725f-127">That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.</span></span>

<span data-ttu-id="d725f-128">Para obter informações gerais sobre o `$filter`parâmetro de consulta, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d725f-128">For general information on the `$filter` query parameter, see [OData query parameters](/graph/query-parameters).</span></span>



## <a name="request-headers"></a><span data-ttu-id="d725f-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d725f-129">Request headers</span></span>
| <span data-ttu-id="d725f-130">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d725f-130">Header</span></span>       | <span data-ttu-id="d725f-131">Valor</span><span class="sxs-lookup"><span data-stu-id="d725f-131">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d725f-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="d725f-132">Authorization</span></span>  | <span data-ttu-id="d725f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d725f-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d725f-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d725f-135">Content-Type</span></span>   | <span data-ttu-id="d725f-136">application/json</span><span class="sxs-lookup"><span data-stu-id="d725f-136">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d725f-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d725f-137">Request body</span></span>
<span data-ttu-id="d725f-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d725f-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d725f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d725f-139">Response</span></span>

<span data-ttu-id="d725f-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d725f-140">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d725f-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d725f-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d725f-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d725f-142">Request</span></span>
<span data-ttu-id="d725f-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d725f-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d725f-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="d725f-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_contacts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/contacts
```
# <a name="c"></a>[<span data-ttu-id="d725f-145">C#</span><span class="sxs-lookup"><span data-stu-id="d725f-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-contacts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d725f-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d725f-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-contacts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d725f-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d725f-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-contacts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d725f-148">Java</span><span class="sxs-lookup"><span data-stu-id="d725f-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-contacts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="d725f-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="d725f-149">Response</span></span>
<span data-ttu-id="d725f-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d725f-150">Here is an example of the response.</span></span> <span data-ttu-id="d725f-151">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d725f-151">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "datetime-value",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

