---
title: Obter managedDeviceEncryptionState
description: Leia as propriedades e as relações do objeto managedDeviceEncryptionState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: efc57de0c8913f74698b6a847bb557a14a6ad2c8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024875"
---
# <a name="get-manageddeviceencryptionstate"></a><span data-ttu-id="c7814-103">Obter managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="c7814-103">Get managedDeviceEncryptionState</span></span>

<span data-ttu-id="c7814-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7814-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7814-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c7814-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7814-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c7814-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7814-107">Leia as propriedades e as relações do objeto [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="c7814-107">Read properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7814-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c7814-108">Prerequisites</span></span>
<span data-ttu-id="c7814-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7814-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7814-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7814-111">Permission type</span></span>|<span data-ttu-id="c7814-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c7814-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7814-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7814-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7814-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7814-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c7814-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7814-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7814-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7814-116">Not supported.</span></span>|
|<span data-ttu-id="c7814-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7814-117">Application</span></span>|<span data-ttu-id="c7814-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7814-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7814-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7814-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7814-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c7814-120">Optional query parameters</span></span>
<span data-ttu-id="c7814-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c7814-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7814-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7814-122">Request headers</span></span>
|<span data-ttu-id="c7814-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7814-123">Header</span></span>|<span data-ttu-id="c7814-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c7814-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7814-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7814-125">Authorization</span></span>|<span data-ttu-id="c7814-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7814-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7814-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c7814-127">Accept</span></span>|<span data-ttu-id="c7814-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c7814-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7814-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7814-129">Request body</span></span>
<span data-ttu-id="c7814-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c7814-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7814-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7814-131">Response</span></span>
<span data-ttu-id="c7814-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7814-132">If successful, this method returns a `200 OK` response code and [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7814-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7814-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7814-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7814-134">Request</span></span>
<span data-ttu-id="c7814-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7814-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
```

### <a name="response"></a><span data-ttu-id="c7814-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7814-136">Response</span></span>
<span data-ttu-id="c7814-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7814-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






