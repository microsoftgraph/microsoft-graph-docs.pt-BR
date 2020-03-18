---
title: Obter managedDeviceEncryptionState
description: Leia as propriedades e as relações do objeto managedDeviceEncryptionState.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 44ad1e6d61ae4cb7d355f8c1f67381a5a9977c94
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42743048"
---
# <a name="get-manageddeviceencryptionstate"></a><span data-ttu-id="9ab97-103">Obter managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="9ab97-103">Get managedDeviceEncryptionState</span></span>

> <span data-ttu-id="9ab97-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9ab97-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ab97-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9ab97-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ab97-106">Leia as propriedades e as relações do objeto [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="9ab97-106">Read properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ab97-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9ab97-107">Prerequisites</span></span>
<span data-ttu-id="9ab97-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ab97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ab97-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ab97-110">Permission type</span></span>|<span data-ttu-id="9ab97-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9ab97-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ab97-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ab97-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9ab97-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9ab97-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9ab97-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ab97-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ab97-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ab97-115">Not supported.</span></span>|
|<span data-ttu-id="9ab97-116">Application</span><span class="sxs-lookup"><span data-stu-id="9ab97-116">Application</span></span>|<span data-ttu-id="9ab97-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9ab97-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ab97-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ab97-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9ab97-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9ab97-119">Optional query parameters</span></span>
<span data-ttu-id="9ab97-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9ab97-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ab97-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ab97-121">Request headers</span></span>
|<span data-ttu-id="9ab97-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9ab97-122">Header</span></span>|<span data-ttu-id="9ab97-123">Valor</span><span class="sxs-lookup"><span data-stu-id="9ab97-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ab97-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ab97-124">Authorization</span></span>|<span data-ttu-id="9ab97-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ab97-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ab97-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9ab97-126">Accept</span></span>|<span data-ttu-id="9ab97-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9ab97-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ab97-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ab97-128">Request body</span></span>
<span data-ttu-id="9ab97-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9ab97-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ab97-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ab97-130">Response</span></span>
<span data-ttu-id="9ab97-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ab97-131">If successful, this method returns a `200 OK` response code and [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ab97-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ab97-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ab97-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ab97-133">Request</span></span>
<span data-ttu-id="9ab97-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ab97-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
```

### <a name="response"></a><span data-ttu-id="9ab97-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ab97-135">Response</span></span>
<span data-ttu-id="9ab97-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ab97-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 810

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
    "id": "f09b4ab6-4ab6-f09b-b64a-9bf0b64a9bf0",
    "userPrincipalName": "User Principal Name value",
    "deviceType": "windowsRT",
    "osVersion": "Os Version value",
    "tpmSpecificationVersion": "Tpm Specification Version value",
    "deviceName": "Device Name value",
    "encryptionReadinessState": "ready",
    "encryptionState": "encrypted",
    "encryptionPolicySettingState": "notApplicable",
    "advancedBitLockerStates": "noUserConsent",
    "fileVaultStates": "driveEncryptedByUser",
    "policyDetails": [
      {
        "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
        "policyId": "Policy Id value",
        "policyName": "Policy Name value"
      }
    ]
  }
}
```




