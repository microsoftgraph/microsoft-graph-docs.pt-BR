---
title: Acessar iosCompliancePolicy
description: Leia as propriedades e as relações do objeto iosCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ccb4ee75266e85f5089b17ec8670572cbfe3cfc5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467579"
---
# <a name="get-ioscompliancepolicy"></a><span data-ttu-id="fbf03-103">Acessar iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="fbf03-103">Get iosCompliancePolicy</span></span>

> <span data-ttu-id="fbf03-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fbf03-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbf03-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fbf03-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbf03-106">Leia as propriedades e as relações do objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fbf03-106">Read properties and relationships of the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbf03-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fbf03-107">Prerequisites</span></span>
<span data-ttu-id="fbf03-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbf03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbf03-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fbf03-110">Permission type</span></span>|<span data-ttu-id="fbf03-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fbf03-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbf03-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fbf03-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fbf03-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbf03-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fbf03-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fbf03-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbf03-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbf03-115">Not supported.</span></span>|
|<span data-ttu-id="fbf03-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fbf03-116">Application</span></span>|<span data-ttu-id="fbf03-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbf03-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbf03-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fbf03-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fbf03-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fbf03-119">Optional query parameters</span></span>
<span data-ttu-id="fbf03-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fbf03-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fbf03-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fbf03-121">Request headers</span></span>
|<span data-ttu-id="fbf03-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fbf03-122">Header</span></span>|<span data-ttu-id="fbf03-123">Valor</span><span class="sxs-lookup"><span data-stu-id="fbf03-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbf03-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fbf03-124">Authorization</span></span>|<span data-ttu-id="fbf03-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbf03-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbf03-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fbf03-126">Accept</span></span>|<span data-ttu-id="fbf03-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fbf03-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbf03-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fbf03-128">Request body</span></span>
<span data-ttu-id="fbf03-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fbf03-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbf03-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbf03-130">Response</span></span>
<span data-ttu-id="fbf03-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fbf03-131">If successful, this method returns a `200 OK` response code and [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbf03-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fbf03-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbf03-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbf03-133">Request</span></span>
<span data-ttu-id="fbf03-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fbf03-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="fbf03-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbf03-135">Response</span></span>
<span data-ttu-id="fbf03-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fbf03-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1504

{
  "value": {
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
}
```





