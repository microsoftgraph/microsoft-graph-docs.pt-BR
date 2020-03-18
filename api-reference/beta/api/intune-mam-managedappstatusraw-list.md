---
title: Listar managedAppStatusRaws
description: Listar propriedades e relações dos objetos managedAppStatusRaw.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0ed40045e1f9e823bba88b9b551470de0ed1fc13
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803474"
---
# <a name="list-managedappstatusraws"></a><span data-ttu-id="a7564-103">Listar managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="a7564-103">List managedAppStatusRaws</span></span>

> <span data-ttu-id="a7564-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a7564-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7564-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a7564-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7564-106">Listar propriedades e relações dos objetos [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="a7564-106">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7564-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a7564-107">Prerequisites</span></span>
<span data-ttu-id="a7564-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7564-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7564-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7564-110">Permission type</span></span>|<span data-ttu-id="a7564-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a7564-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7564-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7564-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a7564-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7564-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a7564-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7564-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7564-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7564-115">Not supported.</span></span>|
|<span data-ttu-id="a7564-116">Application</span><span class="sxs-lookup"><span data-stu-id="a7564-116">Application</span></span>|<span data-ttu-id="a7564-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7564-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7564-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7564-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a><span data-ttu-id="a7564-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7564-119">Request headers</span></span>
|<span data-ttu-id="a7564-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a7564-120">Header</span></span>|<span data-ttu-id="a7564-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a7564-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7564-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7564-122">Authorization</span></span>|<span data-ttu-id="a7564-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7564-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7564-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a7564-124">Accept</span></span>|<span data-ttu-id="a7564-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a7564-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7564-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7564-126">Request body</span></span>
<span data-ttu-id="a7564-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a7564-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7564-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7564-128">Response</span></span>
<span data-ttu-id="a7564-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7564-129">If successful, this method returns a `200 OK` response code and a collection of [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7564-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a7564-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7564-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7564-131">Request</span></span>
<span data-ttu-id="a7564-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7564-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppStatuses
```

### <a name="response"></a><span data-ttu-id="a7564-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7564-133">Response</span></span>
<span data-ttu-id="a7564-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a7564-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 307

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppStatusRaw",
      "displayName": "Display Name value",
      "id": "80847581-7581-8084-8175-848081758480",
      "version": "Version value",
      "content": {
        "@odata.type": "microsoft.graph.Json"
      }
    }
  ]
}
```




