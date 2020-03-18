---
title: Listar deviceCompliancePolicyPolicySetItems
description: Listar Propriedades e relações dos objetos deviceCompliancePolicyPolicySetItem.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d949e5312934c817d45c73eed8b788632634b823
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802437"
---
# <a name="list-devicecompliancepolicypolicysetitems"></a><span data-ttu-id="ca186-103">Listar deviceCompliancePolicyPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="ca186-103">List deviceCompliancePolicyPolicySetItems</span></span>

> <span data-ttu-id="ca186-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ca186-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca186-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ca186-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca186-106">Listar Propriedades e relações dos objetos [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="ca186-106">List properties and relationships of the [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca186-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ca186-107">Prerequisites</span></span>
<span data-ttu-id="ca186-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca186-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca186-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca186-110">Permission type</span></span>|<span data-ttu-id="ca186-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ca186-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca186-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca186-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ca186-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca186-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ca186-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca186-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca186-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca186-115">Not supported.</span></span>|
|<span data-ttu-id="ca186-116">Application</span><span class="sxs-lookup"><span data-stu-id="ca186-116">Application</span></span>|<span data-ttu-id="ca186-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca186-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca186-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca186-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="ca186-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca186-119">Request headers</span></span>
|<span data-ttu-id="ca186-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ca186-120">Header</span></span>|<span data-ttu-id="ca186-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ca186-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca186-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca186-122">Authorization</span></span>|<span data-ttu-id="ca186-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca186-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca186-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ca186-124">Accept</span></span>|<span data-ttu-id="ca186-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ca186-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca186-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca186-126">Request body</span></span>
<span data-ttu-id="ca186-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ca186-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca186-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca186-128">Response</span></span>
<span data-ttu-id="ca186-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca186-129">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca186-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca186-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca186-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca186-131">Request</span></span>
<span data-ttu-id="ca186-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca186-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
```

### <a name="response"></a><span data-ttu-id="ca186-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca186-133">Response</span></span>
<span data-ttu-id="ca186-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca186-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 570

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicyPolicySetItem",
      "id": "5c0bc827-c827-5c0b-27c8-0b5c27c80b5c",
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




