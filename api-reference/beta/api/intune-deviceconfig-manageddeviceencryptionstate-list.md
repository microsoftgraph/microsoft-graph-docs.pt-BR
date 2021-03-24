---
title: Listar managedDeviceEncryptionStates
description: Listar propriedades e relações dos objetos managedDeviceEncryptionState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0592b74ffd1869a86e610b08c47a833a1f96f699
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147508"
---
# <a name="list-manageddeviceencryptionstates"></a><span data-ttu-id="72cfb-103">Listar managedDeviceEncryptionStates</span><span class="sxs-lookup"><span data-stu-id="72cfb-103">List managedDeviceEncryptionStates</span></span>

<span data-ttu-id="72cfb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72cfb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72cfb-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="72cfb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72cfb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="72cfb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72cfb-107">Listar propriedades e relações dos [objetos managedDeviceEncryptionState.](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)</span><span class="sxs-lookup"><span data-stu-id="72cfb-107">List properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72cfb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="72cfb-108">Prerequisites</span></span>
<span data-ttu-id="72cfb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72cfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72cfb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72cfb-111">Permission type</span></span>|<span data-ttu-id="72cfb-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="72cfb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72cfb-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72cfb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="72cfb-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72cfb-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="72cfb-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72cfb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72cfb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72cfb-116">Not supported.</span></span>|
|<span data-ttu-id="72cfb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72cfb-117">Application</span></span>|<span data-ttu-id="72cfb-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72cfb-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="72cfb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72cfb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceEncryptionStates
```

## <a name="request-headers"></a><span data-ttu-id="72cfb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72cfb-120">Request headers</span></span>
|<span data-ttu-id="72cfb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="72cfb-121">Header</span></span>|<span data-ttu-id="72cfb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="72cfb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72cfb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="72cfb-123">Authorization</span></span>|<span data-ttu-id="72cfb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72cfb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72cfb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="72cfb-125">Accept</span></span>|<span data-ttu-id="72cfb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="72cfb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72cfb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72cfb-127">Request body</span></span>
<span data-ttu-id="72cfb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="72cfb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72cfb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="72cfb-129">Response</span></span>
<span data-ttu-id="72cfb-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72cfb-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72cfb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72cfb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="72cfb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72cfb-132">Request</span></span>
<span data-ttu-id="72cfb-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72cfb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates
```

### <a name="response"></a><span data-ttu-id="72cfb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="72cfb-134">Response</span></span>
<span data-ttu-id="72cfb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72cfb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




