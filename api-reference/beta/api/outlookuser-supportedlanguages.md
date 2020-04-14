---
title: 'outlookUser: supportedLanguages'
description: Obtenha a lista de locais e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 47aceb842309ce7bed1c987262f5cda7ad398c67
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440665"
---
# <a name="outlookuser-supportedlanguages"></a><span data-ttu-id="85d34-103">outlookUser: supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="85d34-103">outlookUser: supportedLanguages</span></span>

<span data-ttu-id="85d34-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85d34-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85d34-105">Obtenha a lista de locais e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="85d34-105">Get the list of locales and languages that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="85d34-106">Ao configurar um cliente do Outlook, o usuário seleciona o idioma de preferência na lista compatível.</span><span class="sxs-lookup"><span data-stu-id="85d34-106">When setting up an Outlook client, the user selects the preferred language from this supported list.</span></span> <span data-ttu-id="85d34-107">Posteriormente, é possível obter o idioma de sua preferência [acessando as configurações da caixa de correio do usuário](user-get-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="85d34-107">You can subsequently get the preferred language by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="85d34-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="85d34-108">Permissions</span></span>
<span data-ttu-id="85d34-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85d34-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85d34-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85d34-111">Permission type</span></span>      | <span data-ttu-id="85d34-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="85d34-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85d34-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85d34-113">Delegated (work or school account)</span></span> | <span data-ttu-id="85d34-114">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="85d34-114">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="85d34-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85d34-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85d34-116">User.Read</span><span class="sxs-lookup"><span data-stu-id="85d34-116">User.Read</span></span>    |
|<span data-ttu-id="85d34-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85d34-117">Application</span></span> | <span data-ttu-id="85d34-118">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="85d34-118">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="85d34-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85d34-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedLanguages
GET /users/{id|userPrincipalName}/outlook/supportedLanguages
```
## <a name="request-headers"></a><span data-ttu-id="85d34-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85d34-120">Request headers</span></span>
| <span data-ttu-id="85d34-121">Nome</span><span class="sxs-lookup"><span data-stu-id="85d34-121">Name</span></span>       | <span data-ttu-id="85d34-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="85d34-122">Type</span></span> | <span data-ttu-id="85d34-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="85d34-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="85d34-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="85d34-124">Authorization</span></span>  | <span data-ttu-id="85d34-125">string</span><span class="sxs-lookup"><span data-stu-id="85d34-125">string</span></span>  | <span data-ttu-id="85d34-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85d34-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="85d34-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85d34-128">Request body</span></span>
<span data-ttu-id="85d34-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="85d34-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85d34-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="85d34-130">Response</span></span>
<span data-ttu-id="85d34-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [localeInfo](../resources/localeinfo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85d34-131">If successful, this method returns `200 OK` response code and a collection of [localeInfo](../resources/localeinfo.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85d34-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85d34-132">Example</span></span>
<span data-ttu-id="85d34-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="85d34-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="85d34-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85d34-134">Request</span></span>
<span data-ttu-id="85d34-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="85d34-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="85d34-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="85d34-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_supportedlanguages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/supportedLanguages
```
# <a name="c"></a>[<span data-ttu-id="85d34-137">C#</span><span class="sxs-lookup"><span data-stu-id="85d34-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-supportedlanguages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85d34-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85d34-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-supportedlanguages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85d34-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85d34-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-supportedlanguages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="85d34-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="85d34-140">Response</span></span>
<span data-ttu-id="85d34-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85d34-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.localeInfo",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.localeInfo)",
  "value":[
    {
      "locale":"af-ZA",
      "displayName":"Afrikaans (Suid-Afrika)"
    },
    {
      "locale":"en-US",
      "displayName":"English (United States)"
    },
    {
       "locale":"en-CA",
       "displayName":"English (Canada)"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: supportedLanguages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
