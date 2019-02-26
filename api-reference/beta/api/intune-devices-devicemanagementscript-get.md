---
title: Obter deviceManagementScript
description: Leia as propriedades e as relações do objeto deviceManagementScript.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0e3d8ae3c6b28d9a4527bdf477a0250c4d9c2aa2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170543"
---
# <a name="get-devicemanagementscript"></a><span data-ttu-id="1fe14-103">Obter deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="1fe14-103">Get deviceManagementScript</span></span>

> <span data-ttu-id="1fe14-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1fe14-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1fe14-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1fe14-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fe14-106">Leia as propriedades e as relações do objeto [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="1fe14-106">Read properties and relationships of the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1fe14-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1fe14-107">Prerequisites</span></span>
<span data-ttu-id="1fe14-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1fe14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1fe14-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1fe14-110">Permission type</span></span>|<span data-ttu-id="1fe14-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1fe14-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fe14-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1fe14-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1fe14-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1fe14-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="1fe14-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1fe14-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fe14-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fe14-115">Not supported.</span></span>|
|<span data-ttu-id="1fe14-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1fe14-116">Application</span></span>|<span data-ttu-id="1fe14-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fe14-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fe14-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1fe14-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1fe14-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1fe14-119">Optional query parameters</span></span>
<span data-ttu-id="1fe14-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1fe14-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1fe14-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1fe14-121">Request headers</span></span>
|<span data-ttu-id="1fe14-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1fe14-122">Header</span></span>|<span data-ttu-id="1fe14-123">Valor</span><span class="sxs-lookup"><span data-stu-id="1fe14-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fe14-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1fe14-124">Authorization</span></span>|<span data-ttu-id="1fe14-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fe14-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fe14-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1fe14-126">Accept</span></span>|<span data-ttu-id="1fe14-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1fe14-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fe14-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1fe14-128">Request body</span></span>
<span data-ttu-id="1fe14-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1fe14-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1fe14-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fe14-130">Response</span></span>
<span data-ttu-id="1fe14-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1fe14-131">If successful, this method returns a `200 OK` response code and [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fe14-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1fe14-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1fe14-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1fe14-133">Request</span></span>
<span data-ttu-id="1fe14-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1fe14-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

### <a name="response"></a><span data-ttu-id="1fe14-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fe14-135">Response</span></span>
<span data-ttu-id="1fe14-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1fe14-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 668

{
  "value": {
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
}
```




