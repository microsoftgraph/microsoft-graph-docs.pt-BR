---
title: Listar iosCompliancePolicies
description: Listar propriedades e relações dos objetos iosCompliancePolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3aab9f8b0767a8e30676990b05451d747b3936f6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394051"
---
# <a name="list-ioscompliancepolicies"></a><span data-ttu-id="a9eb2-103">Listar iosCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="a9eb2-103">List iosCompliancePolicies</span></span>

> <span data-ttu-id="a9eb2-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="a9eb2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a9eb2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a9eb2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a9eb2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="a9eb2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9eb2-107">Listar propriedades e relações dos objetos [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a9eb2-107">List properties and relationships of the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9eb2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a9eb2-108">Prerequisites</span></span>
<span data-ttu-id="a9eb2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a9eb2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a9eb2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9eb2-111">Permission type</span></span>|<span data-ttu-id="a9eb2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a9eb2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9eb2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9eb2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9eb2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9eb2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a9eb2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9eb2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9eb2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9eb2-116">Not supported.</span></span>|
|<span data-ttu-id="a9eb2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9eb2-117">Application</span></span>|<span data-ttu-id="a9eb2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9eb2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9eb2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9eb2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="a9eb2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9eb2-120">Request headers</span></span>
|<span data-ttu-id="a9eb2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a9eb2-121">Header</span></span>|<span data-ttu-id="a9eb2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a9eb2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9eb2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9eb2-123">Authorization</span></span>|<span data-ttu-id="a9eb2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9eb2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9eb2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a9eb2-125">Accept</span></span>|<span data-ttu-id="a9eb2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9eb2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9eb2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9eb2-127">Request body</span></span>
<span data-ttu-id="a9eb2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a9eb2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9eb2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9eb2-129">Response</span></span>
<span data-ttu-id="a9eb2-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9eb2-130">If successful, this method returns a `200 OK` response code and a collection of [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9eb2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9eb2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9eb2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9eb2-132">Request</span></span>
<span data-ttu-id="a9eb2-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9eb2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="a9eb2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9eb2-134">Response</span></span>
<span data-ttu-id="a9eb2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9eb2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




