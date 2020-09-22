---
title: Obter resourceOperation
description: Ler propriedades e relações do objeto resourceOperation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bc4e8f62b22a25e1f1860cb860fc0d35135d74c5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058792"
---
# <a name="get-resourceoperation"></a><span data-ttu-id="6e132-103">Obter resourceOperation</span><span class="sxs-lookup"><span data-stu-id="6e132-103">Get resourceOperation</span></span>

<span data-ttu-id="6e132-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e132-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e132-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6e132-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e132-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6e132-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e132-107">Ler propriedades e relações do objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="6e132-107">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e132-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6e132-108">Prerequisites</span></span>
<span data-ttu-id="6e132-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e132-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e132-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e132-111">Permission type</span></span>|<span data-ttu-id="6e132-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6e132-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e132-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e132-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e132-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e132-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="6e132-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e132-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e132-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e132-116">Not supported.</span></span>|
|<span data-ttu-id="6e132-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e132-117">Application</span></span>|<span data-ttu-id="6e132-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e132-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e132-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e132-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6e132-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6e132-120">Optional query parameters</span></span>
<span data-ttu-id="6e132-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6e132-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e132-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e132-122">Request headers</span></span>
|<span data-ttu-id="6e132-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6e132-123">Header</span></span>|<span data-ttu-id="6e132-124">Valor</span><span class="sxs-lookup"><span data-stu-id="6e132-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e132-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e132-125">Authorization</span></span>|<span data-ttu-id="6e132-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e132-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e132-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6e132-127">Accept</span></span>|<span data-ttu-id="6e132-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6e132-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e132-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e132-129">Request body</span></span>
<span data-ttu-id="6e132-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6e132-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e132-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e132-131">Response</span></span>
<span data-ttu-id="6e132-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e132-132">If successful, this method returns a `200 OK` response code and [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e132-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e132-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e132-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e132-134">Request</span></span>
<span data-ttu-id="6e132-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e132-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}
```

### <a name="response"></a><span data-ttu-id="6e132-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e132-136">Response</span></span>
<span data-ttu-id="6e132-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e132-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 331

{
  "value": {
    "@odata.type": "#microsoft.graph.resourceOperation",
    "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
    "resource": "Resource value",
    "resourceName": "Resource Name value",
    "actionName": "Action Name value",
    "description": "Description value",
    "enabledForScopeValidation": true
  }
}
```






