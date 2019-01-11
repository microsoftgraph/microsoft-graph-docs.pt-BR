---
title: Obter grupo
description: Recupere o **group** do Office 365 que corresponde a essa **educationClass**.
localization_priority: Normal
ms.openlocfilehash: 9f84a1310fbc42d2f5e5a1b7e828dc90a71ab5fc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866266"
---
# <a name="get-group"></a><span data-ttu-id="31464-103">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="31464-103">Get group</span></span>

> <span data-ttu-id="31464-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="31464-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31464-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="31464-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="31464-106">Recupere o **group** do Office 365 que corresponde a essa **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="31464-106">Retrieve the Office 365 **group** that corresponds to this **educationClass**.</span></span>

><span data-ttu-id="31464-107">**Observação:** se o token delegado for usado, os membros só poderão ver informações sobre as próprias escolas.</span><span class="sxs-lookup"><span data-stu-id="31464-107">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="31464-108">Nesse caso, use o recurso `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="31464-108">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="31464-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="31464-109">Permissions</span></span>
<span data-ttu-id="31464-110">Uma combinação de permissões é obrigatória para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="31464-110">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="31464-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31464-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31464-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31464-112">Permission type</span></span>      | <span data-ttu-id="31464-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31464-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31464-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31464-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="31464-115">Uma de EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write além de Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="31464-115">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="31464-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31464-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="31464-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31464-117">Not supported.</span></span>  |
|<span data-ttu-id="31464-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31464-118">Application</span></span> | <span data-ttu-id="31464-119">EduRoster.Read.All, EduRoster.ReadWrite.All além de Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="31464-119">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="31464-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31464-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/group
```
## <a name="request-headers"></a><span data-ttu-id="31464-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31464-121">Request headers</span></span>
| <span data-ttu-id="31464-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="31464-122">Header</span></span>       | <span data-ttu-id="31464-123">Valor</span><span class="sxs-lookup"><span data-stu-id="31464-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="31464-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="31464-124">Authorization</span></span>  | <span data-ttu-id="31464-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31464-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="31464-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31464-127">Request body</span></span>
<span data-ttu-id="31464-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="31464-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="31464-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="31464-129">Response</span></span>
<span data-ttu-id="31464-130">Se bem-sucedido, esse método retorna um código de resposta `200 OK` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31464-130">If successful, this method returns a `200 OK` response code and a [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="31464-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31464-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31464-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31464-132">Request</span></span>
<span data-ttu-id="31464-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="31464-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/2961761D-8094-4183-A9F6-8E36E966C7D9/group
```
##### <a name="response"></a><span data-ttu-id="31464-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="31464-134">Response</span></span>
<span data-ttu-id="31464-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="31464-135">The following is an example of the response.</span></span> 

><span data-ttu-id="31464-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31464-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
