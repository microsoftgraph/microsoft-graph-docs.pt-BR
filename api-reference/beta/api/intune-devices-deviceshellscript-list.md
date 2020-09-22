---
title: Listar deviceShellScripts
description: Listar Propriedades e relações dos objetos deviceShellScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0c7330a19fb65e17fafde20e5d2e055713a73678
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072547"
---
# <a name="list-deviceshellscripts"></a><span data-ttu-id="b2034-103">Listar deviceShellScripts</span><span class="sxs-lookup"><span data-stu-id="b2034-103">List deviceShellScripts</span></span>

<span data-ttu-id="b2034-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2034-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2034-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b2034-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2034-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2034-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2034-107">Listar Propriedades e relações dos objetos [deviceShellScript](../resources/intune-devices-deviceshellscript.md) .</span><span class="sxs-lookup"><span data-stu-id="b2034-107">List properties and relationships of the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2034-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b2034-108">Prerequisites</span></span>
<span data-ttu-id="b2034-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2034-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2034-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2034-111">Permission type</span></span>|<span data-ttu-id="b2034-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b2034-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2034-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2034-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b2034-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2034-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b2034-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2034-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2034-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2034-116">Not supported.</span></span>|
|<span data-ttu-id="b2034-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2034-117">Application</span></span>|<span data-ttu-id="b2034-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2034-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2034-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2034-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts
```

## <a name="request-headers"></a><span data-ttu-id="b2034-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2034-120">Request headers</span></span>
|<span data-ttu-id="b2034-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2034-121">Header</span></span>|<span data-ttu-id="b2034-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b2034-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2034-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2034-123">Authorization</span></span>|<span data-ttu-id="b2034-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2034-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2034-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b2034-125">Accept</span></span>|<span data-ttu-id="b2034-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b2034-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2034-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2034-127">Request body</span></span>
<span data-ttu-id="b2034-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b2034-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2034-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2034-129">Response</span></span>
<span data-ttu-id="b2034-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [deviceShellScript](../resources/intune-devices-deviceshellscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2034-130">If successful, this method returns a `200 OK` response code and a collection of [deviceShellScript](../resources/intune-devices-deviceshellscript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2034-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2034-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2034-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2034-132">Request</span></span>
<span data-ttu-id="b2034-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2034-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts
```

### <a name="response"></a><span data-ttu-id="b2034-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2034-134">Response</span></span>
<span data-ttu-id="b2034-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2034-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 674

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceShellScript",
      "executionFrequency": "PT2M43.444327S",
      "retryCount": 10,
      "blockExecutionNotifications": true,
      "id": "ca9e0ad8-0ad8-ca9e-d80a-9ecad80a9eca",
      "displayName": "Display Name value",
      "description": "Description value",
      "scriptContent": "c2NyaXB0Q29udGVudA==",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "runAsAccount": "user",
      "fileName": "File Name value",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```






