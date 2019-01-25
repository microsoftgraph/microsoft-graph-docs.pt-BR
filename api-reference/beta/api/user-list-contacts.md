---
title: Listar contatos
description: Obtenha os contatos na caixa de correio do usuário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8c444a818b933196ddc46ae0d12d64355656bd7f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510908"
---
# <a name="list-contacts"></a><span data-ttu-id="5920a-103">Listar contatos</span><span class="sxs-lookup"><span data-stu-id="5920a-103">List contacts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5920a-104">Obtenha os contatos na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="5920a-104">Get contacts in the user's mailbox.</span></span>

<span data-ttu-id="5920a-105">Há dois cenários onde um aplicativo pode obter contatos na pasta de contatos de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="5920a-105">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="5920a-106">Se o aplicativo tem permissões de aplicativo, ou,</span><span class="sxs-lookup"><span data-stu-id="5920a-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="5920a-107">Se o aplicativo tiver apropriada [permissões](#permissions) delegadas de um usuário, e outro usuário compartilhou uma pasta de contato com que o usuário ou, tem acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="5920a-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="5920a-108">Consulte os [detalhes e um exemplo](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="5920a-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="5920a-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="5920a-109">Permissions</span></span>
<span data-ttu-id="5920a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5920a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5920a-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5920a-112">Permission type</span></span>      | <span data-ttu-id="5920a-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5920a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5920a-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5920a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5920a-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5920a-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="5920a-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5920a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5920a-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5920a-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="5920a-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5920a-118">Application</span></span> | <span data-ttu-id="5920a-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5920a-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5920a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5920a-120">HTTP request</span></span>

<span data-ttu-id="5920a-121">Para obter todos os contatos na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="5920a-121">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="5920a-122">Para obter os contatos em uma pasta específica na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="5920a-122">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5920a-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5920a-123">Optional query parameters</span></span>
<span data-ttu-id="5920a-124">Você pode usar o `$filter` parâmetro de consulta para contatos de filtro com base em seus endereços de email:</span><span class="sxs-lookup"><span data-stu-id="5920a-124">You can use the `$filter` query parameter to filter contacts based on their email addresses:</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

<span data-ttu-id="5920a-125">Observe que você pode usar `$filter`, `any`e o `eq` operador somente à propriedade sub-recursos do **endereço** do instâncias em um conjunto de **emailAddresses** .</span><span class="sxs-lookup"><span data-stu-id="5920a-125">Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection.</span></span> <span data-ttu-id="5920a-126">Ou seja, é possível filtrar o **nome** ou qualquer outra propriedade sub-recurso de uma instância de **emailAddresses**, nem você pode aplicar o operador any ou funcionar com `filter`, tais como `ne`, `le`, e `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="5920a-126">That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.</span></span>

<span data-ttu-id="5920a-127">Para obter informações gerais sobre o `$filter` consulta parâmetro, consulte [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5920a-127">For general information on the `$filter` query parameter, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5920a-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5920a-128">Request headers</span></span>
| <span data-ttu-id="5920a-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5920a-129">Header</span></span>       | <span data-ttu-id="5920a-130">Valor</span><span class="sxs-lookup"><span data-stu-id="5920a-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5920a-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="5920a-131">Authorization</span></span>  | <span data-ttu-id="5920a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5920a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5920a-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5920a-134">Request body</span></span>
<span data-ttu-id="5920a-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5920a-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5920a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5920a-136">Response</span></span>

<span data-ttu-id="5920a-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos de [contato](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5920a-137">If successful, this method returns a `200 OK` response code and collection of [contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5920a-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5920a-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5920a-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5920a-139">Request</span></span>
<span data-ttu-id="5920a-140">O exemplo a seguir obtém as propriedades **displayName** e **emailAddresses** de contatos do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="5920a-140">The following example gets the **displayName** and **emailAddresses** properties of the signed-in user's contacts.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contacts?$select=displayName,emailAddresses
```


##### <a name="response"></a><span data-ttu-id="5920a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="5920a-141">Response</span></span>
<span data-ttu-id="5920a-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5920a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
