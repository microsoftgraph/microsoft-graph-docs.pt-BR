---
title: Listar managedAppStatusRaws
description: Listar propriedades e relações dos objetos managedAppStatusRaw.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b18962c5ac51a1e6d287ea009c1dc2f4be65bdef
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36354048"
---
# <a name="list-managedappstatusraws"></a><span data-ttu-id="d9be1-103">Listar managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="d9be1-103">List managedAppStatusRaws</span></span>

> <span data-ttu-id="d9be1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d9be1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9be1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9be1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9be1-106">Listar propriedades e relações dos objetos [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="d9be1-106">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9be1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d9be1-107">Prerequisites</span></span>
<span data-ttu-id="d9be1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9be1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9be1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9be1-110">Permission type</span></span>|<span data-ttu-id="d9be1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d9be1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9be1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9be1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d9be1-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9be1-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d9be1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9be1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9be1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9be1-115">Not supported.</span></span>|
|<span data-ttu-id="d9be1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9be1-116">Application</span></span>|<span data-ttu-id="d9be1-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9be1-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9be1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9be1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a><span data-ttu-id="d9be1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9be1-119">Request headers</span></span>
|<span data-ttu-id="d9be1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d9be1-120">Header</span></span>|<span data-ttu-id="d9be1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d9be1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9be1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9be1-122">Authorization</span></span>|<span data-ttu-id="d9be1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9be1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9be1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d9be1-124">Accept</span></span>|<span data-ttu-id="d9be1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d9be1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9be1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9be1-126">Request body</span></span>
<span data-ttu-id="d9be1-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d9be1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9be1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9be1-128">Response</span></span>
<span data-ttu-id="d9be1-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9be1-129">If successful, this method returns a `200 OK` response code and a collection of [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9be1-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9be1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9be1-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9be1-131">Request</span></span>
<span data-ttu-id="d9be1-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9be1-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppStatuses
```

### <a name="response"></a><span data-ttu-id="d9be1-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9be1-133">Response</span></span>
<span data-ttu-id="d9be1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9be1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






