---
title: Listar macOSCompliancePolicies
description: Listar propriedades e relações dos objetos macOSCompliancePolicy.
ms.openlocfilehash: 3164297670b0402bd51428928577f3c3ad4134d9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034808"
---
# <a name="list-macoscompliancepolicies"></a><span data-ttu-id="e1efe-103">Listar macOSCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="e1efe-103">List macOSCompliancePolicies</span></span>

> <span data-ttu-id="e1efe-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e1efe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1efe-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e1efe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1efe-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e1efe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1efe-107">Listar propriedades e relações dos objetos [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e1efe-107">List properties and relationships of the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e1efe-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1efe-108">Prerequisites</span></span>
<span data-ttu-id="e1efe-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1efe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1efe-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1efe-111">Permission type</span></span>|<span data-ttu-id="e1efe-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1efe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1efe-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1efe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1efe-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1efe-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e1efe-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1efe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1efe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1efe-116">Not supported.</span></span>|
|<span data-ttu-id="e1efe-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1efe-117">Application</span></span>|<span data-ttu-id="e1efe-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1efe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1efe-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1efe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="e1efe-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1efe-120">Request headers</span></span>
|<span data-ttu-id="e1efe-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1efe-121">Header</span></span>|<span data-ttu-id="e1efe-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e1efe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1efe-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1efe-123">Authorization</span></span>|<span data-ttu-id="e1efe-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1efe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1efe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e1efe-125">Accept</span></span>|<span data-ttu-id="e1efe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1efe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1efe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1efe-127">Request body</span></span>
<span data-ttu-id="e1efe-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1efe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1efe-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1efe-129">Response</span></span>
<span data-ttu-id="e1efe-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1efe-130">If successful, this method returns a `200 OK` response code and a collection of [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1efe-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1efe-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e1efe-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1efe-132">Request</span></span>
<span data-ttu-id="e1efe-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1efe-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="e1efe-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1efe-134">Response</span></span>
<span data-ttu-id="e1efe-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1efe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1276

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





