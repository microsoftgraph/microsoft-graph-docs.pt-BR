---
title: Listar windowsAutopilotDeviceIdentities
description: Listar propriedades e relações dos objetos windowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 76433afb73b62b80df51e6c4962256d965b3babd
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752857"
---
# <a name="list-windowsautopilotdeviceidentities"></a><span data-ttu-id="5d852-103">Listar windowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="5d852-103">List windowsAutopilotDeviceIdentities</span></span>

<span data-ttu-id="5d852-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d852-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5d852-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5d852-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d852-106">Listar propriedades e relações dos [objetos windowsAutopilotDeviceIdentity.](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="5d852-106">List properties and relationships of the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d852-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5d852-107">Prerequisites</span></span>
<span data-ttu-id="5d852-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d852-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d852-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d852-110">Permission type</span></span>|<span data-ttu-id="5d852-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d852-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d852-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d852-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5d852-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d852-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5d852-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d852-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d852-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d852-115">Not supported.</span></span>|
|<span data-ttu-id="5d852-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d852-116">Application</span></span>|<span data-ttu-id="5d852-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d852-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d852-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d852-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="5d852-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d852-119">Request headers</span></span>
|<span data-ttu-id="5d852-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5d852-120">Header</span></span>|<span data-ttu-id="5d852-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5d852-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d852-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d852-122">Authorization</span></span>|<span data-ttu-id="5d852-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d852-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d852-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5d852-124">Accept</span></span>|<span data-ttu-id="5d852-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5d852-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d852-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d852-126">Request body</span></span>
<span data-ttu-id="5d852-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5d852-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d852-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d852-128">Response</span></span>
<span data-ttu-id="5d852-129">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d852-129">If successful, this method returns a `200 OK` response code and a collection of [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d852-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d852-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d852-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d852-131">Request</span></span>
<span data-ttu-id="5d852-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d852-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="5d852-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d852-133">Response</span></span>
<span data-ttu-id="5d852-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5d852-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 968

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
      "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
      "groupTag": "Group Tag value",
      "purchaseOrderIdentifier": "Purchase Order Identifier value",
      "serialNumber": "Serial Number value",
      "productKey": "Product Key value",
      "manufacturer": "Manufacturer value",
      "model": "Model value",
      "enrollmentState": "enrolled",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "addressableUserName": "Addressable User Name value",
      "userPrincipalName": "User Principal Name value",
      "resourceName": "Resource Name value",
      "skuNumber": "Sku Number value",
      "systemFamily": "System Family value",
      "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
      "managedDeviceId": "Managed Device Id value",
      "displayName": "Display Name value"
    }
  ]
}
```




