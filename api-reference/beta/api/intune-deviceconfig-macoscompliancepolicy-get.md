---
title: Get macOSCompliancePolicy
description: Ler propriedades e relações do objeto macOSCompliancePolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cf31a9fefbb1e98f331f2fe87ac69ffbefdf15cc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419706"
---
# <a name="get-macoscompliancepolicy"></a><span data-ttu-id="4e095-103">Get macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="4e095-103">Get macOSCompliancePolicy</span></span>

> <span data-ttu-id="4e095-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="4e095-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4e095-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4e095-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e095-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="4e095-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e095-107">Ler propriedades e relações do objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4e095-107">Read properties and relationships of the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e095-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4e095-108">Prerequisites</span></span>
<span data-ttu-id="4e095-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4e095-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4e095-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e095-111">Permission type</span></span>|<span data-ttu-id="4e095-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4e095-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e095-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e095-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e095-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e095-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4e095-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e095-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e095-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e095-116">Not supported.</span></span>|
|<span data-ttu-id="4e095-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e095-117">Application</span></span>|<span data-ttu-id="4e095-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e095-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e095-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e095-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4e095-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4e095-120">Optional query parameters</span></span>
<span data-ttu-id="4e095-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4e095-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4e095-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e095-122">Request headers</span></span>
|<span data-ttu-id="4e095-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4e095-123">Header</span></span>|<span data-ttu-id="4e095-124">Valor</span><span class="sxs-lookup"><span data-stu-id="4e095-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e095-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e095-125">Authorization</span></span>|<span data-ttu-id="4e095-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e095-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e095-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4e095-127">Accept</span></span>|<span data-ttu-id="4e095-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4e095-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e095-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e095-129">Request body</span></span>
<span data-ttu-id="4e095-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4e095-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e095-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e095-131">Response</span></span>
<span data-ttu-id="4e095-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e095-132">If successful, this method returns a `200 OK` response code and [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e095-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4e095-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e095-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e095-134">Request</span></span>
<span data-ttu-id="4e095-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e095-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="4e095-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e095-136">Response</span></span>
<span data-ttu-id="4e095-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4e095-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




