---
title: Listar deviceComplianceScripts
description: Listar Propriedades e relações dos objetos deviceComplianceScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 04c6c9ae186097d77c3752842c227ece43115ee2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48011274"
---
# <a name="list-devicecompliancescripts"></a><span data-ttu-id="bd6b1-103">Listar deviceComplianceScripts</span><span class="sxs-lookup"><span data-stu-id="bd6b1-103">List deviceComplianceScripts</span></span>

<span data-ttu-id="bd6b1-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="bd6b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bd6b1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bd6b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd6b1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bd6b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd6b1-107">Listar Propriedades e relações dos objetos [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) .</span><span class="sxs-lookup"><span data-stu-id="bd6b1-107">List properties and relationships of the [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd6b1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bd6b1-108">Prerequisites</span></span>
<span data-ttu-id="bd6b1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd6b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd6b1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd6b1-111">Permission type</span></span>|<span data-ttu-id="bd6b1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bd6b1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd6b1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd6b1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bd6b1-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd6b1-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="bd6b1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd6b1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd6b1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd6b1-116">Not supported.</span></span>|
|<span data-ttu-id="bd6b1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd6b1-117">Application</span></span>|<span data-ttu-id="bd6b1-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd6b1-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd6b1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd6b1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceComplianceScripts
```

## <a name="request-headers"></a><span data-ttu-id="bd6b1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd6b1-120">Request headers</span></span>
|<span data-ttu-id="bd6b1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bd6b1-121">Header</span></span>|<span data-ttu-id="bd6b1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bd6b1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd6b1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd6b1-123">Authorization</span></span>|<span data-ttu-id="bd6b1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd6b1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd6b1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bd6b1-125">Accept</span></span>|<span data-ttu-id="bd6b1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bd6b1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd6b1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd6b1-127">Request body</span></span>
<span data-ttu-id="bd6b1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bd6b1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd6b1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd6b1-129">Response</span></span>
<span data-ttu-id="bd6b1-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd6b1-130">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd6b1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bd6b1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd6b1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd6b1-132">Request</span></span>
<span data-ttu-id="bd6b1-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd6b1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts
```

### <a name="response"></a><span data-ttu-id="bd6b1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd6b1-134">Response</span></span>
<span data-ttu-id="bd6b1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bd6b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






