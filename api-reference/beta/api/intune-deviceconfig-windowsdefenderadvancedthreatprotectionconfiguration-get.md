---
title: Obter windowsDefenderAdvancedThreatProtectionConfiguration
description: Ler propriedades e relações do objeto windowsDefenderAdvancedThreatProtectionConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 11b9d459e542cc49eb2d1175997477b065a0f7e1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400785"
---
# <a name="get-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="d0c63-103">Obter windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="d0c63-103">Get windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="d0c63-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="d0c63-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d0c63-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d0c63-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d0c63-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="d0c63-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0c63-107">Ler propriedades e relações do objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0c63-107">Read properties and relationships of the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0c63-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d0c63-108">Prerequisites</span></span>
<span data-ttu-id="d0c63-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d0c63-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d0c63-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0c63-111">Permission type</span></span>|<span data-ttu-id="d0c63-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d0c63-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0c63-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0c63-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d0c63-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d0c63-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d0c63-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0c63-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0c63-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0c63-116">Not supported.</span></span>|
|<span data-ttu-id="d0c63-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0c63-117">Application</span></span>|<span data-ttu-id="d0c63-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0c63-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0c63-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0c63-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d0c63-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d0c63-120">Optional query parameters</span></span>
<span data-ttu-id="d0c63-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d0c63-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d0c63-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0c63-122">Request headers</span></span>
|<span data-ttu-id="d0c63-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d0c63-123">Header</span></span>|<span data-ttu-id="d0c63-124">Valor</span><span class="sxs-lookup"><span data-stu-id="d0c63-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0c63-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0c63-125">Authorization</span></span>|<span data-ttu-id="d0c63-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0c63-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0c63-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d0c63-127">Accept</span></span>|<span data-ttu-id="d0c63-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d0c63-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0c63-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0c63-129">Request body</span></span>
<span data-ttu-id="d0c63-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d0c63-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0c63-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0c63-131">Response</span></span>
<span data-ttu-id="d0c63-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0c63-132">If successful, this method returns a `200 OK` response code and [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0c63-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0c63-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0c63-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0c63-134">Request</span></span>
<span data-ttu-id="d0c63-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0c63-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d0c63-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0c63-136">Response</span></span>
<span data-ttu-id="d0c63-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d0c63-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1057

{
  "value": {
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
}
```




