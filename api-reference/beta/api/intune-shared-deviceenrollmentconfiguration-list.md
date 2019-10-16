---
title: Listar deviceEnrollmentConfigurations
description: Listar propriedades e relações de objetos de deviceEnrollmentConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 42571fa9e33b86d348e9533a6fccd5912578f791
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537019"
---
# <a name="list-deviceenrollmentconfigurations"></a><span data-ttu-id="3d9e5-103">Listar deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="3d9e5-103">List deviceEnrollmentConfigurations</span></span>

> <span data-ttu-id="3d9e5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3d9e5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d9e5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3d9e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d9e5-106">Listar propriedades e relações de objetos de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d9e5-106">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d9e5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3d9e5-107">Prerequisites</span></span>
<span data-ttu-id="3d9e5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d9e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d9e5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d9e5-110">Permission type</span></span>|<span data-ttu-id="3d9e5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3d9e5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d9e5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d9e5-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3d9e5-113">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="3d9e5-113">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="3d9e5-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d9e5-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="3d9e5-115">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="3d9e5-115">&nbsp; &nbsp; **Policy Set**</span></span>| <span data-ttu-id="3d9e5-116">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d9e5-116">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="3d9e5-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d9e5-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d9e5-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d9e5-118">Not supported.</span></span>|
|<span data-ttu-id="3d9e5-119">Application</span><span class="sxs-lookup"><span data-stu-id="3d9e5-119">Application</span></span>||
| <span data-ttu-id="3d9e5-120">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="3d9e5-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="3d9e5-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d9e5-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="3d9e5-122">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="3d9e5-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="3d9e5-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d9e5-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d9e5-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d9e5-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3d9e5-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d9e5-125">Request headers</span></span>
|<span data-ttu-id="3d9e5-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3d9e5-126">Header</span></span>|<span data-ttu-id="3d9e5-127">Valor</span><span class="sxs-lookup"><span data-stu-id="3d9e5-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d9e5-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d9e5-128">Authorization</span></span>|<span data-ttu-id="3d9e5-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d9e5-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d9e5-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3d9e5-130">Accept</span></span>|<span data-ttu-id="3d9e5-131">application/json</span><span class="sxs-lookup"><span data-stu-id="3d9e5-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d9e5-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d9e5-132">Request body</span></span>
<span data-ttu-id="3d9e5-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3d9e5-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d9e5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d9e5-134">Response</span></span>
<span data-ttu-id="3d9e5-135">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d9e5-135">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d9e5-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d9e5-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d9e5-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d9e5-137">Request</span></span>
<span data-ttu-id="3d9e5-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d9e5-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="3d9e5-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d9e5-139">Response</span></span>
<span data-ttu-id="3d9e5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3d9e5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 422

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
      "id": "df13d8b9-d8b9-df13-b9d8-13dfb9d813df",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7
    }
  ]
}
```






