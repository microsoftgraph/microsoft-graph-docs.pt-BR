---
title: Listar contatos
description: Obter uma coleção de contatos da pasta padrão de contatos do usuário conectado.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 55e00235ac6f1d983aed5f34bd553ef7ef3f05f1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460375"
---
# <a name="list-contacts"></a><span data-ttu-id="23b28-103">Listar contatos</span><span class="sxs-lookup"><span data-stu-id="23b28-103">List contacts</span></span>

<span data-ttu-id="23b28-104">Obter uma coleção de contatos da pasta padrão de contatos do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="23b28-104">Get a contact collection from the default contacts folder of the signed-in user.</span></span>

<span data-ttu-id="23b28-105">Há duas situações em que um aplicativo pode obter contatos na pasta de contatos de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="23b28-105">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="23b28-106">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="23b28-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="23b28-107">Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário, e outro usuário tiver compartilhado uma pasta de contatos com esse usuário, ou tiver concedido acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="23b28-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="23b28-108">Confira [detalhes e um exemplo](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="23b28-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="23b28-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="23b28-109">Permissions</span></span>
<span data-ttu-id="23b28-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23b28-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23b28-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23b28-112">Permission type</span></span>      | <span data-ttu-id="23b28-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="23b28-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23b28-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23b28-114">Delegated (work or school account)</span></span> | <span data-ttu-id="23b28-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23b28-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="23b28-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23b28-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23b28-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23b28-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="23b28-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23b28-118">Application</span></span> | <span data-ttu-id="23b28-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23b28-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="23b28-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23b28-120">HTTP request</span></span>

<span data-ttu-id="23b28-121">Para obter todos os contatos na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="23b28-121">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="23b28-122">Para obter os contatos em uma pasta específica na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="23b28-122">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="23b28-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="23b28-123">Optional query parameters</span></span>
<span data-ttu-id="23b28-124">Você pode usar o `$filter`parâmetro de consulta para filtrar contatos com base em seus endereços de email:</span><span class="sxs-lookup"><span data-stu-id="23b28-124">You can use the `$filter` query parameter to filter contacts based on their email addresses:</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

<span data-ttu-id="23b28-125">Observe que você pode usar `$filter`, `any`, e o `eq` operador apenas na subpropriedade de **endereço** das instâncias em uma coleção **emailAddresses**.</span><span class="sxs-lookup"><span data-stu-id="23b28-125">Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection.</span></span> <span data-ttu-id="23b28-126">Ou seja, você não pode filtrar o **nome** ou qualquer outra subpropriedade de uma instância de **emailAddresses**, nem pode aplicar qualquer outro operador ou função com `filter`, como `ne`, `le` e `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="23b28-126">That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.</span></span>

<span data-ttu-id="23b28-127">Para obter informações gerais sobre o `$filter`parâmetro de consulta, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="23b28-127">For general information on the `$filter` query parameter, see [OData query parameters](/graph/query-parameters).</span></span>



## <a name="request-headers"></a><span data-ttu-id="23b28-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23b28-128">Request headers</span></span>
| <span data-ttu-id="23b28-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="23b28-129">Header</span></span>       | <span data-ttu-id="23b28-130">Valor</span><span class="sxs-lookup"><span data-stu-id="23b28-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="23b28-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="23b28-131">Authorization</span></span>  | <span data-ttu-id="23b28-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23b28-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="23b28-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="23b28-134">Content-Type</span></span>   | <span data-ttu-id="23b28-135">application/json</span><span class="sxs-lookup"><span data-stu-id="23b28-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="23b28-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23b28-136">Request body</span></span>
<span data-ttu-id="23b28-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="23b28-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23b28-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="23b28-138">Response</span></span>

<span data-ttu-id="23b28-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23b28-139">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="23b28-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23b28-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="23b28-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23b28-141">Request</span></span>
<span data-ttu-id="23b28-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="23b28-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="23b28-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="23b28-143">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="23b28-144">C#</span><span class="sxs-lookup"><span data-stu-id="23b28-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contacts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="23b28-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="23b28-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contacts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="23b28-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23b28-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contacts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="23b28-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="23b28-147">Response</span></span>
<span data-ttu-id="23b28-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="23b28-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
