---
title: Obter mobileAppManagementPolicy
description: Leia as propriedades e as relações de uma política de gerenciamento de aplicativo móvel.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 062382f52f4efbd709a68f122a38a0ce0d4b5718
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547318"
---
# <a name="get-mobileappmanagementpolicy"></a><span data-ttu-id="3823e-103">Obter mobileAppManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="3823e-103">Get mobileAppManagementPolicy</span></span>

<span data-ttu-id="3823e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3823e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3823e-105">Leia as propriedades e as relações de um [objeto mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3823e-105">Read the properties and relationships of a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3823e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3823e-106">Permissions</span></span>

<span data-ttu-id="3823e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3823e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3823e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3823e-109">Permission type</span></span>|<span data-ttu-id="3823e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3823e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3823e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3823e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3823e-112">Policy.Read.All, Policy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3823e-112">Policy.Read.All, Policy.ReadWrite.All</span></span>|
|<span data-ttu-id="3823e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3823e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3823e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3823e-114">Not supported.</span></span>|
|<span data-ttu-id="3823e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3823e-115">Application</span></span> | <span data-ttu-id="3823e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3823e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3823e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3823e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/mobileAppManagementPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3823e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3823e-118">Request headers</span></span>

|<span data-ttu-id="3823e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3823e-119">Name</span></span>|<span data-ttu-id="3823e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3823e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3823e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3823e-121">Authorization</span></span>|<span data-ttu-id="3823e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3823e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3823e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3823e-124">Request body</span></span>

<span data-ttu-id="3823e-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3823e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3823e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="3823e-126">Response</span></span>

<span data-ttu-id="3823e-127">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3823e-127">If successful, this method returns a `200 OK` response code and a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3823e-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3823e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3823e-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3823e-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_mobilitymanagementpolicy"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020
```

### <a name="response"></a><span data-ttu-id="3823e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3823e-130">Response</span></span>

><span data-ttu-id="3823e-131">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3823e-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mobilityManagementPolicy"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "ab90bacf-55a3-4a3e-839a-aa4b74e4f020",
    "appliesTo": "selected",
    "complianceUrl": "https://portal.mam.contoso.com/?portalAction=Compliance",
    "description": "Contoso mobilty app is a cloud-based  Endpoint Management solution for managing Windows.",
    "discoveryUrl": "https://enrollment.mam.contoso.com/enrollmentserver/discovery.svc",
    "displayName": "Contoso mobilty app",
    "termsOfUseUrl": "https://portal.mam.contoso.com/TermsofUse.aspx",
    "includedGroups": [
      {
        "id": "800c583d-cc3d-4361-8e4a-3fbf668f27f4",
        "displayName": "Test Group"
      }
    ]
  }
}
```
