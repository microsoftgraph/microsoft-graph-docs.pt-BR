---
title: Listar iosCompliancePolicies
description: Listar propriedades e relações dos objetos iosCompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 648848e4268d034eacb8e290587bf9b83828c441
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42752489"
---
# <a name="list-ioscompliancepolicies"></a><span data-ttu-id="4ed30-103">Listar iosCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="4ed30-103">List iosCompliancePolicies</span></span>

> <span data-ttu-id="4ed30-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4ed30-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ed30-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4ed30-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ed30-106">Listar propriedades e relações dos objetos [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4ed30-106">List properties and relationships of the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ed30-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4ed30-107">Prerequisites</span></span>
<span data-ttu-id="4ed30-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ed30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ed30-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ed30-110">Permission type</span></span>|<span data-ttu-id="4ed30-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4ed30-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ed30-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ed30-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4ed30-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ed30-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4ed30-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ed30-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ed30-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ed30-115">Not supported.</span></span>|
|<span data-ttu-id="4ed30-116">Application</span><span class="sxs-lookup"><span data-stu-id="4ed30-116">Application</span></span>|<span data-ttu-id="4ed30-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ed30-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ed30-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ed30-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="4ed30-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ed30-119">Request headers</span></span>
|<span data-ttu-id="4ed30-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4ed30-120">Header</span></span>|<span data-ttu-id="4ed30-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4ed30-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ed30-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ed30-122">Authorization</span></span>|<span data-ttu-id="4ed30-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ed30-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ed30-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4ed30-124">Accept</span></span>|<span data-ttu-id="4ed30-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4ed30-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ed30-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ed30-126">Request body</span></span>
<span data-ttu-id="4ed30-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4ed30-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ed30-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ed30-128">Response</span></span>
<span data-ttu-id="4ed30-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ed30-129">If successful, this method returns a `200 OK` response code and a collection of [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ed30-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ed30-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ed30-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ed30-131">Request</span></span>
<span data-ttu-id="4ed30-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ed30-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="4ed30-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ed30-133">Response</span></span>
<span data-ttu-id="4ed30-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ed30-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1590

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
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
      "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
      "passcodePreviousPasscodeBlockCount": 2,
      "passcodeMinimumCharacterSetCount": 0,
      "passcodeRequiredType": "alphanumeric",
      "passcodeRequired": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "osMinimumBuildVersion": "Os Minimum Build Version value",
      "osMaximumBuildVersion": "Os Maximum Build Version value",
      "securityBlockJailbrokenDevices": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "managedEmailProfileRequired": true,
      "restrictedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ]
    }
  ]
}
```




