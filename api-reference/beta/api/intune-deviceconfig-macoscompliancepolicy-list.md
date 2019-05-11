---
title: Listar macOSCompliancePolicies
description: Listar propriedades e relações dos objetos macOSCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 99874ea538b5fc8e654c1d3965f27789219ebd28
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33922933"
---
# <a name="list-macoscompliancepolicies"></a><span data-ttu-id="2a253-103">Listar macOSCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="2a253-103">List macOSCompliancePolicies</span></span>

> <span data-ttu-id="2a253-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2a253-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a253-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2a253-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a253-106">Listar propriedades e relações dos objetos [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2a253-106">List properties and relationships of the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a253-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2a253-107">Prerequisites</span></span>
<span data-ttu-id="2a253-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a253-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a253-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a253-110">Permission type</span></span>|<span data-ttu-id="2a253-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2a253-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a253-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a253-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2a253-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a253-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2a253-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a253-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a253-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a253-115">Not supported.</span></span>|
|<span data-ttu-id="2a253-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a253-116">Application</span></span>|<span data-ttu-id="2a253-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a253-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a253-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a253-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="2a253-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a253-119">Request headers</span></span>
|<span data-ttu-id="2a253-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2a253-120">Header</span></span>|<span data-ttu-id="2a253-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2a253-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a253-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a253-122">Authorization</span></span>|<span data-ttu-id="2a253-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a253-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a253-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2a253-124">Accept</span></span>|<span data-ttu-id="2a253-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2a253-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a253-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a253-126">Request body</span></span>
<span data-ttu-id="2a253-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2a253-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a253-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a253-128">Response</span></span>
<span data-ttu-id="2a253-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a253-129">If successful, this method returns a `200 OK` response code and a collection of [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a253-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a253-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a253-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a253-131">Request</span></span>
<span data-ttu-id="2a253-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a253-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="2a253-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a253-133">Response</span></span>
<span data-ttu-id="2a253-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a253-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1408

{
  "value": [
    {
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
  ]
}
```




