---
title: 'outlookUser: supportedLanguages'
description: Obtenha a lista de locais e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.
ms.openlocfilehash: ac1b9693121f3ba3f180b53532bb6a6c917e2108
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033369"
---
# <a name="outlookuser-supportedlanguages"></a><span data-ttu-id="31539-103">outlookUser: supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="31539-103">outlookUser: supportedLanguages</span></span>

> <span data-ttu-id="31539-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="31539-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31539-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="31539-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="31539-106">Obtenha a lista de locais e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="31539-106">Get the list of locales and languages that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="31539-107">Ao configurar um cliente do Outlook, o usuário seleciona o idioma de preferência na lista compatível.</span><span class="sxs-lookup"><span data-stu-id="31539-107">When setting up an Outlook client, the user selects the preferred language from this supported list.</span></span> <span data-ttu-id="31539-108">Posteriormente, é possível obter o idioma de sua preferência [acessando as configurações da caixa de correio do usuário](user-get-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="31539-108">You can subsequently get the preferred language by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="31539-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="31539-109">Permissions</span></span>
<span data-ttu-id="31539-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31539-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31539-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31539-112">Permission type</span></span>      | <span data-ttu-id="31539-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31539-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31539-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31539-114">Delegated (work or school account)</span></span> | <span data-ttu-id="31539-115">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="31539-115">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="31539-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31539-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31539-117">User.Read</span><span class="sxs-lookup"><span data-stu-id="31539-117">User.Read</span></span>    |
|<span data-ttu-id="31539-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31539-118">Application</span></span> | <span data-ttu-id="31539-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="31539-119">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="31539-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31539-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedLanguages
GET /users/{id|userPrincipalName}/outlook/supportedLanguages
```
## <a name="request-headers"></a><span data-ttu-id="31539-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31539-121">Request headers</span></span>
| <span data-ttu-id="31539-122">Nome</span><span class="sxs-lookup"><span data-stu-id="31539-122">Name</span></span>       | <span data-ttu-id="31539-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="31539-123">Type</span></span> | <span data-ttu-id="31539-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="31539-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="31539-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="31539-125">Authorization</span></span>  | <span data-ttu-id="31539-126">string</span><span class="sxs-lookup"><span data-stu-id="31539-126">string</span></span>  | <span data-ttu-id="31539-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31539-p104">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="31539-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31539-129">Request body</span></span>
<span data-ttu-id="31539-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="31539-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31539-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="31539-131">Response</span></span>
<span data-ttu-id="31539-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [localeInfo](../resources/localeinfo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31539-132">If successful, this method returns `200 OK` response code and a collection of [localeInfo](../resources/localeinfo.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31539-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31539-133">Example</span></span>
<span data-ttu-id="31539-134">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="31539-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="31539-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31539-135">Request</span></span>
<span data-ttu-id="31539-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="31539-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_supportedlanguages"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/supportedLanguages
```

##### <a name="response"></a><span data-ttu-id="31539-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="31539-137">Response</span></span>
<span data-ttu-id="31539-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31539-138">Here is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "user: supportedLanguages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->