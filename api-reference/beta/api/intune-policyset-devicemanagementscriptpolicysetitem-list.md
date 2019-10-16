---
title: Listar deviceManagementScriptPolicySetItems
description: Listar Propriedades e relações dos objetos deviceManagementScriptPolicySetItem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bca88b5aa40af2e970719160d1509c8af61c4d4d
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537584"
---
# <a name="list-devicemanagementscriptpolicysetitems"></a><span data-ttu-id="b3ebe-103">Listar deviceManagementScriptPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="b3ebe-103">List deviceManagementScriptPolicySetItems</span></span>

> <span data-ttu-id="b3ebe-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b3ebe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3ebe-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b3ebe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3ebe-106">Listar Propriedades e relações dos objetos [deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="b3ebe-106">List properties and relationships of the [deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3ebe-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b3ebe-107">Prerequisites</span></span>
<span data-ttu-id="b3ebe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3ebe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3ebe-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3ebe-110">Permission type</span></span>|<span data-ttu-id="b3ebe-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b3ebe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3ebe-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3ebe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b3ebe-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3ebe-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b3ebe-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3ebe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3ebe-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3ebe-115">Not supported.</span></span>|
|<span data-ttu-id="b3ebe-116">Application</span><span class="sxs-lookup"><span data-stu-id="b3ebe-116">Application</span></span>|<span data-ttu-id="b3ebe-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3ebe-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3ebe-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3ebe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="b3ebe-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3ebe-119">Request headers</span></span>
|<span data-ttu-id="b3ebe-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b3ebe-120">Header</span></span>|<span data-ttu-id="b3ebe-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b3ebe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3ebe-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3ebe-122">Authorization</span></span>|<span data-ttu-id="b3ebe-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3ebe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3ebe-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b3ebe-124">Accept</span></span>|<span data-ttu-id="b3ebe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b3ebe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3ebe-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3ebe-126">Request body</span></span>
<span data-ttu-id="b3ebe-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b3ebe-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3ebe-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3ebe-128">Response</span></span>
<span data-ttu-id="b3ebe-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3ebe-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3ebe-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3ebe-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3ebe-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3ebe-131">Request</span></span>
<span data-ttu-id="b3ebe-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3ebe-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
```

### <a name="response"></a><span data-ttu-id="b3ebe-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3ebe-133">Response</span></span>
<span data-ttu-id="b3ebe-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3ebe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 570

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptPolicySetItem",
      "id": "b6b82c18-2c18-b6b8-182c-b8b6182cb8b6",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "payloadId": "Payload Id value",
      "itemType": "Item Type value",
      "displayName": "Display Name value",
      "status": "validating",
      "errorCode": "unauthorized",
      "guidedDeploymentTags": [
        "Guided Deployment Tags value"
      ]
    }
  ]
}
```






