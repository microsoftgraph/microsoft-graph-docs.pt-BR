---
title: Listar deviceComplianceScripts
description: Listar Propriedades e relações dos objetos deviceComplianceScript.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 96dd9a95930794c56806d05c4de7f07a2dc5d553
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792482"
---
# <a name="list-devicecompliancescripts"></a><span data-ttu-id="d90f2-103">Listar deviceComplianceScripts</span><span class="sxs-lookup"><span data-stu-id="d90f2-103">List deviceComplianceScripts</span></span>

<span data-ttu-id="d90f2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d90f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d90f2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d90f2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d90f2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d90f2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d90f2-107">Listar Propriedades e relações dos objetos [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) .</span><span class="sxs-lookup"><span data-stu-id="d90f2-107">List properties and relationships of the [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d90f2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d90f2-108">Prerequisites</span></span>
<span data-ttu-id="d90f2-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="d90f2-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d90f2-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d90f2-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d90f2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d90f2-111">Permission type</span></span>|<span data-ttu-id="d90f2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d90f2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d90f2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d90f2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d90f2-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d90f2-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d90f2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d90f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d90f2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d90f2-116">Not supported.</span></span>|
|<span data-ttu-id="d90f2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d90f2-117">Application</span></span>|<span data-ttu-id="d90f2-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d90f2-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d90f2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d90f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceComplianceScripts
```

## <a name="request-headers"></a><span data-ttu-id="d90f2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d90f2-120">Request headers</span></span>
|<span data-ttu-id="d90f2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d90f2-121">Header</span></span>|<span data-ttu-id="d90f2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d90f2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d90f2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d90f2-123">Authorization</span></span>|<span data-ttu-id="d90f2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d90f2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d90f2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d90f2-125">Accept</span></span>|<span data-ttu-id="d90f2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d90f2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d90f2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d90f2-127">Request body</span></span>
<span data-ttu-id="d90f2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d90f2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d90f2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d90f2-129">Response</span></span>
<span data-ttu-id="d90f2-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d90f2-130">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d90f2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d90f2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d90f2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d90f2-132">Request</span></span>
<span data-ttu-id="d90f2-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d90f2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts
```

### <a name="response"></a><span data-ttu-id="d90f2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d90f2-134">Response</span></span>
<span data-ttu-id="d90f2-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="d90f2-135">Here is an example of the response.</span></span> <span data-ttu-id="d90f2-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="d90f2-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d90f2-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="d90f2-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 685

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceScript",
      "id": "14e72a7b-2a7b-14e7-7b2a-e7147b2ae714",
      "publisher": "Publisher value",
      "version": "Version value",
      "displayName": "Display Name value",
      "description": "Description value",
      "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "runAsAccount": "user",
      "enforceSignatureCheck": true,
      "runAs32Bit": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```



