---
title: Listar iosCompliancePolicies
description: Listar propriedades e relações dos objetos iosCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4557edfe695d5ba00cbb96dd9155e859b36b3438
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753871"
---
# <a name="list-ioscompliancepolicies"></a><span data-ttu-id="7a536-103">Listar iosCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="7a536-103">List iosCompliancePolicies</span></span>

<span data-ttu-id="7a536-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a536-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a536-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7a536-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a536-106">Listar propriedades e relações dos objetos [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7a536-106">List properties and relationships of the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a536-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7a536-107">Prerequisites</span></span>
<span data-ttu-id="7a536-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a536-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a536-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a536-110">Permission type</span></span>|<span data-ttu-id="7a536-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a536-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a536-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a536-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7a536-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a536-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7a536-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a536-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a536-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a536-115">Not supported.</span></span>|
|<span data-ttu-id="7a536-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a536-116">Application</span></span>|<span data-ttu-id="7a536-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a536-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a536-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a536-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="7a536-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a536-119">Request headers</span></span>
|<span data-ttu-id="7a536-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7a536-120">Header</span></span>|<span data-ttu-id="7a536-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7a536-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a536-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a536-122">Authorization</span></span>|<span data-ttu-id="7a536-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a536-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a536-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7a536-124">Accept</span></span>|<span data-ttu-id="7a536-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7a536-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a536-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a536-126">Request body</span></span>
<span data-ttu-id="7a536-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7a536-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a536-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a536-128">Response</span></span>
<span data-ttu-id="7a536-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a536-129">If successful, this method returns a `200 OK` response code and a collection of [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a536-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7a536-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a536-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a536-131">Request</span></span>
<span data-ttu-id="7a536-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a536-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="7a536-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a536-133">Response</span></span>
<span data-ttu-id="7a536-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7a536-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1034

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosCompliancePolicy",
      "id": "4f501351-1351-4f50-5113-504f5113504f",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passcodeBlockSimple": true,
      "passcodeExpirationDays": 6,
      "passcodeMinimumLength": 5,
      "passcodeMinutesOfInactivityBeforeLock": 5,
      "passcodePreviousPasscodeBlockCount": 2,
      "passcodeMinimumCharacterSetCount": 0,
      "passcodeRequiredType": "alphanumeric",
      "passcodeRequired": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "securityBlockJailbrokenDevices": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "managedEmailProfileRequired": true
    }
  ]
}
```




