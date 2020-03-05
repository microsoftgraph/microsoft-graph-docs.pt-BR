---
title: Listar deviceManagementIntents
description: Listar Propriedades e relações dos objetos deviceManagementIntent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4c996cf37b90a639f1bb6f5fb559e6dd6b78dcb1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42471376"
---
# <a name="list-devicemanagementintents"></a><span data-ttu-id="90c9c-103">Listar deviceManagementIntents</span><span class="sxs-lookup"><span data-stu-id="90c9c-103">List deviceManagementIntents</span></span>

<span data-ttu-id="90c9c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="90c9c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90c9c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="90c9c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90c9c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="90c9c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90c9c-107">Listar Propriedades e relações dos objetos [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) .</span><span class="sxs-lookup"><span data-stu-id="90c9c-107">List properties and relationships of the [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90c9c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="90c9c-108">Prerequisites</span></span>
<span data-ttu-id="90c9c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90c9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90c9c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90c9c-111">Permission type</span></span>|<span data-ttu-id="90c9c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="90c9c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90c9c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90c9c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90c9c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="90c9c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="90c9c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90c9c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90c9c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90c9c-116">Not supported.</span></span>|
|<span data-ttu-id="90c9c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90c9c-117">Application</span></span>|<span data-ttu-id="90c9c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="90c9c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90c9c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90c9c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents
```

## <a name="request-headers"></a><span data-ttu-id="90c9c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90c9c-120">Request headers</span></span>
|<span data-ttu-id="90c9c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="90c9c-121">Header</span></span>|<span data-ttu-id="90c9c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="90c9c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90c9c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="90c9c-123">Authorization</span></span>|<span data-ttu-id="90c9c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90c9c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90c9c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="90c9c-125">Accept</span></span>|<span data-ttu-id="90c9c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90c9c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90c9c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90c9c-127">Request body</span></span>
<span data-ttu-id="90c9c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="90c9c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90c9c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="90c9c-129">Response</span></span>
<span data-ttu-id="90c9c-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90c9c-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90c9c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90c9c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="90c9c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90c9c-132">Request</span></span>
<span data-ttu-id="90c9c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90c9c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents
```

### <a name="response"></a><span data-ttu-id="90c9c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="90c9c-134">Response</span></span>
<span data-ttu-id="90c9c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90c9c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





