---
title: Listar iosLobAppProvisioningConfigurationPolicySetItems
description: Listar propriedades e relações dos objetos iosLobAppProvisioningConfigurationPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a35506429ab9852f71bef6f8c72c9ceee46ac9d3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156713"
---
# <a name="list-ioslobappprovisioningconfigurationpolicysetitems"></a><span data-ttu-id="7cecc-103">Listar iosLobAppProvisioningConfigurationPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="7cecc-103">List iosLobAppProvisioningConfigurationPolicySetItems</span></span>

<span data-ttu-id="7cecc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7cecc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7cecc-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7cecc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7cecc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7cecc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7cecc-107">Listar propriedades e relações dos [objetos iosLobAppProvisioningConfigurationPolicySetItem.](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="7cecc-107">List properties and relationships of the [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7cecc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7cecc-108">Prerequisites</span></span>
<span data-ttu-id="7cecc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cecc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cecc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7cecc-111">Permission type</span></span>|<span data-ttu-id="7cecc-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7cecc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cecc-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7cecc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7cecc-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cecc-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7cecc-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7cecc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cecc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7cecc-116">Not supported.</span></span>|
|<span data-ttu-id="7cecc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7cecc-117">Application</span></span>|<span data-ttu-id="7cecc-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cecc-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cecc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7cecc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="7cecc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7cecc-120">Request headers</span></span>
|<span data-ttu-id="7cecc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7cecc-121">Header</span></span>|<span data-ttu-id="7cecc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7cecc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7cecc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7cecc-123">Authorization</span></span>|<span data-ttu-id="7cecc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7cecc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7cecc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7cecc-125">Accept</span></span>|<span data-ttu-id="7cecc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7cecc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cecc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7cecc-127">Request body</span></span>
<span data-ttu-id="7cecc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7cecc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7cecc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cecc-129">Response</span></span>
<span data-ttu-id="7cecc-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7cecc-130">If successful, this method returns a `200 OK` response code and a collection of [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cecc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7cecc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7cecc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7cecc-132">Request</span></span>
<span data-ttu-id="7cecc-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7cecc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
```

### <a name="response"></a><span data-ttu-id="7cecc-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cecc-134">Response</span></span>
<span data-ttu-id="7cecc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7cecc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 582

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationPolicySetItem",
      "id": "6a978d58-8d58-6a97-588d-976a588d976a",
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




