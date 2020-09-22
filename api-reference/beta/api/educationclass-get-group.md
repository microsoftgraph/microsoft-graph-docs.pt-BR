---
title: Obter grupo
description: Recupere o **grupo** Microsoft 365 que corresponde a esse **educationClass**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: dd2dcadf0272a14222d42aaadce30c89df92ac83
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007681"
---
# <a name="get-group"></a><span data-ttu-id="4d4ad-103">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="4d4ad-103">Get group</span></span>

<span data-ttu-id="4d4ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d4ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d4ad-105">Recupere o **grupo** Microsoft 365 que corresponde a esse **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="4d4ad-105">Retrieve the Microsoft 365 **group** that corresponds to this **educationClass**.</span></span>

><span data-ttu-id="4d4ad-106">**Observação:** se o token delegado for usado, os membros só poderão ver informações sobre as próprias escolas.</span><span class="sxs-lookup"><span data-stu-id="4d4ad-106">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="4d4ad-107">Nesse caso, use o recurso `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="4d4ad-107">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d4ad-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="4d4ad-108">Permissions</span></span>
<span data-ttu-id="4d4ad-109">Uma combinação de permissões é obrigatória para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="4d4ad-109">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="4d4ad-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d4ad-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d4ad-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d4ad-111">Permission type</span></span>      | <span data-ttu-id="4d4ad-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d4ad-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d4ad-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d4ad-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="4d4ad-114">Uma de EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write além de Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d4ad-114">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="4d4ad-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d4ad-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4d4ad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d4ad-116">Not supported.</span></span>  |
|<span data-ttu-id="4d4ad-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d4ad-117">Application</span></span> | <span data-ttu-id="4d4ad-118">EduRoster.Read.All, EduRoster.ReadWrite.All além de Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d4ad-118">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="4d4ad-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d4ad-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/group
```
## <a name="request-headers"></a><span data-ttu-id="4d4ad-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d4ad-120">Request headers</span></span>
| <span data-ttu-id="4d4ad-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4d4ad-121">Header</span></span>       | <span data-ttu-id="4d4ad-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4d4ad-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4d4ad-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d4ad-123">Authorization</span></span>  | <span data-ttu-id="4d4ad-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d4ad-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4d4ad-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d4ad-126">Request body</span></span>
<span data-ttu-id="4d4ad-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4d4ad-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4d4ad-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d4ad-128">Response</span></span>
<span data-ttu-id="4d4ad-129">Se bem-sucedido, esse método retorna um código de resposta `200 OK` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d4ad-129">If successful, this method returns a `200 OK` response code and a [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4d4ad-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d4ad-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4d4ad-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d4ad-131">Request</span></span>
<span data-ttu-id="4d4ad-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d4ad-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4d4ad-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d4ad-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationclass_get_group"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/2961761D-8094-4183-A9F6-8E36E966C7D9/group
```
# <a name="c"></a>[<span data-ttu-id="4d4ad-134">C#</span><span class="sxs-lookup"><span data-stu-id="4d4ad-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationclass-get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4d4ad-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d4ad-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationclass-get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4d4ad-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4d4ad-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationclass-get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4d4ad-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d4ad-137">Response</span></span>
<span data-ttu-id="4d4ad-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4d4ad-138">The following is an example of the response.</span></span> 

><span data-ttu-id="4d4ad-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d4ad-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


