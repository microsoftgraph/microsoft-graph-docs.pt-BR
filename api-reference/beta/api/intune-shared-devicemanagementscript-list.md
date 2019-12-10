---
title: Listar deviceManagementScripts
description: Listar Propriedades e relações dos objetos deviceManagementScript.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1b0fe4c28e759e5490f2bf154b55877e06a41240
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939876"
---
# <a name="list-devicemanagementscripts"></a><span data-ttu-id="eea5b-103">Listar deviceManagementScripts</span><span class="sxs-lookup"><span data-stu-id="eea5b-103">List deviceManagementScripts</span></span>

> <span data-ttu-id="eea5b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eea5b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eea5b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eea5b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eea5b-106">Listar Propriedades e relações dos objetos [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="eea5b-106">List properties and relationships of the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eea5b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eea5b-107">Prerequisites</span></span>
<span data-ttu-id="eea5b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eea5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eea5b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eea5b-110">Permission type</span></span>|<span data-ttu-id="eea5b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eea5b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eea5b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eea5b-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="eea5b-113">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="eea5b-113">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="eea5b-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="eea5b-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="eea5b-115">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="eea5b-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="eea5b-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="eea5b-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="eea5b-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eea5b-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eea5b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eea5b-118">Not supported.</span></span>|
|<span data-ttu-id="eea5b-119">Application</span><span class="sxs-lookup"><span data-stu-id="eea5b-119">Application</span></span>||
| <span data-ttu-id="eea5b-120">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="eea5b-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="eea5b-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="eea5b-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="eea5b-122">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="eea5b-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="eea5b-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="eea5b-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eea5b-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eea5b-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="eea5b-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eea5b-125">Request headers</span></span>
|<span data-ttu-id="eea5b-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eea5b-126">Header</span></span>|<span data-ttu-id="eea5b-127">Valor</span><span class="sxs-lookup"><span data-stu-id="eea5b-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eea5b-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="eea5b-128">Authorization</span></span>|<span data-ttu-id="eea5b-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eea5b-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eea5b-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eea5b-130">Accept</span></span>|<span data-ttu-id="eea5b-131">application/json</span><span class="sxs-lookup"><span data-stu-id="eea5b-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eea5b-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eea5b-132">Request body</span></span>
<span data-ttu-id="eea5b-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eea5b-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eea5b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="eea5b-134">Response</span></span>
<span data-ttu-id="eea5b-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eea5b-135">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eea5b-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eea5b-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="eea5b-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eea5b-137">Request</span></span>
<span data-ttu-id="eea5b-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eea5b-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
```

### <a name="response"></a><span data-ttu-id="eea5b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="eea5b-139">Response</span></span>
<span data-ttu-id="eea5b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eea5b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 716

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScript",
      "id": "59ea4525-4525-59ea-2545-ea592545ea59",
      "displayName": "Display Name value",
      "description": "Description value",
      "runSchedule": {
        "@odata.type": "microsoft.graph.runSchedule"
      },
      "scriptContent": "c2NyaXB0Q29udGVudA==",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "runAsAccount": "user",
      "enforceSignatureCheck": true,
      "fileName": "File Name value",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "runAs32Bit": true
    }
  ]
}
```








