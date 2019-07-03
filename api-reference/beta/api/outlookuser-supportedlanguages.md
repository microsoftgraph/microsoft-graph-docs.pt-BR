---
title: 'outlookUser: supportedLanguages'
description: Obtenha a lista de locais e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: d4ce8902458688e693293742987a831c7fb8440d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35452512"
---
# <a name="outlookuser-supportedlanguages"></a><span data-ttu-id="f7f86-103">outlookUser: supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="f7f86-103">outlookUser: supportedLanguages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7f86-104">Obtenha a lista de locais e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="f7f86-104">Get the list of locales and languages that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="f7f86-105">Ao configurar um cliente do Outlook, o usuário seleciona o idioma de preferência na lista compatível.</span><span class="sxs-lookup"><span data-stu-id="f7f86-105">When setting up an Outlook client, the user selects the preferred language from this supported list.</span></span> <span data-ttu-id="f7f86-106">Posteriormente, é possível obter o idioma de sua preferência [acessando as configurações da caixa de correio do usuário](user-get-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="f7f86-106">You can subsequently get the preferred language by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="f7f86-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7f86-107">Permissions</span></span>
<span data-ttu-id="f7f86-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7f86-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7f86-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7f86-110">Permission type</span></span>      | <span data-ttu-id="f7f86-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7f86-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7f86-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7f86-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f7f86-113">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="f7f86-113">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="f7f86-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7f86-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7f86-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="f7f86-115">User.Read</span></span>    |
|<span data-ttu-id="f7f86-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7f86-116">Application</span></span> | <span data-ttu-id="f7f86-117">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7f86-117">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7f86-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7f86-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedLanguages
GET /users/{id|userPrincipalName}/outlook/supportedLanguages
```
## <a name="request-headers"></a><span data-ttu-id="f7f86-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7f86-119">Request headers</span></span>
| <span data-ttu-id="f7f86-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f7f86-120">Name</span></span>       | <span data-ttu-id="f7f86-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7f86-121">Type</span></span> | <span data-ttu-id="f7f86-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7f86-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f7f86-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7f86-123">Authorization</span></span>  | <span data-ttu-id="f7f86-124">string</span><span class="sxs-lookup"><span data-stu-id="f7f86-124">string</span></span>  | <span data-ttu-id="f7f86-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7f86-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="f7f86-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7f86-127">Request body</span></span>
<span data-ttu-id="f7f86-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f7f86-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7f86-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7f86-129">Response</span></span>
<span data-ttu-id="f7f86-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [localeInfo](../resources/localeinfo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7f86-130">If successful, this method returns `200 OK` response code and a collection of [localeInfo](../resources/localeinfo.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7f86-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7f86-131">Example</span></span>
<span data-ttu-id="f7f86-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f7f86-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f7f86-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7f86-133">Request</span></span>
<span data-ttu-id="f7f86-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7f86-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f7f86-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7f86-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_supportedlanguages"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/supportedLanguages
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f7f86-136">C#</span><span class="sxs-lookup"><span data-stu-id="f7f86-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-supportedlanguages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f7f86-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="f7f86-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-supportedlanguages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f7f86-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f7f86-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-supportedlanguages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f7f86-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7f86-139">Response</span></span>
<span data-ttu-id="f7f86-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7f86-140">Here is an example of the response.</span></span> 
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
