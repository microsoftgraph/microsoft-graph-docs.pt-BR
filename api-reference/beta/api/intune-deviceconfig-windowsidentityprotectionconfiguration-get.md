---
title: Obter windowsIdentityProtectionConfiguration
description: Leia as propriedades e os relacionamentos do objeto windowsIdentityProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fde8d4dcb8c7a5b94069466757d6c2ffb1351355
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880994"
---
# <a name="get-windowsidentityprotectionconfiguration"></a><span data-ttu-id="52bf6-103">Obter windowsIdentityProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="52bf6-103">Get windowsIdentityProtectionConfiguration</span></span>

> <span data-ttu-id="52bf6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="52bf6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52bf6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="52bf6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="52bf6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="52bf6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="52bf6-107">Leia as propriedades e os relacionamentos do objeto [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="52bf6-107">Read properties and relationships of the [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="52bf6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="52bf6-108">Prerequisites</span></span>
<span data-ttu-id="52bf6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52bf6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52bf6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52bf6-111">Permission type</span></span>|<span data-ttu-id="52bf6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="52bf6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52bf6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52bf6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="52bf6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="52bf6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="52bf6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52bf6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52bf6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52bf6-116">Not supported.</span></span>|
|<span data-ttu-id="52bf6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52bf6-117">Application</span></span>|<span data-ttu-id="52bf6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52bf6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52bf6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52bf6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="52bf6-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="52bf6-120">Optional query parameters</span></span>
<span data-ttu-id="52bf6-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="52bf6-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="52bf6-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52bf6-122">Request headers</span></span>
|<span data-ttu-id="52bf6-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="52bf6-123">Header</span></span>|<span data-ttu-id="52bf6-124">Valor</span><span class="sxs-lookup"><span data-stu-id="52bf6-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52bf6-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="52bf6-125">Authorization</span></span>|<span data-ttu-id="52bf6-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52bf6-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52bf6-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="52bf6-127">Accept</span></span>|<span data-ttu-id="52bf6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="52bf6-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52bf6-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52bf6-129">Request body</span></span>
<span data-ttu-id="52bf6-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="52bf6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52bf6-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="52bf6-131">Response</span></span>
<span data-ttu-id="52bf6-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52bf6-132">If successful, this method returns a `200 OK` response code and [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52bf6-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52bf6-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="52bf6-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52bf6-134">Request</span></span>
<span data-ttu-id="52bf6-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52bf6-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="52bf6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="52bf6-136">Response</span></span>
<span data-ttu-id="52bf6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52bf6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1013

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
    "id": "b2e64303-4303-b2e6-0343-e6b20343e6b2",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
    "pinMinimumLength": 0,
    "pinMaximumLength": 0,
    "pinUppercaseCharactersUsage": "required",
    "pinLowercaseCharactersUsage": "required",
    "pinSpecialCharactersUsage": "required",
    "pinExpirationInDays": 3,
    "pinPreviousBlockCount": 5,
    "pinRecoveryEnabled": true,
    "securityDeviceRequired": true,
    "unlockWithBiometricsEnabled": true,
    "useCertificatesForOnPremisesAuthEnabled": true,
    "windowsHelloForBusinessBlocked": true
  }
}
```





