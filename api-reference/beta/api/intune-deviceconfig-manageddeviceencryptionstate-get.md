---
title: Obter managedDeviceEncryptionState
description: Leia as propriedades e as relações do objeto managedDeviceEncryptionState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a181f6303891e2a88cb73a5e24bee70149ae6589
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448582"
---
# <a name="get-manageddeviceencryptionstate"></a><span data-ttu-id="c77db-103">Obter managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="c77db-103">Get managedDeviceEncryptionState</span></span>

<span data-ttu-id="c77db-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c77db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c77db-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c77db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c77db-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c77db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c77db-107">Leia as propriedades e as relações do objeto [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="c77db-107">Read properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c77db-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c77db-108">Prerequisites</span></span>
<span data-ttu-id="c77db-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c77db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c77db-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c77db-111">Permission type</span></span>|<span data-ttu-id="c77db-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c77db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c77db-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c77db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c77db-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c77db-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c77db-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c77db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c77db-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c77db-116">Not supported.</span></span>|
|<span data-ttu-id="c77db-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c77db-117">Application</span></span>|<span data-ttu-id="c77db-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c77db-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c77db-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c77db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c77db-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c77db-120">Optional query parameters</span></span>
<span data-ttu-id="c77db-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c77db-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c77db-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c77db-122">Request headers</span></span>
|<span data-ttu-id="c77db-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c77db-123">Header</span></span>|<span data-ttu-id="c77db-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c77db-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c77db-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c77db-125">Authorization</span></span>|<span data-ttu-id="c77db-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c77db-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c77db-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c77db-127">Accept</span></span>|<span data-ttu-id="c77db-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c77db-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c77db-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c77db-129">Request body</span></span>
<span data-ttu-id="c77db-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c77db-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c77db-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c77db-131">Response</span></span>
<span data-ttu-id="c77db-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c77db-132">If successful, this method returns a `200 OK` response code and [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c77db-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c77db-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c77db-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c77db-134">Request</span></span>
<span data-ttu-id="c77db-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c77db-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
```

### <a name="response"></a><span data-ttu-id="c77db-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c77db-136">Response</span></span>
<span data-ttu-id="c77db-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c77db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





