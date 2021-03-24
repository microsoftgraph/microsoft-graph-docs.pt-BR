---
title: Listar managedDeviceMobileAppConfigurationPolicySetItems
description: Listar propriedades e relações dos objetos managedDeviceMobileAppConfigurationPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a1e78c3094df462e600e32d3f9f16df4cab9d3ff
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145135"
---
# <a name="list-manageddevicemobileappconfigurationpolicysetitems"></a><span data-ttu-id="73e27-103">Listar managedDeviceMobileAppConfigurationPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="73e27-103">List managedDeviceMobileAppConfigurationPolicySetItems</span></span>

<span data-ttu-id="73e27-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73e27-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73e27-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="73e27-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73e27-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="73e27-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73e27-107">Listar propriedades e relações dos [objetos managedDeviceMobileAppConfigurationPolicySetItem.](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="73e27-107">List properties and relationships of the [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73e27-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="73e27-108">Prerequisites</span></span>
<span data-ttu-id="73e27-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73e27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73e27-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73e27-111">Permission type</span></span>|<span data-ttu-id="73e27-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="73e27-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73e27-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73e27-113">Delegated (work or school account)</span></span>|<span data-ttu-id="73e27-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73e27-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="73e27-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73e27-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73e27-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73e27-116">Not supported.</span></span>|
|<span data-ttu-id="73e27-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73e27-117">Application</span></span>|<span data-ttu-id="73e27-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73e27-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="73e27-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73e27-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="73e27-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73e27-120">Request headers</span></span>
|<span data-ttu-id="73e27-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="73e27-121">Header</span></span>|<span data-ttu-id="73e27-122">Valor</span><span class="sxs-lookup"><span data-stu-id="73e27-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73e27-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="73e27-123">Authorization</span></span>|<span data-ttu-id="73e27-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73e27-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73e27-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="73e27-125">Accept</span></span>|<span data-ttu-id="73e27-126">application/json</span><span class="sxs-lookup"><span data-stu-id="73e27-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73e27-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73e27-127">Request body</span></span>
<span data-ttu-id="73e27-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="73e27-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73e27-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="73e27-129">Response</span></span>
<span data-ttu-id="73e27-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73e27-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73e27-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73e27-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="73e27-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73e27-132">Request</span></span>
<span data-ttu-id="73e27-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="73e27-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
```

### <a name="response"></a><span data-ttu-id="73e27-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="73e27-134">Response</span></span>
<span data-ttu-id="73e27-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73e27-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 583

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationPolicySetItem",
      "id": "bb065442-5442-bb06-4254-06bb425406bb",
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




