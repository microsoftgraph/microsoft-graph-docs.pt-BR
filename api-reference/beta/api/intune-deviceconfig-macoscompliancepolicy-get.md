---
title: Get macOSCompliancePolicy
description: Ler propriedades e relações do objeto macOSCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ea29aa15665142de63411e85f7946ceee454bf65
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38083743"
---
# <a name="get-macoscompliancepolicy"></a><span data-ttu-id="0de40-103">Get macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="0de40-103">Get macOSCompliancePolicy</span></span>

> <span data-ttu-id="0de40-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0de40-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0de40-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0de40-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0de40-106">Ler propriedades e relações do objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0de40-106">Read properties and relationships of the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0de40-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0de40-107">Prerequisites</span></span>
<span data-ttu-id="0de40-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0de40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0de40-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0de40-110">Permission type</span></span>|<span data-ttu-id="0de40-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0de40-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0de40-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0de40-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0de40-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0de40-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0de40-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0de40-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0de40-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0de40-115">Not supported.</span></span>|
|<span data-ttu-id="0de40-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0de40-116">Application</span></span>|<span data-ttu-id="0de40-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0de40-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0de40-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0de40-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0de40-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0de40-119">Optional query parameters</span></span>
<span data-ttu-id="0de40-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0de40-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0de40-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0de40-121">Request headers</span></span>
|<span data-ttu-id="0de40-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0de40-122">Header</span></span>|<span data-ttu-id="0de40-123">Valor</span><span class="sxs-lookup"><span data-stu-id="0de40-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0de40-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0de40-124">Authorization</span></span>|<span data-ttu-id="0de40-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0de40-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0de40-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0de40-126">Accept</span></span>|<span data-ttu-id="0de40-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0de40-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0de40-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0de40-128">Request body</span></span>
<span data-ttu-id="0de40-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0de40-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0de40-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="0de40-130">Response</span></span>
<span data-ttu-id="0de40-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0de40-131">If successful, this method returns a `200 OK` response code and [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0de40-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0de40-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0de40-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0de40-133">Request</span></span>
<span data-ttu-id="0de40-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0de40-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="0de40-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0de40-135">Response</span></span>
<span data-ttu-id="0de40-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0de40-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1334

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "ddbadff3-dff3-ddba-f3df-baddf3dfbadd",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordRequired": true,
    "passwordBlockSimple": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "osMinimumBuildVersion": "Os Minimum Build Version value",
    "osMaximumBuildVersion": "Os Maximum Build Version value",
    "systemIntegrityProtectionEnabled": true,
    "deviceThreatProtectionEnabled": true,
    "deviceThreatProtectionRequiredSecurityLevel": "secured",
    "storageRequireEncryption": true,
    "gatekeeperAllowedAppSource": "macAppStore",
    "firewallEnabled": true,
    "firewallBlockAllIncoming": true,
    "firewallEnableStealthMode": true
  }
}
```






