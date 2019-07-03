---
title: Listar contatos
description: Obter contatos na caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 92b017bd9bb9ffc9c9959e0ba38b60a5a0c9eea9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35452876"
---
# <a name="list-contacts"></a><span data-ttu-id="bd6ea-103">Listar contatos</span><span class="sxs-lookup"><span data-stu-id="bd6ea-103">List contacts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd6ea-104">Obter contatos na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="bd6ea-104">Get contacts in the user's mailbox.</span></span>

<span data-ttu-id="bd6ea-105">Há duas situações em que um aplicativo pode obter contatos na pasta de contatos de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="bd6ea-105">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="bd6ea-106">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="bd6ea-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="bd6ea-107">Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário, e outro usuário tiver compartilhado uma pasta de contatos com esse usuário, ou tiver concedido acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="bd6ea-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="bd6ea-108">Confira [detalhes e um exemplo](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="bd6ea-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="bd6ea-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="bd6ea-109">Permissions</span></span>
<span data-ttu-id="bd6ea-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd6ea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd6ea-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd6ea-112">Permission type</span></span>      | <span data-ttu-id="bd6ea-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bd6ea-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd6ea-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd6ea-114">Delegated (work or school account)</span></span> | <span data-ttu-id="bd6ea-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd6ea-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="bd6ea-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd6ea-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd6ea-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd6ea-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="bd6ea-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd6ea-118">Application</span></span> | <span data-ttu-id="bd6ea-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd6ea-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd6ea-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd6ea-120">HTTP request</span></span>

<span data-ttu-id="bd6ea-121">Para obter todos os contatos na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="bd6ea-121">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="bd6ea-122">Para obter os contatos em uma pasta específica na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="bd6ea-122">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bd6ea-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bd6ea-123">Optional query parameters</span></span>
<span data-ttu-id="bd6ea-124">Você pode usar o `$filter`parâmetro de consulta para filtrar contatos com base em seus endereços de email:</span><span class="sxs-lookup"><span data-stu-id="bd6ea-124">You can use the `$filter` query parameter to filter contacts based on their email addresses:</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

<span data-ttu-id="bd6ea-125">Observe que você pode usar `$filter`, `any`, e o `eq` operador apenas na subpropriedade de **endereço** das instâncias em uma coleção **emailAddresses**.</span><span class="sxs-lookup"><span data-stu-id="bd6ea-125">Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection.</span></span> <span data-ttu-id="bd6ea-126">Ou seja, você não pode filtrar o **nome** ou qualquer outra subpropriedade de uma instância de **emailAddresses**, nem pode aplicar qualquer outro operador ou função com `filter`, como `ne`, `le` e `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="bd6ea-126">That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.</span></span>

<span data-ttu-id="bd6ea-127">Para obter informações gerais sobre o `$filter`parâmetro de consulta, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="bd6ea-127">For general information on the `$filter` query parameter, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd6ea-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd6ea-128">Request headers</span></span>
| <span data-ttu-id="bd6ea-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bd6ea-129">Header</span></span>       | <span data-ttu-id="bd6ea-130">Valor</span><span class="sxs-lookup"><span data-stu-id="bd6ea-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bd6ea-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd6ea-131">Authorization</span></span>  | <span data-ttu-id="bd6ea-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd6ea-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bd6ea-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd6ea-134">Request body</span></span>
<span data-ttu-id="bd6ea-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bd6ea-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd6ea-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd6ea-136">Response</span></span>

<span data-ttu-id="bd6ea-137">Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de objetos [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd6ea-137">If successful, this method returns a `200 OK` response code and collection of [contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bd6ea-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bd6ea-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bd6ea-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd6ea-139">Request</span></span>
<span data-ttu-id="bd6ea-140">O exemplo a seguir obtém as propriedades **DisplayName** e **EmailAddresses** dos contatos do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="bd6ea-140">The following example gets the **displayName** and **emailAddresses** properties of the signed-in user's contacts.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bd6ea-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd6ea-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contacts?$select=displayName,emailAddresses
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bd6ea-142">C#</span><span class="sxs-lookup"><span data-stu-id="bd6ea-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contacts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bd6ea-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="bd6ea-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contacts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bd6ea-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="bd6ea-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contacts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="bd6ea-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd6ea-145">Response</span></span>
<span data-ttu-id="bd6ea-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bd6ea-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('c3e1fcd2-db78-42a8-aec5-1f2cd59abb5c')/contacts(displayName,emailAddresses)",
    "value":[
        {
            "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7f6\"",
            "id":"AAMkADh6v5AAAvgTCFAAA=",
            "displayName":"Elvis Blank",
            "emailAddresses":[
                {
                    "type":"personal",
                    "name":"Elvis Blank",
                    "address":"elvisb@relecloud.onmicrosoft.com"
                },
                {
                    "type":"other",
                    "otherLabel":"Volunteer work",
                    "name":"Elvis Blank",
                    "address":"elvisb@fabrikam.onmicrosoft.com"
                }
            ]
        },
        {
            "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fn\"",
            "id":"AAMkADh6v5AAAvgTCEAAA=",
            "displayName":"Pavel Bansky",
            "emailAddresses":[
                {
                    "type":"personal",
                    "name":"Pavel Bansky",
                    "address":"pavelb@contoso.onmicrosoft.com"
                },
                {
                    "type":"other",
                    "otherLabel":"Volunteer work",
                    "name":"Pavel Bansky",
                    "address":"pavelb@fabrikam.onmicrosoft.com"
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
