---
title: Obter mobileDeviceManagementPolicy
description: Leia as propriedades e as relações de um objeto de política de gerenciamento de dispositivo móvel.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 3e09179fa6ebbbbe2c168b575883192ee9ba4f93
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547304"
---
# <a name="get-mobiledevicemanagementpolicy"></a><span data-ttu-id="659d2-103">Obter mobileDeviceManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="659d2-103">Get mobileDeviceManagementPolicy</span></span>

<span data-ttu-id="659d2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="659d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="659d2-105">Leia as propriedades e as relações de um [objeto mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="659d2-105">Read the properties and relationships of a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="659d2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="659d2-106">Permissions</span></span>

<span data-ttu-id="659d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="659d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="659d2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="659d2-109">Permission type</span></span>|<span data-ttu-id="659d2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="659d2-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="659d2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="659d2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="659d2-112">Policy.Read.All, Policy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="659d2-112">Policy.Read.All, Policy.ReadWrite.All</span></span>|
|<span data-ttu-id="659d2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="659d2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="659d2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="659d2-114">Not supported.</span></span>|
|<span data-ttu-id="659d2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="659d2-115">Application</span></span> | <span data-ttu-id="659d2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="659d2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="659d2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="659d2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/mobileDeviceManagementPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="659d2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="659d2-118">Request headers</span></span>

|<span data-ttu-id="659d2-119">Nome</span><span class="sxs-lookup"><span data-stu-id="659d2-119">Name</span></span>|<span data-ttu-id="659d2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="659d2-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="659d2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="659d2-121">Authorization</span></span>|<span data-ttu-id="659d2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="659d2-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="659d2-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="659d2-124">Request body</span></span>

<span data-ttu-id="659d2-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="659d2-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="659d2-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="659d2-126">Response</span></span>

<span data-ttu-id="659d2-127">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="659d2-127">If successful, this method returns a `200 OK` response code and a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="659d2-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="659d2-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="659d2-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="659d2-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_mobilitymanagementpolicy"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020
```

### <a name="response"></a><span data-ttu-id="659d2-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="659d2-130">Response</span></span>

><span data-ttu-id="659d2-131">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="659d2-131">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "complianceUrl": "https://portal.mdm.contoso.com/?portalAction=Compliance",
    "description": "Contoso mobilty app is a cloud-based  Endpoint Management solution for managing Windows.",
    "discoveryUrl": "https://enrollment.mdm.contoso.com/enrollmentserver/discovery.svc",
    "displayName": "Contoso mobilty app",
    "termsOfUseUrl": "https://portal.mdm.contoso.com/TermsofUse.aspx",
    "includedGroups": [
      {
        "id": "dc3d2ce5-7c5e-4dca-a0ef-2145bf6e53ef",
        "displayName": "Test MDM Group"
      }
    ]
  }
}
```
