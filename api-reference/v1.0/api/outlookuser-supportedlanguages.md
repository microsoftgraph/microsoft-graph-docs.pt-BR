---
title: 'outlookUser: supportedLanguages'
description: Obtenha a lista de locais e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7b1f953e9db89eb95f0873137814681df3e68f3d
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36730068"
---
# <a name="outlookuser-supportedlanguages"></a><span data-ttu-id="6ea2c-103">outlookUser: supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="6ea2c-103">outlookUser: supportedLanguages</span></span>

<span data-ttu-id="6ea2c-104">Obtenha a lista de locais e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="6ea2c-104">Get the list of locales and languages that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="6ea2c-105">Ao configurar um cliente do Outlook, o usuário seleciona o idioma de preferência na lista compatível.</span><span class="sxs-lookup"><span data-stu-id="6ea2c-105">When setting up an Outlook client, the user selects the preferred language from this supported list.</span></span> <span data-ttu-id="6ea2c-106">Posteriormente, é possível obter o idioma de sua preferência [acessando as configurações da caixa de correio do usuário](user-get-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="6ea2c-106">You can subsequently get the preferred language by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="6ea2c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6ea2c-107">Permissions</span></span>
<span data-ttu-id="6ea2c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ea2c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ea2c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ea2c-110">Permission type</span></span>      | <span data-ttu-id="6ea2c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6ea2c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ea2c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ea2c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6ea2c-113">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="6ea2c-113">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="6ea2c-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ea2c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ea2c-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="6ea2c-115">User.Read</span></span>    |
|<span data-ttu-id="6ea2c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ea2c-116">Application</span></span> | <span data-ttu-id="6ea2c-117">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ea2c-117">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ea2c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ea2c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedLanguages
GET /users/{id|userPrincipalName}/outlook/supportedLanguages
```
## <a name="request-headers"></a><span data-ttu-id="6ea2c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ea2c-119">Request headers</span></span>
| <span data-ttu-id="6ea2c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6ea2c-120">Name</span></span>       | <span data-ttu-id="6ea2c-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ea2c-121">Type</span></span> | <span data-ttu-id="6ea2c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ea2c-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6ea2c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ea2c-123">Authorization</span></span>  | <span data-ttu-id="6ea2c-124">string</span><span class="sxs-lookup"><span data-stu-id="6ea2c-124">string</span></span>  | <span data-ttu-id="6ea2c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ea2c-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="6ea2c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ea2c-127">Request body</span></span>
<span data-ttu-id="6ea2c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6ea2c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ea2c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ea2c-129">Response</span></span>
<span data-ttu-id="6ea2c-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [localeInfo](../resources/localeinfo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ea2c-130">If successful, this method returns `200 OK` response code and a collection of [localeInfo](../resources/localeinfo.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ea2c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ea2c-131">Example</span></span>
<span data-ttu-id="6ea2c-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="6ea2c-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6ea2c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ea2c-133">Request</span></span>
<span data-ttu-id="6ea2c-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ea2c-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6ea2c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ea2c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_supportedlanguages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/outlook/supportedLanguages
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6ea2c-136">C#</span><span class="sxs-lookup"><span data-stu-id="6ea2c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-supportedlanguages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6ea2c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ea2c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-supportedlanguages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6ea2c-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6ea2c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-supportedlanguages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6ea2c-139">Java</span><span class="sxs-lookup"><span data-stu-id="6ea2c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-supportedlanguages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6ea2c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ea2c-140">Response</span></span>
<span data-ttu-id="6ea2c-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ea2c-141">Here is an example of the response.</span></span> 
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
