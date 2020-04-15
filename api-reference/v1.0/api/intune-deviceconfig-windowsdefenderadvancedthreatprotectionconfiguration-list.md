---
title: Listar windowsDefenderAdvancedThreatProtectionConfigurations
description: Listar propriedades e relações dos objetos windowsDefenderAdvancedThreatProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 822dbf8431b9b5932bbfa75113de300f4367960c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462037"
---
# <a name="list-windowsdefenderadvancedthreatprotectionconfigurations"></a><span data-ttu-id="0c8fe-103">Listar windowsDefenderAdvancedThreatProtectionConfigurations</span><span class="sxs-lookup"><span data-stu-id="0c8fe-103">List windowsDefenderAdvancedThreatProtectionConfigurations</span></span>

<span data-ttu-id="0c8fe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c8fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c8fe-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0c8fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c8fe-106">Listar propriedades e relações dos objetos [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c8fe-106">List properties and relationships of the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c8fe-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0c8fe-107">Prerequisites</span></span>
<span data-ttu-id="0c8fe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c8fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c8fe-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c8fe-110">Permission type</span></span>|<span data-ttu-id="0c8fe-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0c8fe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c8fe-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c8fe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c8fe-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c8fe-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0c8fe-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c8fe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c8fe-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c8fe-115">Not supported.</span></span>|
|<span data-ttu-id="0c8fe-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c8fe-116">Application</span></span>|<span data-ttu-id="0c8fe-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c8fe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c8fe-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c8fe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0c8fe-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c8fe-119">Request headers</span></span>
|<span data-ttu-id="0c8fe-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0c8fe-120">Header</span></span>|<span data-ttu-id="0c8fe-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0c8fe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c8fe-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c8fe-122">Authorization</span></span>|<span data-ttu-id="0c8fe-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c8fe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c8fe-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0c8fe-124">Accept</span></span>|<span data-ttu-id="0c8fe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0c8fe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c8fe-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c8fe-126">Request body</span></span>
<span data-ttu-id="0c8fe-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0c8fe-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c8fe-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c8fe-128">Response</span></span>
<span data-ttu-id="0c8fe-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c8fe-129">If successful, this method returns a `200 OK` response code and a collection of [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c8fe-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c8fe-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c8fe-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c8fe-131">Request</span></span>
<span data-ttu-id="0c8fe-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c8fe-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="0c8fe-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c8fe-133">Response</span></span>
<span data-ttu-id="0c8fe-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c8fe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 508

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
      "id": "294373aa-73aa-2943-aa73-4329aa734329",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "allowSampleSharing": true,
      "enableExpeditedTelemetryReporting": true
    }
  ]
}
```






