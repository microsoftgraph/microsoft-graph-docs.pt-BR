---
title: Listar iosCompliancePolicies
description: Listar propriedades e relações dos objetos iosCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6bde7a4054db9e6e04c82939080c6b2307b3c4ec
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261422"
---
# <a name="list-ioscompliancepolicies"></a><span data-ttu-id="aef05-103">Listar iosCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="aef05-103">List iosCompliancePolicies</span></span>

> <span data-ttu-id="aef05-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aef05-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aef05-105">Listar propriedades e relações dos objetos [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="aef05-105">List properties and relationships of the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aef05-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aef05-106">Prerequisites</span></span>
<span data-ttu-id="aef05-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="aef05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="aef05-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aef05-109">Permission type</span></span>|<span data-ttu-id="aef05-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aef05-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aef05-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aef05-111">Delegated (work or school account)</span></span>|<span data-ttu-id="aef05-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="aef05-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="aef05-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aef05-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aef05-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aef05-114">Not supported.</span></span>|
|<span data-ttu-id="aef05-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aef05-115">Application</span></span>|<span data-ttu-id="aef05-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aef05-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aef05-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aef05-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="aef05-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aef05-118">Request headers</span></span>
|<span data-ttu-id="aef05-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aef05-119">Header</span></span>|<span data-ttu-id="aef05-120">Valor</span><span class="sxs-lookup"><span data-stu-id="aef05-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aef05-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="aef05-121">Authorization</span></span>|<span data-ttu-id="aef05-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aef05-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aef05-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aef05-123">Accept</span></span>|<span data-ttu-id="aef05-124">application/json</span><span class="sxs-lookup"><span data-stu-id="aef05-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aef05-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aef05-125">Request body</span></span>
<span data-ttu-id="aef05-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aef05-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aef05-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="aef05-127">Response</span></span>
<span data-ttu-id="aef05-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aef05-128">If successful, this method returns a `200 OK` response code and a collection of [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aef05-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aef05-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="aef05-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aef05-130">Request</span></span>
<span data-ttu-id="aef05-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aef05-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="aef05-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="aef05-132">Response</span></span>
<span data-ttu-id="aef05-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aef05-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



