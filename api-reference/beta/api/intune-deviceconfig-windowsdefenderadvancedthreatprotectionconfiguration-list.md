---
title: Listar windowsDefenderAdvancedThreatProtectionConfigurations
description: Listar propriedades e relações dos objetos windowsDefenderAdvancedThreatProtectionConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8d77035d942ddd34cbf3629d760df6e327eeab67
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401576"
---
# <a name="list-windowsdefenderadvancedthreatprotectionconfigurations"></a><span data-ttu-id="e79e0-103">Listar windowsDefenderAdvancedThreatProtectionConfigurations</span><span class="sxs-lookup"><span data-stu-id="e79e0-103">List windowsDefenderAdvancedThreatProtectionConfigurations</span></span>

> <span data-ttu-id="e79e0-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="e79e0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e79e0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e79e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e79e0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e79e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e79e0-107">Listar propriedades e relações dos objetos [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e79e0-107">List properties and relationships of the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e79e0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e79e0-108">Prerequisites</span></span>
<span data-ttu-id="e79e0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e79e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e79e0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e79e0-111">Permission type</span></span>|<span data-ttu-id="e79e0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e79e0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e79e0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e79e0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e79e0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e79e0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e79e0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e79e0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e79e0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e79e0-116">Not supported.</span></span>|
|<span data-ttu-id="e79e0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e79e0-117">Application</span></span>|<span data-ttu-id="e79e0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e79e0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e79e0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e79e0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e79e0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e79e0-120">Request headers</span></span>
|<span data-ttu-id="e79e0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e79e0-121">Header</span></span>|<span data-ttu-id="e79e0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e79e0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e79e0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e79e0-123">Authorization</span></span>|<span data-ttu-id="e79e0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e79e0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e79e0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e79e0-125">Accept</span></span>|<span data-ttu-id="e79e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e79e0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e79e0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e79e0-127">Request body</span></span>
<span data-ttu-id="e79e0-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e79e0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e79e0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e79e0-129">Response</span></span>
<span data-ttu-id="e79e0-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e79e0-130">If successful, this method returns a `200 OK` response code and a collection of [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e79e0-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e79e0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e79e0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e79e0-132">Request</span></span>
<span data-ttu-id="e79e0-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e79e0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="e79e0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e79e0-134">Response</span></span>
<span data-ttu-id="e79e0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e79e0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1107

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
      "id": "294373aa-73aa-2943-aa73-4329aa734329",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "advancedThreatProtectionOnboardingBlob": "Advanced Threat Protection Onboarding Blob value",
      "advancedThreatProtectionOnboardingFilename": "Advanced Threat Protection Onboarding Filename value",
      "advancedThreatProtectionAutoPopulateOnboardingBlob": true,
      "allowSampleSharing": true,
      "enableExpeditedTelemetryReporting": true,
      "advancedThreatProtectionOffboardingBlob": "Advanced Threat Protection Offboarding Blob value",
      "advancedThreatProtectionOffboardingFilename": "Advanced Threat Protection Offboarding Filename value"
    }
  ]
}
```




