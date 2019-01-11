---
title: Listar windowsDefenderAdvancedThreatProtectionConfigurations
description: Listar propriedades e relações dos objetos windowsDefenderAdvancedThreatProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d8a9b6461431281db63b93017748d6b7b2c6bd27
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826408"
---
# <a name="list-windowsdefenderadvancedthreatprotectionconfigurations"></a><span data-ttu-id="d6ef1-103">Listar windowsDefenderAdvancedThreatProtectionConfigurations</span><span class="sxs-lookup"><span data-stu-id="d6ef1-103">List windowsDefenderAdvancedThreatProtectionConfigurations</span></span>

> <span data-ttu-id="d6ef1-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d6ef1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6ef1-105">Listar propriedades e relações dos objetos [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6ef1-105">List properties and relationships of the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d6ef1-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d6ef1-106">Prerequisites</span></span>
<span data-ttu-id="d6ef1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6ef1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6ef1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6ef1-109">Permission type</span></span>|<span data-ttu-id="d6ef1-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d6ef1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6ef1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6ef1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d6ef1-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6ef1-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d6ef1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6ef1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6ef1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6ef1-114">Not supported.</span></span>|
|<span data-ttu-id="d6ef1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6ef1-115">Application</span></span>|<span data-ttu-id="d6ef1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6ef1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6ef1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6ef1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d6ef1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6ef1-118">Request headers</span></span>
|<span data-ttu-id="d6ef1-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d6ef1-119">Header</span></span>|<span data-ttu-id="d6ef1-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d6ef1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6ef1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6ef1-121">Authorization</span></span>|<span data-ttu-id="d6ef1-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6ef1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6ef1-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d6ef1-123">Accept</span></span>|<span data-ttu-id="d6ef1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d6ef1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6ef1-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6ef1-125">Request body</span></span>
<span data-ttu-id="d6ef1-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d6ef1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6ef1-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6ef1-127">Response</span></span>
<span data-ttu-id="d6ef1-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6ef1-128">If successful, this method returns a `200 OK` response code and a collection of [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6ef1-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6ef1-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="d6ef1-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6ef1-130">Request</span></span>
<span data-ttu-id="d6ef1-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6ef1-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="d6ef1-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6ef1-132">Response</span></span>
<span data-ttu-id="d6ef1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6ef1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



