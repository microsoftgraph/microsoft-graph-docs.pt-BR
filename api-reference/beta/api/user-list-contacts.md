---
title: Listar contatos
description: Obtenha os contatos na caixa de correio do usuário.
localization_priority: Normal
ms.openlocfilehash: b78009d44fd442bab31b9911056023256a1d5102
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886615"
---
# <a name="list-contacts"></a><span data-ttu-id="da4a6-103">Listar contatos</span><span class="sxs-lookup"><span data-stu-id="da4a6-103">List contacts</span></span>

> <span data-ttu-id="da4a6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="da4a6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da4a6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="da4a6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="da4a6-106">Obtenha os contatos na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="da4a6-106">Get contacts in the user's mailbox.</span></span>

<span data-ttu-id="da4a6-107">Há dois cenários onde um aplicativo pode obter contatos na pasta de contatos de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="da4a6-107">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="da4a6-108">Se o aplicativo tem permissões de aplicativo, ou,</span><span class="sxs-lookup"><span data-stu-id="da4a6-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="da4a6-109">Se o aplicativo tiver apropriada [permissões](#permissions) delegadas de um usuário, e outro usuário compartilhou uma pasta de contato com que o usuário ou, tem acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="da4a6-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="da4a6-110">Consulte os [detalhes e um exemplo](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="da4a6-110">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="da4a6-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="da4a6-111">Permissions</span></span>
<span data-ttu-id="da4a6-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da4a6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da4a6-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da4a6-114">Permission type</span></span>      | <span data-ttu-id="da4a6-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da4a6-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da4a6-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da4a6-116">Delegated (work or school account)</span></span> | <span data-ttu-id="da4a6-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da4a6-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="da4a6-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da4a6-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da4a6-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da4a6-119">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="da4a6-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da4a6-120">Application</span></span> | <span data-ttu-id="da4a6-121">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da4a6-121">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="da4a6-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da4a6-122">HTTP request</span></span>

<span data-ttu-id="da4a6-123">Para obter todos os contatos na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="da4a6-123">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="da4a6-124">Para obter os contatos em uma pasta específica na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="da4a6-124">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="da4a6-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="da4a6-125">Optional query parameters</span></span>
<span data-ttu-id="da4a6-126">Você pode usar o `$filter` parâmetro de consulta para contatos de filtro com base em seus endereços de email:</span><span class="sxs-lookup"><span data-stu-id="da4a6-126">You can use the `$filter` query parameter to filter contacts based on their email addresses:</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

<span data-ttu-id="da4a6-127">Observe que você pode usar `$filter`, `any`e o `eq` operador somente à propriedade sub-recursos do **endereço** do instâncias em um conjunto de **emailAddresses** .</span><span class="sxs-lookup"><span data-stu-id="da4a6-127">Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection.</span></span> <span data-ttu-id="da4a6-128">Ou seja, é possível filtrar o **nome** ou qualquer outra propriedade sub-recurso de uma instância de **emailAddresses**, nem você pode aplicar o operador any ou funcionar com `filter`, tais como `ne`, `le`, e `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="da4a6-128">That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.</span></span>

<span data-ttu-id="da4a6-129">Para obter informações gerais sobre o `$filter` consulta parâmetro, consulte [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="da4a6-129">For general information on the `$filter` query parameter, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="da4a6-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da4a6-130">Request headers</span></span>
| <span data-ttu-id="da4a6-131">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="da4a6-131">Header</span></span>       | <span data-ttu-id="da4a6-132">Valor</span><span class="sxs-lookup"><span data-stu-id="da4a6-132">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="da4a6-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="da4a6-133">Authorization</span></span>  | <span data-ttu-id="da4a6-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da4a6-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="da4a6-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da4a6-136">Request body</span></span>
<span data-ttu-id="da4a6-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da4a6-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da4a6-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="da4a6-138">Response</span></span>

<span data-ttu-id="da4a6-139">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos de [contato](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da4a6-139">If successful, this method returns a `200 OK` response code and collection of [contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="da4a6-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da4a6-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da4a6-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da4a6-141">Request</span></span>
<span data-ttu-id="da4a6-142">O exemplo a seguir obtém as propriedades **displayName** e **emailAddresses** de contatos do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="da4a6-142">The following example gets the **displayName** and **emailAddresses** properties of the signed-in user's contacts.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contacts?$select=displayName,emailAddresses
```


##### <a name="response"></a><span data-ttu-id="da4a6-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="da4a6-143">Response</span></span>
<span data-ttu-id="da4a6-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da4a6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
