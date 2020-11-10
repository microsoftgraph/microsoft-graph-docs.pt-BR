---
title: Obter grupo
description: Recupere o **grupo** Microsoft 365 que corresponde a esse **educationClass**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5cff82e4b9c93502aacb390925af034159aba101
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966310"
---
# <a name="get-group"></a><span data-ttu-id="fc3ae-103">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="fc3ae-103">Get group</span></span>

<span data-ttu-id="fc3ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc3ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc3ae-105">Recupere o **grupo** Microsoft 365 que corresponde a esse **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="fc3ae-105">Retrieve the Microsoft 365 **group** that corresponds to this **educationClass**.</span></span>

><span data-ttu-id="fc3ae-106">**Observação:** se o token delegado for usado, os membros só poderão ver informações sobre as próprias escolas.</span><span class="sxs-lookup"><span data-stu-id="fc3ae-106">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="fc3ae-107">Nesse caso, use o recurso `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="fc3ae-107">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc3ae-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc3ae-108">Permissions</span></span>
<span data-ttu-id="fc3ae-109">Uma combinação de permissões é obrigatória para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="fc3ae-109">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="fc3ae-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc3ae-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc3ae-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc3ae-111">Permission type</span></span>      | <span data-ttu-id="fc3ae-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc3ae-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc3ae-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc3ae-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="fc3ae-114">Uma de EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write além de Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc3ae-114">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="fc3ae-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc3ae-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fc3ae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc3ae-116">Not supported.</span></span>  |
|<span data-ttu-id="fc3ae-117">Application</span><span class="sxs-lookup"><span data-stu-id="fc3ae-117">Application</span></span> | <span data-ttu-id="fc3ae-118">EduRoster.Read.All, EduRoster.ReadWrite.All além de Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc3ae-118">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="fc3ae-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc3ae-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/group
```
## <a name="request-headers"></a><span data-ttu-id="fc3ae-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc3ae-120">Request headers</span></span>
| <span data-ttu-id="fc3ae-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fc3ae-121">Header</span></span>       | <span data-ttu-id="fc3ae-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fc3ae-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fc3ae-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc3ae-123">Authorization</span></span>  | <span data-ttu-id="fc3ae-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc3ae-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fc3ae-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc3ae-126">Request body</span></span>
<span data-ttu-id="fc3ae-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fc3ae-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="fc3ae-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc3ae-128">Response</span></span>
<span data-ttu-id="fc3ae-129">Se bem-sucedido, esse método retorna um código de resposta `200 OK` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc3ae-129">If successful, this method returns a `200 OK` response code and a [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fc3ae-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc3ae-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc3ae-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc3ae-131">Request</span></span>
<span data-ttu-id="fc3ae-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc3ae-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fc3ae-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc3ae-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationclass_get_group"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/2961761D-8094-4183-A9F6-8E36E966C7D9/group
```
# <a name="c"></a>[<span data-ttu-id="fc3ae-134">C#</span><span class="sxs-lookup"><span data-stu-id="fc3ae-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationclass-get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc3ae-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc3ae-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationclass-get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc3ae-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc3ae-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationclass-get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fc3ae-137">Java</span><span class="sxs-lookup"><span data-stu-id="fc3ae-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationclass-get-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fc3ae-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc3ae-138">Response</span></span>
<span data-ttu-id="fc3ae-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fc3ae-139">The following is an example of the response.</span></span> 

><span data-ttu-id="fc3ae-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc3ae-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


