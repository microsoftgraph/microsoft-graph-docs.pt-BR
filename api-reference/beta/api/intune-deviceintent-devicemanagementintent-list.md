---
title: Listar deviceManagementIntents
description: Listar Propriedades e relações dos objetos deviceManagementIntent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7582014b34a8a0651535d43ed12b8fb67d95d65e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313276"
---
# <a name="list-devicemanagementintents"></a><span data-ttu-id="1dc66-103">Listar deviceManagementIntents</span><span class="sxs-lookup"><span data-stu-id="1dc66-103">List deviceManagementIntents</span></span>

> <span data-ttu-id="1dc66-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1dc66-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1dc66-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1dc66-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dc66-106">Listar Propriedades e relações dos objetos [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) .</span><span class="sxs-lookup"><span data-stu-id="1dc66-106">List properties and relationships of the [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1dc66-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1dc66-107">Prerequisites</span></span>
<span data-ttu-id="1dc66-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dc66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dc66-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1dc66-110">Permission type</span></span>|<span data-ttu-id="1dc66-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1dc66-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1dc66-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1dc66-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1dc66-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1dc66-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1dc66-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1dc66-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1dc66-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1dc66-115">Not supported.</span></span>|
|<span data-ttu-id="1dc66-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dc66-116">Application</span></span>|<span data-ttu-id="1dc66-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1dc66-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1dc66-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1dc66-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents
```

## <a name="request-headers"></a><span data-ttu-id="1dc66-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1dc66-119">Request headers</span></span>
|<span data-ttu-id="1dc66-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1dc66-120">Header</span></span>|<span data-ttu-id="1dc66-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1dc66-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1dc66-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1dc66-122">Authorization</span></span>|<span data-ttu-id="1dc66-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1dc66-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1dc66-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1dc66-124">Accept</span></span>|<span data-ttu-id="1dc66-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1dc66-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dc66-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1dc66-126">Request body</span></span>
<span data-ttu-id="1dc66-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1dc66-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1dc66-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dc66-128">Response</span></span>
<span data-ttu-id="1dc66-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1dc66-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dc66-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1dc66-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1dc66-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1dc66-131">Request</span></span>
<span data-ttu-id="1dc66-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1dc66-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents
```

### <a name="response"></a><span data-ttu-id="1dc66-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dc66-133">Response</span></span>
<span data-ttu-id="1dc66-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1dc66-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 452

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntent",
      "id": "f972c33e-c33e-f972-3ec3-72f93ec372f9",
      "displayName": "Display Name value",
      "description": "Description value",
      "isAssigned": true,
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "templateId": "Template Id value",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```






