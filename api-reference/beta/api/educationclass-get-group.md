---
title: Obter grupo
description: Recupere o **group** do Office 365 que corresponde a essa **educationClass**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c02f2c74bb1338e651125bba411a200757313e73
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42426868"
---
# <a name="get-group"></a><span data-ttu-id="88a9a-103">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="88a9a-103">Get group</span></span>

<span data-ttu-id="88a9a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="88a9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88a9a-105">Recupere o **group** do Office 365 que corresponde a essa **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="88a9a-105">Retrieve the Office 365 **group** that corresponds to this **educationClass**.</span></span>

><span data-ttu-id="88a9a-106">**Observação:** se o token delegado for usado, os membros só poderão ver informações sobre as próprias escolas.</span><span class="sxs-lookup"><span data-stu-id="88a9a-106">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="88a9a-107">Nesse caso, use o recurso `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="88a9a-107">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="88a9a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="88a9a-108">Permissions</span></span>
<span data-ttu-id="88a9a-109">Uma combinação de permissões é obrigatória para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="88a9a-109">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="88a9a-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88a9a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88a9a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88a9a-111">Permission type</span></span>      | <span data-ttu-id="88a9a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="88a9a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88a9a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88a9a-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="88a9a-114">Uma de EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write além de Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="88a9a-114">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="88a9a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88a9a-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="88a9a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88a9a-116">Not supported.</span></span>  |
|<span data-ttu-id="88a9a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88a9a-117">Application</span></span> | <span data-ttu-id="88a9a-118">EduRoster.Read.All, EduRoster.ReadWrite.All além de Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="88a9a-118">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="88a9a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88a9a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/group
```
## <a name="request-headers"></a><span data-ttu-id="88a9a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88a9a-120">Request headers</span></span>
| <span data-ttu-id="88a9a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="88a9a-121">Header</span></span>       | <span data-ttu-id="88a9a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="88a9a-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="88a9a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="88a9a-123">Authorization</span></span>  | <span data-ttu-id="88a9a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88a9a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="88a9a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88a9a-126">Request body</span></span>
<span data-ttu-id="88a9a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="88a9a-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="88a9a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="88a9a-128">Response</span></span>
<span data-ttu-id="88a9a-129">Se bem-sucedido, esse método retorna um código de resposta `200 OK` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88a9a-129">If successful, this method returns a `200 OK` response code and a [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="88a9a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88a9a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88a9a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88a9a-131">Request</span></span>
<span data-ttu-id="88a9a-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="88a9a-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="88a9a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="88a9a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationclass_get_group"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/2961761D-8094-4183-A9F6-8E36E966C7D9/group
```
# <a name="c"></a>[<span data-ttu-id="88a9a-134">C#</span><span class="sxs-lookup"><span data-stu-id="88a9a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationclass-get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88a9a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88a9a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationclass-get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88a9a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88a9a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationclass-get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="88a9a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="88a9a-137">Response</span></span>
<span data-ttu-id="88a9a-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="88a9a-138">The following is an example of the response.</span></span> 

><span data-ttu-id="88a9a-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88a9a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
  "id": "id-value",
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value",
  "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
  "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
  "onPremisesSyncEnabled": true,
  "proxyAddresses": [
    "proxyAddresses-value"
   ],
   "securityEnabled": true,
   "visibility": "visibility-value"
}
```

<!-- uuid: 0087D9B3-1418-4C87-91C9-A18C6D93706B
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
