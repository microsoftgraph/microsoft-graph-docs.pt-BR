---
title: Get macOSCompliancePolicy
description: Ler propriedades e relações do objeto macOSCompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6d659d5f3c9e3870310d90ede3e1e37901f1b0e5
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366101"
---
# <a name="get-macoscompliancepolicy"></a><span data-ttu-id="2a193-103">Get macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="2a193-103">Get macOSCompliancePolicy</span></span>

> <span data-ttu-id="2a193-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2a193-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a193-105">Ler propriedades e relações do objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2a193-105">Read properties and relationships of the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a193-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2a193-106">Prerequisites</span></span>
<span data-ttu-id="2a193-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a193-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a193-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a193-109">Permission type</span></span>|<span data-ttu-id="2a193-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2a193-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a193-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a193-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2a193-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a193-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2a193-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a193-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a193-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a193-114">Not supported.</span></span>|
|<span data-ttu-id="2a193-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a193-115">Application</span></span>|<span data-ttu-id="2a193-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a193-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a193-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a193-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2a193-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2a193-118">Optional query parameters</span></span>
<span data-ttu-id="2a193-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2a193-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a193-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a193-120">Request headers</span></span>
|<span data-ttu-id="2a193-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2a193-121">Header</span></span>|<span data-ttu-id="2a193-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2a193-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a193-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a193-123">Authorization</span></span>|<span data-ttu-id="2a193-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a193-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a193-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2a193-125">Accept</span></span>|<span data-ttu-id="2a193-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2a193-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a193-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a193-127">Request body</span></span>
<span data-ttu-id="2a193-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2a193-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a193-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a193-129">Response</span></span>
<span data-ttu-id="2a193-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a193-130">If successful, this method returns a `200 OK` response code and [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a193-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a193-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a193-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a193-132">Request</span></span>
<span data-ttu-id="2a193-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a193-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="2a193-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a193-134">Response</span></span>
<span data-ttu-id="2a193-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a193-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1088

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
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
    "firewallEnabled": true,
    "firewallBlockAllIncoming": true,
    "firewallEnableStealthMode": true
  }
}
```




