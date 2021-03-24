---
title: Get windows10MobileCompliancePolicy
description: Ler propriedades e relações do objeto windows10MobileCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f0f27ccbbcd36dd98a9b319c14e46e9020c046ee
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127697"
---
# <a name="get-windows10mobilecompliancepolicy"></a><span data-ttu-id="03c28-103">Get windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="03c28-103">Get windows10MobileCompliancePolicy</span></span>

<span data-ttu-id="03c28-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03c28-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03c28-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="03c28-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03c28-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="03c28-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03c28-107">Ler propriedades e relações do objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="03c28-107">Read properties and relationships of the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03c28-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="03c28-108">Prerequisites</span></span>
<span data-ttu-id="03c28-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03c28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03c28-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03c28-111">Permission type</span></span>|<span data-ttu-id="03c28-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="03c28-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03c28-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03c28-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03c28-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03c28-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="03c28-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03c28-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03c28-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03c28-116">Not supported.</span></span>|
|<span data-ttu-id="03c28-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03c28-117">Application</span></span>|<span data-ttu-id="03c28-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03c28-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03c28-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03c28-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="03c28-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="03c28-120">Optional query parameters</span></span>
<span data-ttu-id="03c28-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="03c28-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="03c28-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03c28-122">Request headers</span></span>
|<span data-ttu-id="03c28-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="03c28-123">Header</span></span>|<span data-ttu-id="03c28-124">Valor</span><span class="sxs-lookup"><span data-stu-id="03c28-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03c28-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="03c28-125">Authorization</span></span>|<span data-ttu-id="03c28-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03c28-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03c28-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="03c28-127">Accept</span></span>|<span data-ttu-id="03c28-128">application/json</span><span class="sxs-lookup"><span data-stu-id="03c28-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03c28-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03c28-129">Request body</span></span>
<span data-ttu-id="03c28-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="03c28-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03c28-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="03c28-131">Response</span></span>
<span data-ttu-id="03c28-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03c28-132">If successful, this method returns a `200 OK` response code and [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03c28-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03c28-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="03c28-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03c28-134">Request</span></span>
<span data-ttu-id="03c28-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="03c28-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="03c28-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="03c28-136">Response</span></span>
<span data-ttu-id="03c28-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="03c28-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1419

{
  "value": {
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
}
```




