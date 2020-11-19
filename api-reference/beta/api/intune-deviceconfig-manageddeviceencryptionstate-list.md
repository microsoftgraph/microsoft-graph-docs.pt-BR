---
title: Listar managedDeviceEncryptionStates
description: Listar Propriedades e relações dos objetos managedDeviceEncryptionState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2ea7504925ec87c494cd9068dc7dca080108c5b0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49287148"
---
# <a name="list-manageddeviceencryptionstates"></a><span data-ttu-id="15887-103">Listar managedDeviceEncryptionStates</span><span class="sxs-lookup"><span data-stu-id="15887-103">List managedDeviceEncryptionStates</span></span>

<span data-ttu-id="15887-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15887-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15887-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="15887-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15887-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="15887-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15887-107">Listar Propriedades e relações dos objetos [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="15887-107">List properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15887-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="15887-108">Prerequisites</span></span>
<span data-ttu-id="15887-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15887-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15887-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15887-111">Permission type</span></span>|<span data-ttu-id="15887-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="15887-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15887-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15887-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15887-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="15887-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="15887-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15887-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15887-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15887-116">Not supported.</span></span>|
|<span data-ttu-id="15887-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15887-117">Application</span></span>|<span data-ttu-id="15887-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="15887-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="15887-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15887-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceEncryptionStates
```

## <a name="request-headers"></a><span data-ttu-id="15887-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15887-120">Request headers</span></span>
|<span data-ttu-id="15887-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="15887-121">Header</span></span>|<span data-ttu-id="15887-122">Valor</span><span class="sxs-lookup"><span data-stu-id="15887-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15887-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="15887-123">Authorization</span></span>|<span data-ttu-id="15887-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15887-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15887-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="15887-125">Accept</span></span>|<span data-ttu-id="15887-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15887-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15887-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15887-127">Request body</span></span>
<span data-ttu-id="15887-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="15887-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15887-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="15887-129">Response</span></span>
<span data-ttu-id="15887-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15887-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15887-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15887-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="15887-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15887-132">Request</span></span>
<span data-ttu-id="15887-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15887-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates
```

### <a name="response"></a><span data-ttu-id="15887-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="15887-134">Response</span></span>
<span data-ttu-id="15887-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15887-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 862

{
  "value": [
    {
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
  ]
}
```




