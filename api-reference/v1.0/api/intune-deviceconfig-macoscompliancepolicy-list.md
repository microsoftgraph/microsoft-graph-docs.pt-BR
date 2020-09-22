---
title: Listar macOSCompliancePolicies
description: Listar propriedades e relações dos objetos macOSCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 409e0ad57744cbf31fc73b4c3621d1045d81c9a1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972907"
---
# <a name="list-macoscompliancepolicies"></a><span data-ttu-id="d7b1a-103">Listar macOSCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="d7b1a-103">List macOSCompliancePolicies</span></span>

<span data-ttu-id="d7b1a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7b1a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7b1a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d7b1a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7b1a-106">Listar propriedades e relações dos objetos [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d7b1a-106">List properties and relationships of the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7b1a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d7b1a-107">Prerequisites</span></span>
<span data-ttu-id="d7b1a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7b1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7b1a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7b1a-110">Permission type</span></span>|<span data-ttu-id="d7b1a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d7b1a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7b1a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7b1a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d7b1a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7b1a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d7b1a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7b1a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7b1a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7b1a-115">Not supported.</span></span>|
|<span data-ttu-id="d7b1a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7b1a-116">Application</span></span>|<span data-ttu-id="d7b1a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7b1a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7b1a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7b1a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="d7b1a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7b1a-119">Request headers</span></span>
|<span data-ttu-id="d7b1a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d7b1a-120">Header</span></span>|<span data-ttu-id="d7b1a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d7b1a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7b1a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7b1a-122">Authorization</span></span>|<span data-ttu-id="d7b1a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7b1a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7b1a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d7b1a-124">Accept</span></span>|<span data-ttu-id="d7b1a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d7b1a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7b1a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7b1a-126">Request body</span></span>
<span data-ttu-id="d7b1a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d7b1a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7b1a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7b1a-128">Response</span></span>
<span data-ttu-id="d7b1a-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7b1a-129">If successful, this method returns a `200 OK` response code and a collection of [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7b1a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7b1a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7b1a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7b1a-131">Request</span></span>
<span data-ttu-id="d7b1a-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7b1a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="d7b1a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7b1a-133">Response</span></span>
<span data-ttu-id="d7b1a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7b1a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









