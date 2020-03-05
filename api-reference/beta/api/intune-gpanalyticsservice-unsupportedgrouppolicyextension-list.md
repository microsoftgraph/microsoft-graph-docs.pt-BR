---
title: Listar unsupportedGroupPolicyExtensions
description: Listar Propriedades e relações dos objetos unsupportedGroupPolicyExtension.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 007f65f15dba6bfb1fa0a6c4ab2e9260fd828e47
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465335"
---
# <a name="list-unsupportedgrouppolicyextensions"></a><span data-ttu-id="e3831-103">Listar unsupportedGroupPolicyExtensions</span><span class="sxs-lookup"><span data-stu-id="e3831-103">List unsupportedGroupPolicyExtensions</span></span>

<span data-ttu-id="e3831-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e3831-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3831-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e3831-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3831-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e3831-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3831-107">Listar Propriedades e relações dos objetos [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) .</span><span class="sxs-lookup"><span data-stu-id="e3831-107">List properties and relationships of the [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3831-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e3831-108">Prerequisites</span></span>
<span data-ttu-id="e3831-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3831-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3831-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3831-111">Permission type</span></span>|<span data-ttu-id="e3831-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e3831-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3831-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3831-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e3831-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3831-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e3831-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3831-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3831-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3831-116">Not supported.</span></span>|
|<span data-ttu-id="e3831-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3831-117">Application</span></span>|<span data-ttu-id="e3831-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3831-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3831-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3831-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions
```

## <a name="request-headers"></a><span data-ttu-id="e3831-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3831-120">Request headers</span></span>
|<span data-ttu-id="e3831-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e3831-121">Header</span></span>|<span data-ttu-id="e3831-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e3831-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3831-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3831-123">Authorization</span></span>|<span data-ttu-id="e3831-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3831-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3831-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e3831-125">Accept</span></span>|<span data-ttu-id="e3831-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3831-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3831-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3831-127">Request body</span></span>
<span data-ttu-id="e3831-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e3831-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3831-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3831-129">Response</span></span>
<span data-ttu-id="e3831-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3831-130">If successful, this method returns a `200 OK` response code and a collection of [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3831-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3831-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3831-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3831-132">Request</span></span>
<span data-ttu-id="e3831-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3831-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions
```

### <a name="response"></a><span data-ttu-id="e3831-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3831-134">Response</span></span>
<span data-ttu-id="e3831-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3831-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 342

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.unsupportedGroupPolicyExtension",
      "id": "e59ecce2-cce2-e59e-e2cc-9ee5e2cc9ee5",
      "settingScope": "device",
      "namespaceUrl": "https://example.com/namespaceUrl/",
      "extensionType": "Extension Type value",
      "nodeName": "Node Name value"
    }
  ]
}
```





