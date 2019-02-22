---
title: Listar windows10MobileCompliancePolicies
description: Listar propriedades e relações dos objetos windows10MobileCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6911228f0b3e8ca72085ef1afbf8a9e09318ad40
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147443"
---
# <a name="list-windows10mobilecompliancepolicies"></a><span data-ttu-id="9430e-103">Listar windows10MobileCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="9430e-103">List windows10MobileCompliancePolicies</span></span>

> <span data-ttu-id="9430e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9430e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9430e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9430e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9430e-106">Listar propriedades e relações dos objetos [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9430e-106">List properties and relationships of the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9430e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9430e-107">Prerequisites</span></span>
<span data-ttu-id="9430e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9430e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9430e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9430e-110">Permission type</span></span>|<span data-ttu-id="9430e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9430e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9430e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9430e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9430e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9430e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9430e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9430e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9430e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9430e-115">Not supported.</span></span>|
|<span data-ttu-id="9430e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9430e-116">Application</span></span>|<span data-ttu-id="9430e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9430e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9430e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9430e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="9430e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9430e-119">Request headers</span></span>
|<span data-ttu-id="9430e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9430e-120">Header</span></span>|<span data-ttu-id="9430e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9430e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9430e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9430e-122">Authorization</span></span>|<span data-ttu-id="9430e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9430e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9430e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9430e-124">Accept</span></span>|<span data-ttu-id="9430e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9430e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9430e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9430e-126">Request body</span></span>
<span data-ttu-id="9430e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9430e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9430e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9430e-128">Response</span></span>
<span data-ttu-id="9430e-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9430e-129">If successful, this method returns a `200 OK` response code and a collection of [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9430e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9430e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9430e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9430e-131">Request</span></span>
<span data-ttu-id="9430e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9430e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="9430e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9430e-133">Response</span></span>
<span data-ttu-id="9430e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9430e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




