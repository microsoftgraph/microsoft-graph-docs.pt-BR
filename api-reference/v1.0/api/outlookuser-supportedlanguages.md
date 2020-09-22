---
title: 'outlookUser: supportedLanguages'
description: Obtenha a lista de locais e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6f79c9df2ffeba511f812580e4596fb54e755b86
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087111"
---
# <a name="outlookuser-supportedlanguages"></a><span data-ttu-id="f3bbf-103">outlookUser: supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="f3bbf-103">outlookUser: supportedLanguages</span></span>

<span data-ttu-id="f3bbf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3bbf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f3bbf-105">Obtenha a lista de locais e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="f3bbf-105">Get the list of locales and languages that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="f3bbf-106">Ao configurar um cliente do Outlook, o usuário seleciona o idioma de preferência na lista compatível.</span><span class="sxs-lookup"><span data-stu-id="f3bbf-106">When setting up an Outlook client, the user selects the preferred language from this supported list.</span></span> <span data-ttu-id="f3bbf-107">Posteriormente, é possível obter o idioma de sua preferência [acessando as configurações da caixa de correio do usuário](user-get-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="f3bbf-107">You can subsequently get the preferred language by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="f3bbf-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f3bbf-108">Permissions</span></span>
<span data-ttu-id="f3bbf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3bbf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3bbf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3bbf-111">Permission type</span></span>      | <span data-ttu-id="f3bbf-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f3bbf-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3bbf-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3bbf-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f3bbf-114">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="f3bbf-114">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="f3bbf-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3bbf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3bbf-116">User.Read</span><span class="sxs-lookup"><span data-stu-id="f3bbf-116">User.Read</span></span>    |
|<span data-ttu-id="f3bbf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3bbf-117">Application</span></span> | <span data-ttu-id="f3bbf-118">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="f3bbf-118">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3bbf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3bbf-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedLanguages
GET /users/{id|userPrincipalName}/outlook/supportedLanguages
```
## <a name="request-headers"></a><span data-ttu-id="f3bbf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3bbf-120">Request headers</span></span>
| <span data-ttu-id="f3bbf-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f3bbf-121">Name</span></span>       | <span data-ttu-id="f3bbf-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3bbf-122">Type</span></span> | <span data-ttu-id="f3bbf-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3bbf-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f3bbf-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3bbf-124">Authorization</span></span>  | <span data-ttu-id="f3bbf-125">string</span><span class="sxs-lookup"><span data-stu-id="f3bbf-125">string</span></span>  | <span data-ttu-id="f3bbf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3bbf-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="f3bbf-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3bbf-128">Request body</span></span>
<span data-ttu-id="f3bbf-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f3bbf-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3bbf-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3bbf-130">Response</span></span>
<span data-ttu-id="f3bbf-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [localeInfo](../resources/localeinfo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3bbf-131">If successful, this method returns `200 OK` response code and a collection of [localeInfo](../resources/localeinfo.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3bbf-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3bbf-132">Example</span></span>
<span data-ttu-id="f3bbf-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f3bbf-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f3bbf-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3bbf-134">Request</span></span>
<span data-ttu-id="f3bbf-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3bbf-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f3bbf-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f3bbf-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_supportedlanguages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/outlook/supportedLanguages
```
# <a name="c"></a>[<span data-ttu-id="f3bbf-137">C#</span><span class="sxs-lookup"><span data-stu-id="f3bbf-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-supportedlanguages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f3bbf-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f3bbf-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-supportedlanguages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f3bbf-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f3bbf-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-supportedlanguages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f3bbf-140">Java</span><span class="sxs-lookup"><span data-stu-id="f3bbf-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-supportedlanguages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f3bbf-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3bbf-141">Response</span></span>
<span data-ttu-id="f3bbf-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3bbf-142">Here is an example of the response.</span></span> 
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.localeInfo)",
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
<!-- {
  "type": "#page.annotation",
  "description": "user: supportedLanguages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

