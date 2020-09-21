---
title: 'outlookUser: supportedLanguages'
description: Obtenha a lista de locais e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4828b37ec738d31806c3fecd6a5da29cefefb667
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47969421"
---
# <a name="outlookuser-supportedlanguages"></a><span data-ttu-id="26072-103">outlookUser: supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="26072-103">outlookUser: supportedLanguages</span></span>

<span data-ttu-id="26072-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26072-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26072-105">Obtenha a lista de locais e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="26072-105">Get the list of locales and languages that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="26072-106">Ao configurar um cliente do Outlook, o usuário seleciona o idioma de preferência na lista compatível.</span><span class="sxs-lookup"><span data-stu-id="26072-106">When setting up an Outlook client, the user selects the preferred language from this supported list.</span></span> <span data-ttu-id="26072-107">Posteriormente, é possível obter o idioma de sua preferência [acessando as configurações da caixa de correio do usuário](user-get-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="26072-107">You can subsequently get the preferred language by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="26072-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="26072-108">Permissions</span></span>
<span data-ttu-id="26072-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26072-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26072-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26072-111">Permission type</span></span>      | <span data-ttu-id="26072-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26072-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26072-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26072-113">Delegated (work or school account)</span></span> | <span data-ttu-id="26072-114">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="26072-114">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="26072-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26072-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26072-116">User.Read</span><span class="sxs-lookup"><span data-stu-id="26072-116">User.Read</span></span>    |
|<span data-ttu-id="26072-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26072-117">Application</span></span> | <span data-ttu-id="26072-118">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="26072-118">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="26072-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26072-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedLanguages
GET /users/{id|userPrincipalName}/outlook/supportedLanguages
```
## <a name="request-headers"></a><span data-ttu-id="26072-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26072-120">Request headers</span></span>
| <span data-ttu-id="26072-121">Nome</span><span class="sxs-lookup"><span data-stu-id="26072-121">Name</span></span>       | <span data-ttu-id="26072-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="26072-122">Type</span></span> | <span data-ttu-id="26072-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="26072-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="26072-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="26072-124">Authorization</span></span>  | <span data-ttu-id="26072-125">string</span><span class="sxs-lookup"><span data-stu-id="26072-125">string</span></span>  | <span data-ttu-id="26072-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26072-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="26072-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26072-128">Request body</span></span>
<span data-ttu-id="26072-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="26072-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26072-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="26072-130">Response</span></span>
<span data-ttu-id="26072-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [localeInfo](../resources/localeinfo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26072-131">If successful, this method returns `200 OK` response code and a collection of [localeInfo](../resources/localeinfo.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26072-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26072-132">Example</span></span>
<span data-ttu-id="26072-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="26072-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="26072-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26072-134">Request</span></span>
<span data-ttu-id="26072-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26072-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="26072-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="26072-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_supportedlanguages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/supportedLanguages
```
# <a name="c"></a>[<span data-ttu-id="26072-137">C#</span><span class="sxs-lookup"><span data-stu-id="26072-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-supportedlanguages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26072-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26072-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-supportedlanguages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26072-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26072-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-supportedlanguages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="26072-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="26072-140">Response</span></span>
<span data-ttu-id="26072-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26072-141">Here is an example of the response.</span></span> 
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


