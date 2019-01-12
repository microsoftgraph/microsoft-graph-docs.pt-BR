---
title: Obter grupo
description: Recupere o **group** do Office 365 que corresponde a essa **educationClass**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: d467e36afe09ee37b51afcf25ed8f1917ed6ab16
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931696"
---
# <a name="get-group"></a><span data-ttu-id="16946-103">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="16946-103">Get group</span></span>

<span data-ttu-id="16946-104">Recupere o **group** do Office 365 que corresponde a essa **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="16946-104">Retrieve the Office 365 **group** that corresponds to this **educationClass**.</span></span>

><span data-ttu-id="16946-105">**Observação:** se o token delegado for usado, os membros só poderão ver informações sobre as próprias escolas.</span><span class="sxs-lookup"><span data-stu-id="16946-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="16946-106">Nesse caso, use o recurso `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="16946-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="16946-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="16946-107">Permissions</span></span>
<span data-ttu-id="16946-108">Uma combinação de permissões é obrigatória para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="16946-108">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="16946-109">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16946-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16946-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16946-110">Permission type</span></span>      | <span data-ttu-id="16946-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="16946-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16946-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16946-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="16946-113">Uma de EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write além de Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="16946-113">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="16946-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16946-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="16946-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16946-115">Not supported.</span></span>  |
|<span data-ttu-id="16946-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16946-116">Application</span></span> | <span data-ttu-id="16946-117">EduRoster.Read.All, EduRoster.ReadWrite.All além de Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="16946-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="16946-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16946-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/group
```
## <a name="request-headers"></a><span data-ttu-id="16946-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16946-119">Request headers</span></span>
| <span data-ttu-id="16946-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="16946-120">Header</span></span>       | <span data-ttu-id="16946-121">Valor</span><span class="sxs-lookup"><span data-stu-id="16946-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="16946-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="16946-122">Authorization</span></span>  | <span data-ttu-id="16946-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16946-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="16946-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16946-125">Request body</span></span>
<span data-ttu-id="16946-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="16946-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="16946-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="16946-127">Response</span></span>
<span data-ttu-id="16946-128">Se bem-sucedido, esse método retorna um código de resposta `200 OK` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16946-128">If successful, this method returns a `200 OK` response code and a [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="16946-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16946-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="16946-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16946-130">Request</span></span>
<span data-ttu-id="16946-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="16946-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/group
```
##### <a name="response"></a><span data-ttu-id="16946-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="16946-132">Response</span></span>
<span data-ttu-id="16946-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="16946-133">The following is an example of the response.</span></span> 

><span data-ttu-id="16946-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16946-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
