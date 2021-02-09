---
title: Listar mobileAppDependencies
description: Listar propriedades e relações dos objetos mobileAppDependency.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ef3b75c8d3e30fda7483eaee77ac58630d49c5d7
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157201"
---
# <a name="list-mobileappdependencies"></a><span data-ttu-id="67a9d-103">Listar mobileAppDependencies</span><span class="sxs-lookup"><span data-stu-id="67a9d-103">List mobileAppDependencies</span></span>

<span data-ttu-id="67a9d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67a9d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67a9d-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="67a9d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67a9d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67a9d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67a9d-107">Listar propriedades e relações dos objetos [mobileAppDependency.](../resources/intune-apps-mobileappdependency.md)</span><span class="sxs-lookup"><span data-stu-id="67a9d-107">List properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67a9d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="67a9d-108">Prerequisites</span></span>
<span data-ttu-id="67a9d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67a9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67a9d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67a9d-111">Permission type</span></span>|<span data-ttu-id="67a9d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="67a9d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67a9d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67a9d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="67a9d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="67a9d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="67a9d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67a9d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67a9d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67a9d-116">Not supported.</span></span>|
|<span data-ttu-id="67a9d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67a9d-117">Application</span></span>|<span data-ttu-id="67a9d-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="67a9d-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="67a9d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67a9d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="67a9d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67a9d-120">Request headers</span></span>
|<span data-ttu-id="67a9d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67a9d-121">Header</span></span>|<span data-ttu-id="67a9d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="67a9d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67a9d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="67a9d-123">Authorization</span></span>|<span data-ttu-id="67a9d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67a9d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67a9d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="67a9d-125">Accept</span></span>|<span data-ttu-id="67a9d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="67a9d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67a9d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67a9d-127">Request body</span></span>
<span data-ttu-id="67a9d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="67a9d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67a9d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="67a9d-129">Response</span></span>
<span data-ttu-id="67a9d-130">Se bem-sucedido, este método retorna um código de resposta e uma `200 OK` coleção de [objetos mobileAppDependency](../resources/intune-apps-mobileappdependency.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67a9d-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67a9d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67a9d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="67a9d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67a9d-132">Request</span></span>
<span data-ttu-id="67a9d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67a9d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

### <a name="response"></a><span data-ttu-id="67a9d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="67a9d-134">Response</span></span>
<span data-ttu-id="67a9d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67a9d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 494

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppDependency",
      "id": "c7f6f9ab-f9ab-c7f6-abf9-f6c7abf9f6c7",
      "targetId": "Target Id value",
      "targetDisplayName": "Target Display Name value",
      "targetDisplayVersion": "Target Display Version value",
      "targetPublisher": "Target Publisher value",
      "targetType": "parent",
      "dependencyType": "autoInstall",
      "dependentAppCount": 1,
      "dependsOnAppCount": 1
    }
  ]
}
```




