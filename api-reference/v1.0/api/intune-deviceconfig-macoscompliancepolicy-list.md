---
title: Listar macOSCompliancePolicies
description: Listar propriedades e relações dos objetos macOSCompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cceb6b5d1d3025b75a9545670f8737ba3797ab0f
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366087"
---
# <a name="list-macoscompliancepolicies"></a><span data-ttu-id="a30a8-103">Listar macOSCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="a30a8-103">List macOSCompliancePolicies</span></span>

> <span data-ttu-id="a30a8-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a30a8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a30a8-105">Listar propriedades e relações dos objetos [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a30a8-105">List properties and relationships of the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a30a8-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a30a8-106">Prerequisites</span></span>
<span data-ttu-id="a30a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a30a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a30a8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a30a8-109">Permission type</span></span>|<span data-ttu-id="a30a8-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a30a8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a30a8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a30a8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a30a8-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a30a8-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a30a8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a30a8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a30a8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a30a8-114">Not supported.</span></span>|
|<span data-ttu-id="a30a8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a30a8-115">Application</span></span>|<span data-ttu-id="a30a8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a30a8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a30a8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a30a8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="a30a8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a30a8-118">Request headers</span></span>
|<span data-ttu-id="a30a8-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a30a8-119">Header</span></span>|<span data-ttu-id="a30a8-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a30a8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a30a8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a30a8-121">Authorization</span></span>|<span data-ttu-id="a30a8-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a30a8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a30a8-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a30a8-123">Accept</span></span>|<span data-ttu-id="a30a8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a30a8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a30a8-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a30a8-125">Request body</span></span>
<span data-ttu-id="a30a8-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a30a8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a30a8-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a30a8-127">Response</span></span>
<span data-ttu-id="a30a8-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a30a8-128">If successful, this method returns a `200 OK` response code and a collection of [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a30a8-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a30a8-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a30a8-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a30a8-130">Request</span></span>
<span data-ttu-id="a30a8-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a30a8-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="a30a8-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a30a8-132">Response</span></span>
<span data-ttu-id="a30a8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a30a8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1150

{
  "value": [
    {
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
  ]
}
```




