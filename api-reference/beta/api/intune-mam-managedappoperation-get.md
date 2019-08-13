---
title: Get managedAppOperation
description: Ler propriedades e relações do objeto managedAppOperation.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c8a9b915160a5a1f652f3ca1f4c4c2a59af91a5c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36354230"
---
# <a name="get-managedappoperation"></a><span data-ttu-id="869f2-103">Get managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="869f2-103">Get managedAppOperation</span></span>

> <span data-ttu-id="869f2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="869f2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="869f2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="869f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="869f2-106">Ler propriedades e relações do objeto [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="869f2-106">Read properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="869f2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="869f2-107">Prerequisites</span></span>
<span data-ttu-id="869f2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="869f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="869f2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="869f2-110">Permission type</span></span>|<span data-ttu-id="869f2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="869f2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="869f2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="869f2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="869f2-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="869f2-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="869f2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="869f2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="869f2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="869f2-115">Not supported.</span></span>|
|<span data-ttu-id="869f2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="869f2-116">Application</span></span>|<span data-ttu-id="869f2-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="869f2-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="869f2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="869f2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="869f2-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="869f2-119">Optional query parameters</span></span>
<span data-ttu-id="869f2-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="869f2-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="869f2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="869f2-121">Request headers</span></span>
|<span data-ttu-id="869f2-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="869f2-122">Header</span></span>|<span data-ttu-id="869f2-123">Valor</span><span class="sxs-lookup"><span data-stu-id="869f2-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="869f2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="869f2-124">Authorization</span></span>|<span data-ttu-id="869f2-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="869f2-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="869f2-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="869f2-126">Accept</span></span>|<span data-ttu-id="869f2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="869f2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="869f2-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="869f2-128">Request body</span></span>
<span data-ttu-id="869f2-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="869f2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="869f2-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="869f2-130">Response</span></span>
<span data-ttu-id="869f2-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedAppOperation](../resources/intune-mam-managedappoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="869f2-131">If successful, this method returns a `200 OK` response code and [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="869f2-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="869f2-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="869f2-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="869f2-133">Request</span></span>
<span data-ttu-id="869f2-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="869f2-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

### <a name="response"></a><span data-ttu-id="869f2-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="869f2-135">Response</span></span>
<span data-ttu-id="869f2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="869f2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 303

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppOperation",
    "displayName": "Display Name value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "state": "State value",
    "id": "f2867b06-7b06-f286-067b-86f2067b86f2",
    "version": "Version value"
  }
}
```






