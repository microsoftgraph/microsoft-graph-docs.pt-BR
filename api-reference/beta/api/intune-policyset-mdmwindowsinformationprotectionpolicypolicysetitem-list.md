---
title: Listar mdmWindowsInformationProtectionPolicyPolicySetItems
description: Listar Propriedades e relações dos objetos mdmWindowsInformationProtectionPolicyPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7d1f30cf0ad8889204c9a2655a70354b5b5fa60c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064812"
---
# <a name="list-mdmwindowsinformationprotectionpolicypolicysetitems"></a><span data-ttu-id="abed6-103">Listar mdmWindowsInformationProtectionPolicyPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="abed6-103">List mdmWindowsInformationProtectionPolicyPolicySetItems</span></span>

<span data-ttu-id="abed6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abed6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="abed6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="abed6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abed6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="abed6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abed6-107">Listar Propriedades e relações dos objetos [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="abed6-107">List properties and relationships of the [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abed6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="abed6-108">Prerequisites</span></span>
<span data-ttu-id="abed6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abed6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abed6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="abed6-111">Permission type</span></span>|<span data-ttu-id="abed6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="abed6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abed6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="abed6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="abed6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="abed6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="abed6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="abed6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abed6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abed6-116">Not supported.</span></span>|
|<span data-ttu-id="abed6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="abed6-117">Application</span></span>|<span data-ttu-id="abed6-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="abed6-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="abed6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abed6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="abed6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abed6-120">Request headers</span></span>
|<span data-ttu-id="abed6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="abed6-121">Header</span></span>|<span data-ttu-id="abed6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="abed6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abed6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="abed6-123">Authorization</span></span>|<span data-ttu-id="abed6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="abed6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abed6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="abed6-125">Accept</span></span>|<span data-ttu-id="abed6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="abed6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abed6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abed6-127">Request body</span></span>
<span data-ttu-id="abed6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="abed6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abed6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="abed6-129">Response</span></span>
<span data-ttu-id="abed6-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="abed6-130">If successful, this method returns a `200 OK` response code and a collection of [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abed6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="abed6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="abed6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abed6-132">Request</span></span>
<span data-ttu-id="abed6-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="abed6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
```

### <a name="response"></a><span data-ttu-id="abed6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="abed6-134">Response</span></span>
<span data-ttu-id="abed6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="abed6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 585

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicyPolicySetItem",
      "id": "4ac5be70-be70-4ac5-70be-c54a70bec54a",
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






