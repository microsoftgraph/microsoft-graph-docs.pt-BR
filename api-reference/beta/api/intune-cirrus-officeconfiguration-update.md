---
title: Atualizar officeConfiguration
description: Atualiza as propriedades de um objeto officeConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e452a3743148b4767c1259d68746924d3b0675c4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725820"
---
# <a name="update-officeconfiguration"></a><span data-ttu-id="2bff0-103">Atualizar officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="2bff0-103">Update officeConfiguration</span></span>

> <span data-ttu-id="2bff0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2bff0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2bff0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2bff0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bff0-106">Atualiza as propriedades de um objeto [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2bff0-106">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2bff0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2bff0-107">Prerequisites</span></span>
<span data-ttu-id="2bff0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bff0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bff0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2bff0-110">Permission type</span></span>|<span data-ttu-id="2bff0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2bff0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bff0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2bff0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2bff0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bff0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2bff0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2bff0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bff0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2bff0-115">Not supported.</span></span>|
|<span data-ttu-id="2bff0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2bff0-116">Application</span></span>|<span data-ttu-id="2bff0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2bff0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bff0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2bff0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="2bff0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2bff0-119">Request headers</span></span>
|<span data-ttu-id="2bff0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2bff0-120">Header</span></span>|<span data-ttu-id="2bff0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2bff0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bff0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2bff0-122">Authorization</span></span>|<span data-ttu-id="2bff0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2bff0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bff0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2bff0-124">Accept</span></span>|<span data-ttu-id="2bff0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2bff0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bff0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2bff0-126">Request body</span></span>
<span data-ttu-id="2bff0-127">No corpo da solicitação, forneça uma representação JSON do objeto [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2bff0-127">In the request body, supply a JSON representation for the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>

<span data-ttu-id="2bff0-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2bff0-128">The following table shows the properties that are required when you create the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md).</span></span>

|<span data-ttu-id="2bff0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2bff0-129">Property</span></span>|<span data-ttu-id="2bff0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2bff0-130">Type</span></span>|<span data-ttu-id="2bff0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bff0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bff0-132">id</span><span class="sxs-lookup"><span data-stu-id="2bff0-132">id</span></span>|<span data-ttu-id="2bff0-133">String</span><span class="sxs-lookup"><span data-stu-id="2bff0-133">String</span></span>|<span data-ttu-id="2bff0-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2bff0-134">Not yet documented</span></span>|
|<span data-ttu-id="2bff0-135">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="2bff0-135">tenantCheckinStatuses</span></span>|<span data-ttu-id="2bff0-136">coleção [officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="2bff0-136">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="2bff0-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2bff0-137">Not yet documented</span></span>|
|<span data-ttu-id="2bff0-138">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="2bff0-138">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="2bff0-139">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="2bff0-139">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="2bff0-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2bff0-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2bff0-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bff0-141">Response</span></span>
<span data-ttu-id="2bff0-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2bff0-142">If successful, this method returns a `200 OK` response code and an updated [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bff0-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2bff0-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bff0-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2bff0-144">Request</span></span>
<span data-ttu-id="2bff0-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2bff0-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/officeConfiguration
Content-type: application/json
Content-length: 843

{
  "@odata.type": "#microsoft.graph.officeConfiguration",
  "tenantCheckinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userId": "User Id value",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ],
      "lastTaskName": "Last Task Name value"
    }
  ],
  "tenantUserCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  }
}
```

### <a name="response"></a><span data-ttu-id="2bff0-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bff0-146">Response</span></span>
<span data-ttu-id="2bff0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2bff0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 892

{
  "@odata.type": "#microsoft.graph.officeConfiguration",
  "id": "4b5f7085-7085-4b5f-8570-5f4b85705f4b",
  "tenantCheckinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userId": "User Id value",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ],
      "lastTaskName": "Last Task Name value"
    }
  ],
  "tenantUserCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  }
}
```





