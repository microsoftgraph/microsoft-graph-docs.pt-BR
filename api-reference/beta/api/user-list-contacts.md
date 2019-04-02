---
title: Listar contatos
description: Obter contatos na caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a1eaeac682f511bf9b895e06e6a19b3bc728a38c
ms.sourcegitcommit: e6168b868660ad0078d460424d4e6f987d2684a8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2019
ms.locfileid: "31026007"
---
# <a name="list-contacts"></a><span data-ttu-id="c47fd-103">Listar contatos</span><span class="sxs-lookup"><span data-stu-id="c47fd-103">List contacts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c47fd-104">Obter contatos na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="c47fd-104">Get contacts in the user's mailbox.</span></span>

<span data-ttu-id="c47fd-105">Há dois cenários em que um aplicativo pode obter contatos na pasta de contatos de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="c47fd-105">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="c47fd-106">Se o aplicativo tem permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="c47fd-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="c47fd-107">Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário, e outro usuário tiver compartilhado uma pasta de contatos com esse usuário, ou, o terá acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="c47fd-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="c47fd-108">Confira os [detalhes e um exemplo](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="c47fd-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="c47fd-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="c47fd-109">Permissions</span></span>
<span data-ttu-id="c47fd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c47fd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c47fd-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c47fd-112">Permission type</span></span>      | <span data-ttu-id="c47fd-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c47fd-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c47fd-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c47fd-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c47fd-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c47fd-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c47fd-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c47fd-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c47fd-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c47fd-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c47fd-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c47fd-118">Application</span></span> | <span data-ttu-id="c47fd-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c47fd-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c47fd-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c47fd-120">HTTP request</span></span>

<span data-ttu-id="c47fd-121">Para obter todos os contatos na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="c47fd-121">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="c47fd-122">Para obter os contatos em uma pasta específica na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="c47fd-122">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c47fd-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c47fd-123">Optional query parameters</span></span>
<span data-ttu-id="c47fd-124">Você pode usar o `$filter` parâmetro de consulta para filtrar os contatos com base em seus endereços de email:</span><span class="sxs-lookup"><span data-stu-id="c47fd-124">You can use the `$filter` query parameter to filter contacts based on their email addresses:</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

<span data-ttu-id="c47fd-125">Observe que você pode usar `$filter`, `any`e o `eq` operador somente na subpropriedade **Address** de instâncias em uma coleção EmailAddresses \*\*\*\* .</span><span class="sxs-lookup"><span data-stu-id="c47fd-125">Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection.</span></span> <span data-ttu-id="c47fd-126">Ou seja, você não pode filtrar o **nome** ou qualquer outra subpropriedade de uma instância de **EmailAddresses**, nem pode aplicar qualquer outro operador ou função com `filter`, como `ne`, `le`e. `startswith()`</span><span class="sxs-lookup"><span data-stu-id="c47fd-126">That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.</span></span>

<span data-ttu-id="c47fd-127">Para obter informações gerais sobre `$filter` o parâmetro de consulta, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c47fd-127">For general information on the `$filter` query parameter, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c47fd-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c47fd-128">Request headers</span></span>
| <span data-ttu-id="c47fd-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c47fd-129">Header</span></span>       | <span data-ttu-id="c47fd-130">Valor</span><span class="sxs-lookup"><span data-stu-id="c47fd-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c47fd-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="c47fd-131">Authorization</span></span>  | <span data-ttu-id="c47fd-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c47fd-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c47fd-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c47fd-134">Request body</span></span>
<span data-ttu-id="c47fd-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c47fd-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c47fd-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c47fd-136">Response</span></span>

<span data-ttu-id="c47fd-137">Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de objetos [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c47fd-137">If successful, this method returns a `200 OK` response code and collection of [contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c47fd-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c47fd-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c47fd-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c47fd-139">Request</span></span>
<span data-ttu-id="c47fd-140">O exemplo a seguir obtém as propriedades **DisplayName** e **EmailAddresses** dos contatos do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="c47fd-140">The following example gets the **displayName** and **emailAddresses** properties of the signed-in user's contacts.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contacts?$select=displayName,emailAddresses
```


##### <a name="response"></a><span data-ttu-id="c47fd-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c47fd-141">Response</span></span>
<span data-ttu-id="c47fd-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c47fd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/user-list-contacts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
