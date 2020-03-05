---
title: Listar iosCompliancePolicies
description: Listar propriedades e relações dos objetos iosCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 14bb57bd9b0e78d717d6b8b4f365ce229f5065ee
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442912"
---
# <a name="list-ioscompliancepolicies"></a><span data-ttu-id="d3f1c-103">Listar iosCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="d3f1c-103">List iosCompliancePolicies</span></span>

<span data-ttu-id="d3f1c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d3f1c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3f1c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d3f1c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3f1c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d3f1c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3f1c-107">Listar propriedades e relações dos objetos [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d3f1c-107">List properties and relationships of the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3f1c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d3f1c-108">Prerequisites</span></span>
<span data-ttu-id="d3f1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3f1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3f1c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3f1c-111">Permission type</span></span>|<span data-ttu-id="d3f1c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d3f1c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3f1c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3f1c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3f1c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3f1c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d3f1c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3f1c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3f1c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3f1c-116">Not supported.</span></span>|
|<span data-ttu-id="d3f1c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3f1c-117">Application</span></span>|<span data-ttu-id="d3f1c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3f1c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3f1c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3f1c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="d3f1c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3f1c-120">Request headers</span></span>
|<span data-ttu-id="d3f1c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3f1c-121">Header</span></span>|<span data-ttu-id="d3f1c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d3f1c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3f1c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3f1c-123">Authorization</span></span>|<span data-ttu-id="d3f1c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3f1c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3f1c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d3f1c-125">Accept</span></span>|<span data-ttu-id="d3f1c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3f1c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3f1c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3f1c-127">Request body</span></span>
<span data-ttu-id="d3f1c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d3f1c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3f1c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3f1c-129">Response</span></span>
<span data-ttu-id="d3f1c-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3f1c-130">If successful, this method returns a `200 OK` response code and a collection of [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3f1c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3f1c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3f1c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3f1c-132">Request</span></span>
<span data-ttu-id="d3f1c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3f1c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="d3f1c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3f1c-134">Response</span></span>
<span data-ttu-id="d3f1c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3f1c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





