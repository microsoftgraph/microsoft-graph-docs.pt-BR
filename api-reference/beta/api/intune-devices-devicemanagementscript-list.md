---
title: Listar deviceManagementScripts
description: Listar Propriedades e relações dos objetos deviceManagementScript.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8520ca1788b4628be80f5bd4c7f2cd464e889e04
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33909978"
---
# <a name="list-devicemanagementscripts"></a><span data-ttu-id="d8f44-103">Listar deviceManagementScripts</span><span class="sxs-lookup"><span data-stu-id="d8f44-103">List deviceManagementScripts</span></span>

> <span data-ttu-id="d8f44-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d8f44-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8f44-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d8f44-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8f44-106">Listar Propriedades e relações dos objetos [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="d8f44-106">List properties and relationships of the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8f44-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d8f44-107">Prerequisites</span></span>
<span data-ttu-id="d8f44-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8f44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8f44-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8f44-110">Permission type</span></span>|<span data-ttu-id="d8f44-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d8f44-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8f44-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8f44-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d8f44-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8f44-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d8f44-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8f44-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8f44-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8f44-115">Not supported.</span></span>|
|<span data-ttu-id="d8f44-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8f44-116">Application</span></span>|<span data-ttu-id="d8f44-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8f44-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8f44-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8f44-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="d8f44-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8f44-119">Request headers</span></span>
|<span data-ttu-id="d8f44-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d8f44-120">Header</span></span>|<span data-ttu-id="d8f44-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d8f44-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8f44-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8f44-122">Authorization</span></span>|<span data-ttu-id="d8f44-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8f44-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8f44-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d8f44-124">Accept</span></span>|<span data-ttu-id="d8f44-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d8f44-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8f44-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8f44-126">Request body</span></span>
<span data-ttu-id="d8f44-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d8f44-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8f44-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8f44-128">Response</span></span>
<span data-ttu-id="d8f44-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8f44-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8f44-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8f44-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8f44-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8f44-131">Request</span></span>
<span data-ttu-id="d8f44-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8f44-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
```

### <a name="response"></a><span data-ttu-id="d8f44-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8f44-133">Response</span></span>
<span data-ttu-id="d8f44-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8f44-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




