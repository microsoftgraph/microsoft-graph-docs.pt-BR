---
title: Obter deviceManagementScript
description: Leia propriedades e relações do objeto deviceManagementScript.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8e3a522a77469e0d664ddf39f1a87d12a51b8500
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867788"
---
# <a name="get-devicemanagementscript"></a><span data-ttu-id="be043-103">Obter deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="be043-103">Get deviceManagementScript</span></span>

<span data-ttu-id="be043-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be043-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="be043-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="be043-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be043-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="be043-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be043-107">Leia propriedades e relações do [objeto deviceManagementScript.](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="be043-107">Read properties and relationships of the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be043-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="be043-108">Prerequisites</span></span>
<span data-ttu-id="be043-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be043-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be043-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be043-111">Permission type</span></span>|<span data-ttu-id="be043-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="be043-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be043-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be043-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="be043-114">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="be043-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="be043-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="be043-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="be043-116">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="be043-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="be043-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="be043-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="be043-118">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be043-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be043-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be043-119">Not supported.</span></span>|
|<span data-ttu-id="be043-120">Application</span><span class="sxs-lookup"><span data-stu-id="be043-120">Application</span></span>||
| <span data-ttu-id="be043-121">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="be043-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="be043-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="be043-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="be043-123">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="be043-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="be043-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="be043-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="be043-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be043-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="be043-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="be043-126">Optional query parameters</span></span>
<span data-ttu-id="be043-127">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="be043-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be043-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be043-128">Request headers</span></span>
|<span data-ttu-id="be043-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="be043-129">Header</span></span>|<span data-ttu-id="be043-130">Valor</span><span class="sxs-lookup"><span data-stu-id="be043-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be043-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="be043-131">Authorization</span></span>|<span data-ttu-id="be043-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be043-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be043-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="be043-133">Accept</span></span>|<span data-ttu-id="be043-134">application/json</span><span class="sxs-lookup"><span data-stu-id="be043-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be043-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be043-135">Request body</span></span>
<span data-ttu-id="be043-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="be043-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be043-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="be043-137">Response</span></span>
<span data-ttu-id="be043-138">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be043-138">If successful, this method returns a `200 OK` response code and [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be043-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="be043-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="be043-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be043-140">Request</span></span>
<span data-ttu-id="be043-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="be043-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

### <a name="response"></a><span data-ttu-id="be043-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="be043-142">Response</span></span>
<span data-ttu-id="be043-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="be043-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







