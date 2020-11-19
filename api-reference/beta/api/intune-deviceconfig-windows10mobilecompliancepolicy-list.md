---
title: Listar windows10MobileCompliancePolicies
description: Listar propriedades e relações dos objetos windows10MobileCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6b938a7e4f1d5ce28a4a29aebc7a8f1f9f1baf9a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49205262"
---
# <a name="list-windows10mobilecompliancepolicies"></a><span data-ttu-id="0f77a-103">Listar windows10MobileCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="0f77a-103">List windows10MobileCompliancePolicies</span></span>

<span data-ttu-id="0f77a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f77a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f77a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0f77a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f77a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0f77a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f77a-107">Listar propriedades e relações dos objetos [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0f77a-107">List properties and relationships of the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f77a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0f77a-108">Prerequisites</span></span>
<span data-ttu-id="0f77a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f77a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f77a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f77a-111">Permission type</span></span>|<span data-ttu-id="0f77a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0f77a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f77a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f77a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0f77a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f77a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0f77a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f77a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f77a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f77a-116">Not supported.</span></span>|
|<span data-ttu-id="0f77a-117">Application</span><span class="sxs-lookup"><span data-stu-id="0f77a-117">Application</span></span>|<span data-ttu-id="0f77a-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f77a-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f77a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f77a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="0f77a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f77a-120">Request headers</span></span>
|<span data-ttu-id="0f77a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0f77a-121">Header</span></span>|<span data-ttu-id="0f77a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0f77a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f77a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f77a-123">Authorization</span></span>|<span data-ttu-id="0f77a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f77a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f77a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0f77a-125">Accept</span></span>|<span data-ttu-id="0f77a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f77a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f77a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f77a-127">Request body</span></span>
<span data-ttu-id="0f77a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0f77a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f77a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f77a-129">Response</span></span>
<span data-ttu-id="0f77a-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f77a-130">If successful, this method returns a `200 OK` response code and a collection of [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f77a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f77a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f77a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f77a-132">Request</span></span>
<span data-ttu-id="0f77a-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f77a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="0f77a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f77a-134">Response</span></span>
<span data-ttu-id="0f77a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f77a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1503

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "3d4237b0-37b0-3d42-b037-423db037423d",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordBlockSimple": true,
      "passwordMinimumLength": 5,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "passwordPreviousPasswordBlockCount": 2,
      "passwordExpirationDays": 6,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordRequireToUnlockFromIdle": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "earlyLaunchAntiMalwareDriverEnabled": true,
      "bitLockerEnabled": true,
      "secureBootEnabled": true,
      "codeIntegrityEnabled": true,
      "storageRequireEncryption": true,
      "activeFirewallRequired": true,
      "validOperatingSystemBuildRanges": [
        {
          "@odata.type": "microsoft.graph.operatingSystemVersionRange",
          "description": "Description value",
          "lowestVersion": "Lowest Version value",
          "highestVersion": "Highest Version value"
        }
      ]
    }
  ]
}
```




