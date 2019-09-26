---
title: Listar macManagedAppProtections
description: Listar Propriedades e relações dos objetos macManagedAppProtection.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a16d41a3c1916d4d5f81f5e7cf7a3634db9938d9
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37191790"
---
# <a name="list-macmanagedappprotections"></a><span data-ttu-id="cd4d0-103">Listar macManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="cd4d0-103">List macManagedAppProtections</span></span>

> <span data-ttu-id="cd4d0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cd4d0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd4d0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cd4d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd4d0-106">Listar Propriedades e relações dos objetos [macManagedAppProtection](../resources/intune-policyset-macmanagedappprotection.md) .</span><span class="sxs-lookup"><span data-stu-id="cd4d0-106">List properties and relationships of the [macManagedAppProtection](../resources/intune-policyset-macmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd4d0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cd4d0-107">Prerequisites</span></span>
<span data-ttu-id="cd4d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd4d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd4d0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd4d0-110">Permission type</span></span>|<span data-ttu-id="cd4d0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cd4d0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd4d0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd4d0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cd4d0-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd4d0-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cd4d0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd4d0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd4d0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd4d0-115">Not supported.</span></span>|
|<span data-ttu-id="cd4d0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd4d0-116">Application</span></span>|<span data-ttu-id="cd4d0-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd4d0-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd4d0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd4d0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/macManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="cd4d0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd4d0-119">Request headers</span></span>
|<span data-ttu-id="cd4d0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cd4d0-120">Header</span></span>|<span data-ttu-id="cd4d0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cd4d0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd4d0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd4d0-122">Authorization</span></span>|<span data-ttu-id="cd4d0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd4d0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd4d0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cd4d0-124">Accept</span></span>|<span data-ttu-id="cd4d0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cd4d0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd4d0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd4d0-126">Request body</span></span>
<span data-ttu-id="cd4d0-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cd4d0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd4d0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd4d0-128">Response</span></span>
<span data-ttu-id="cd4d0-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [macManagedAppProtection](../resources/intune-policyset-macmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cd4d0-129">If successful, this method returns a `200 OK` response code and a collection of [macManagedAppProtection](../resources/intune-policyset-macmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd4d0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cd4d0-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd4d0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd4d0-131">Request</span></span>
<span data-ttu-id="cd4d0-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd4d0-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/macManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="cd4d0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd4d0-133">Response</span></span>
<span data-ttu-id="cd4d0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cd4d0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 155

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macManagedAppProtection",
      "id": "bb139531-9531-bb13-3195-13bb319513bb"
    }
  ]
}
```




