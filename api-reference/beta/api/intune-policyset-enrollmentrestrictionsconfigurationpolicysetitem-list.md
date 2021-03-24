---
title: Listar enrollmentRestrictionsConfigurationPolicySetItems
description: Listar propriedades e relações dos objetos enrollmentRestrictionsConfigurationPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ca3df0957405890ec2f62dc73fc88678fc01ead6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148601"
---
# <a name="list-enrollmentrestrictionsconfigurationpolicysetitems"></a><span data-ttu-id="ffb08-103">Listar enrollmentRestrictionsConfigurationPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="ffb08-103">List enrollmentRestrictionsConfigurationPolicySetItems</span></span>

<span data-ttu-id="ffb08-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffb08-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ffb08-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ffb08-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ffb08-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ffb08-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffb08-107">Listar propriedades e relações dos objetos [enrollmentRestrictionsConfigurationPolicySetItem.](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="ffb08-107">List properties and relationships of the [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ffb08-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ffb08-108">Prerequisites</span></span>
<span data-ttu-id="ffb08-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffb08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffb08-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ffb08-111">Permission type</span></span>|<span data-ttu-id="ffb08-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ffb08-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffb08-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ffb08-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ffb08-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffb08-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ffb08-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ffb08-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffb08-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ffb08-116">Not supported.</span></span>|
|<span data-ttu-id="ffb08-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ffb08-117">Application</span></span>|<span data-ttu-id="ffb08-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffb08-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffb08-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ffb08-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="ffb08-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ffb08-120">Request headers</span></span>
|<span data-ttu-id="ffb08-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ffb08-121">Header</span></span>|<span data-ttu-id="ffb08-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ffb08-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffb08-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ffb08-123">Authorization</span></span>|<span data-ttu-id="ffb08-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ffb08-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffb08-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ffb08-125">Accept</span></span>|<span data-ttu-id="ffb08-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ffb08-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffb08-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ffb08-127">Request body</span></span>
<span data-ttu-id="ffb08-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ffb08-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffb08-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ffb08-129">Response</span></span>
<span data-ttu-id="ffb08-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objetos enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ffb08-130">If successful, this method returns a `200 OK` response code and a collection of [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffb08-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ffb08-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ffb08-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ffb08-132">Request</span></span>
<span data-ttu-id="ffb08-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ffb08-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
```

### <a name="response"></a><span data-ttu-id="ffb08-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ffb08-134">Response</span></span>
<span data-ttu-id="ffb08-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ffb08-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 624

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.enrollmentRestrictionsConfigurationPolicySetItem",
      "id": "08c4f0b1-f0b1-08c4-b1f0-c408b1f0c408",
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
      "priority": 8,
      "limit": 5
    }
  ]
}
```




