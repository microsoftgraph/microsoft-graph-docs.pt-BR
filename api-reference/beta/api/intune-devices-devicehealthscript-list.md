---
title: Listar deviceHealthScripts
description: Listar Propriedades e relações dos objetos deviceHealthScript.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9c9e7699f4cf1d681e71c9df63625ff4ec88d1d3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42814600"
---
# <a name="list-devicehealthscripts"></a><span data-ttu-id="cf565-103">Listar deviceHealthScripts</span><span class="sxs-lookup"><span data-stu-id="cf565-103">List deviceHealthScripts</span></span>

> <span data-ttu-id="cf565-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cf565-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf565-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cf565-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf565-106">Listar Propriedades e relações dos objetos [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="cf565-106">List properties and relationships of the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf565-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cf565-107">Prerequisites</span></span>
<span data-ttu-id="cf565-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf565-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf565-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf565-110">Permission type</span></span>|<span data-ttu-id="cf565-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cf565-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf565-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf565-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cf565-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf565-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cf565-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf565-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf565-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf565-115">Not supported.</span></span>|
|<span data-ttu-id="cf565-116">Application</span><span class="sxs-lookup"><span data-stu-id="cf565-116">Application</span></span>|<span data-ttu-id="cf565-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf565-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf565-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf565-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts
```

## <a name="request-headers"></a><span data-ttu-id="cf565-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf565-119">Request headers</span></span>
|<span data-ttu-id="cf565-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf565-120">Header</span></span>|<span data-ttu-id="cf565-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cf565-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf565-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf565-122">Authorization</span></span>|<span data-ttu-id="cf565-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf565-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf565-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cf565-124">Accept</span></span>|<span data-ttu-id="cf565-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cf565-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf565-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf565-126">Request body</span></span>
<span data-ttu-id="cf565-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cf565-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf565-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf565-128">Response</span></span>
<span data-ttu-id="cf565-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf565-129">If successful, this method returns a `200 OK` response code and a collection of [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf565-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf565-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf565-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf565-131">Request</span></span>
<span data-ttu-id="cf565-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf565-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts
```

### <a name="response"></a><span data-ttu-id="cf565-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf565-133">Response</span></span>
<span data-ttu-id="cf565-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf565-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 852

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceHealthScript",
      "id": "bcb60502-0502-bcb6-0205-b6bc0205b6bc",
      "publisher": "Publisher value",
      "version": "Version value",
      "displayName": "Display Name value",
      "description": "Description value",
      "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
      "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "runAsAccount": "user",
      "enforceSignatureCheck": true,
      "runAs32Bit": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "isGlobalScript": true,
      "highestAvailableVersion": "Highest Available Version value"
    }
  ]
}
```




