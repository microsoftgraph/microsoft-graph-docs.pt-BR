---
title: Listar deviceManagementScripts
description: Listar Propriedades e relações dos objetos deviceManagementScript.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b34029884f250208b80bdb2d887b1ed0ac5d80cc
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800953"
---
# <a name="list-devicemanagementscripts"></a><span data-ttu-id="b4d02-103">Listar deviceManagementScripts</span><span class="sxs-lookup"><span data-stu-id="b4d02-103">List deviceManagementScripts</span></span>

> <span data-ttu-id="b4d02-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b4d02-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4d02-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b4d02-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4d02-106">Listar Propriedades e relações dos objetos [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="b4d02-106">List properties and relationships of the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4d02-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b4d02-107">Prerequisites</span></span>
<span data-ttu-id="b4d02-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4d02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4d02-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4d02-110">Permission type</span></span>|<span data-ttu-id="b4d02-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b4d02-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4d02-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4d02-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b4d02-113">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="b4d02-113">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="b4d02-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4d02-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="b4d02-115">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="b4d02-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="b4d02-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4d02-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b4d02-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4d02-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4d02-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4d02-118">Not supported.</span></span>|
|<span data-ttu-id="b4d02-119">Application</span><span class="sxs-lookup"><span data-stu-id="b4d02-119">Application</span></span>||
| <span data-ttu-id="b4d02-120">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="b4d02-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="b4d02-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4d02-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="b4d02-122">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="b4d02-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="b4d02-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4d02-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4d02-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4d02-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="b4d02-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4d02-125">Request headers</span></span>
|<span data-ttu-id="b4d02-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b4d02-126">Header</span></span>|<span data-ttu-id="b4d02-127">Valor</span><span class="sxs-lookup"><span data-stu-id="b4d02-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4d02-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4d02-128">Authorization</span></span>|<span data-ttu-id="b4d02-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4d02-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4d02-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b4d02-130">Accept</span></span>|<span data-ttu-id="b4d02-131">application/json</span><span class="sxs-lookup"><span data-stu-id="b4d02-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4d02-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4d02-132">Request body</span></span>
<span data-ttu-id="b4d02-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b4d02-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4d02-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4d02-134">Response</span></span>
<span data-ttu-id="b4d02-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4d02-135">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4d02-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b4d02-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4d02-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4d02-137">Request</span></span>
<span data-ttu-id="b4d02-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4d02-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
```

### <a name="response"></a><span data-ttu-id="b4d02-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4d02-139">Response</span></span>
<span data-ttu-id="b4d02-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b4d02-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







