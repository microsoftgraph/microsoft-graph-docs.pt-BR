---
title: Listar managedAppProtectionPolicySetItems
description: Listar Propriedades e relações dos objetos managedAppProtectionPolicySetItem.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2385d83511e3bf7e4803064fb6688a450e1d8fb5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802262"
---
# <a name="list-managedappprotectionpolicysetitems"></a><span data-ttu-id="31788-103">Listar managedAppProtectionPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="31788-103">List managedAppProtectionPolicySetItems</span></span>

> <span data-ttu-id="31788-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="31788-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31788-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="31788-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31788-106">Listar Propriedades e relações dos objetos [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="31788-106">List properties and relationships of the [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31788-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="31788-107">Prerequisites</span></span>
<span data-ttu-id="31788-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31788-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31788-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31788-110">Permission type</span></span>|<span data-ttu-id="31788-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="31788-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31788-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31788-112">Delegated (work or school account)</span></span>|<span data-ttu-id="31788-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="31788-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="31788-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31788-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31788-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31788-115">Not supported.</span></span>|
|<span data-ttu-id="31788-116">Application</span><span class="sxs-lookup"><span data-stu-id="31788-116">Application</span></span>|<span data-ttu-id="31788-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="31788-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31788-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31788-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="31788-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31788-119">Request headers</span></span>
|<span data-ttu-id="31788-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="31788-120">Header</span></span>|<span data-ttu-id="31788-121">Valor</span><span class="sxs-lookup"><span data-stu-id="31788-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31788-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="31788-122">Authorization</span></span>|<span data-ttu-id="31788-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31788-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31788-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="31788-124">Accept</span></span>|<span data-ttu-id="31788-125">application/json</span><span class="sxs-lookup"><span data-stu-id="31788-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31788-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31788-126">Request body</span></span>
<span data-ttu-id="31788-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="31788-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31788-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="31788-128">Response</span></span>
<span data-ttu-id="31788-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31788-129">If successful, this method returns a `200 OK` response code and a collection of [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31788-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31788-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="31788-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31788-131">Request</span></span>
<span data-ttu-id="31788-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="31788-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
```

### <a name="response"></a><span data-ttu-id="31788-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="31788-133">Response</span></span>
<span data-ttu-id="31788-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31788-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 646

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppProtectionPolicySetItem",
      "id": "e10d79c9-79c9-e10d-c979-0de1c9790de1",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "payloadId": "Payload Id value",
      "itemType": "Item Type value",
      "displayName": "Display Name value",
      "status": "validating",
      "errorCode": "unauthorized",
      "guidedDeploymentTags": [
        "Guided Deployment Tags value"
      ],
      "targetedAppManagementLevels": "Targeted App Management Levels value"
    }
  ]
}
```




