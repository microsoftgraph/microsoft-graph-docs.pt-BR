---
title: Listar mobileAppDependencies
description: Listar Propriedades e relações dos objetos mobileAppDependency.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6fe13b2d62a9f5d4bffed4daf1f682dce33d7bc4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31809168"
---
# <a name="list-mobileappdependencies"></a><span data-ttu-id="33b19-103">Listar mobileAppDependencies</span><span class="sxs-lookup"><span data-stu-id="33b19-103">List mobileAppDependencies</span></span>

> <span data-ttu-id="33b19-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="33b19-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33b19-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="33b19-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33b19-106">Listar Propriedades e relações dos objetos [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) .</span><span class="sxs-lookup"><span data-stu-id="33b19-106">List properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33b19-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="33b19-107">Prerequisites</span></span>
<span data-ttu-id="33b19-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33b19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33b19-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33b19-110">Permission type</span></span>|<span data-ttu-id="33b19-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="33b19-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33b19-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33b19-112">Delegated (work or school account)</span></span>|<span data-ttu-id="33b19-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="33b19-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="33b19-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33b19-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33b19-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33b19-115">Not supported.</span></span>|
|<span data-ttu-id="33b19-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33b19-116">Application</span></span>|<span data-ttu-id="33b19-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33b19-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33b19-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33b19-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="33b19-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33b19-119">Request headers</span></span>
|<span data-ttu-id="33b19-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="33b19-120">Header</span></span>|<span data-ttu-id="33b19-121">Valor</span><span class="sxs-lookup"><span data-stu-id="33b19-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33b19-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="33b19-122">Authorization</span></span>|<span data-ttu-id="33b19-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33b19-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33b19-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="33b19-124">Accept</span></span>|<span data-ttu-id="33b19-125">application/json</span><span class="sxs-lookup"><span data-stu-id="33b19-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33b19-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33b19-126">Request body</span></span>
<span data-ttu-id="33b19-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="33b19-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33b19-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="33b19-128">Response</span></span>
<span data-ttu-id="33b19-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33b19-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33b19-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33b19-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="33b19-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33b19-131">Request</span></span>
<span data-ttu-id="33b19-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33b19-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

### <a name="response"></a><span data-ttu-id="33b19-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="33b19-133">Response</span></span>
<span data-ttu-id="33b19-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33b19-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppDependency",
      "id": "c7f6f9ab-f9ab-c7f6-abf9-f6c7abf9f6c7",
      "targetId": "Target Id value",
      "targetDisplayName": "Target Display Name value",
      "dependencyType": "autoInstall",
      "dependentAppCount": 1
    }
  ]
}
```





