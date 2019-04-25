---
title: Obter resourceOperation
description: Ler propriedades e relações do objeto resourceOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2ab1a48550e8b99b942baac2bcc9e37542606011
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527599"
---
# <a name="get-resourceoperation"></a><span data-ttu-id="39864-103">Obter resourceOperation</span><span class="sxs-lookup"><span data-stu-id="39864-103">Get resourceOperation</span></span>

> <span data-ttu-id="39864-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="39864-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39864-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="39864-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39864-106">Ler propriedades e relações do objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="39864-106">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39864-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="39864-107">Prerequisites</span></span>
<span data-ttu-id="39864-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39864-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39864-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39864-110">Permission type</span></span>|<span data-ttu-id="39864-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="39864-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39864-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39864-112">Delegated (work or school account)</span></span>|<span data-ttu-id="39864-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="39864-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="39864-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39864-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39864-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39864-115">Not supported.</span></span>|
|<span data-ttu-id="39864-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39864-116">Application</span></span>|<span data-ttu-id="39864-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39864-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39864-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39864-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="39864-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="39864-119">Optional query parameters</span></span>
<span data-ttu-id="39864-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="39864-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="39864-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39864-121">Request headers</span></span>
|<span data-ttu-id="39864-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="39864-122">Header</span></span>|<span data-ttu-id="39864-123">Valor</span><span class="sxs-lookup"><span data-stu-id="39864-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39864-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="39864-124">Authorization</span></span>|<span data-ttu-id="39864-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39864-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39864-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="39864-126">Accept</span></span>|<span data-ttu-id="39864-127">application/json</span><span class="sxs-lookup"><span data-stu-id="39864-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39864-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="39864-128">Request body</span></span>
<span data-ttu-id="39864-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="39864-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39864-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="39864-130">Response</span></span>
<span data-ttu-id="39864-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39864-131">If successful, this method returns a `200 OK` response code and [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39864-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="39864-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="39864-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39864-133">Request</span></span>
<span data-ttu-id="39864-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="39864-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}
```

### <a name="response"></a><span data-ttu-id="39864-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="39864-135">Response</span></span>
<span data-ttu-id="39864-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="39864-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





