---
title: Listar deviceHealthScripts
description: Listar Propriedades e relações dos objetos deviceHealthScript.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0e200369dd4ce21199fd5cfd494811a9997915c6
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162194"
---
# <a name="list-devicehealthscripts"></a><span data-ttu-id="1a825-103">Listar deviceHealthScripts</span><span class="sxs-lookup"><span data-stu-id="1a825-103">List deviceHealthScripts</span></span>

> <span data-ttu-id="1a825-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1a825-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a825-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1a825-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a825-106">Listar Propriedades e relações dos objetos [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="1a825-106">List properties and relationships of the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a825-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1a825-107">Prerequisites</span></span>
<span data-ttu-id="1a825-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a825-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a825-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a825-110">Permission type</span></span>|<span data-ttu-id="1a825-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1a825-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a825-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a825-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1a825-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a825-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1a825-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a825-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a825-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a825-115">Not supported.</span></span>|
|<span data-ttu-id="1a825-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a825-116">Application</span></span>|<span data-ttu-id="1a825-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a825-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a825-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a825-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts
```

## <a name="request-headers"></a><span data-ttu-id="1a825-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a825-119">Request headers</span></span>
|<span data-ttu-id="1a825-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1a825-120">Header</span></span>|<span data-ttu-id="1a825-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1a825-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a825-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a825-122">Authorization</span></span>|<span data-ttu-id="1a825-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a825-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a825-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1a825-124">Accept</span></span>|<span data-ttu-id="1a825-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1a825-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a825-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a825-126">Request body</span></span>
<span data-ttu-id="1a825-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1a825-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a825-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a825-128">Response</span></span>
<span data-ttu-id="1a825-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a825-129">If successful, this method returns a `200 OK` response code and a collection of [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a825-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1a825-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a825-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a825-131">Request</span></span>
<span data-ttu-id="1a825-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a825-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts
```

### <a name="response"></a><span data-ttu-id="1a825-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a825-133">Response</span></span>
<span data-ttu-id="1a825-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1a825-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





