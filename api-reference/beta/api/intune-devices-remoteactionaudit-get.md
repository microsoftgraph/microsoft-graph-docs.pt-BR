---
title: Obter remoteActionAudit
description: Leia as propriedades e as relações do objeto remoteActionAudit.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 623d90302a2d66a7f97638d3c6c325b6ed2cd2a2
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37188231"
---
# <a name="get-remoteactionaudit"></a><span data-ttu-id="aa796-103">Obter remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="aa796-103">Get remoteActionAudit</span></span>

> <span data-ttu-id="aa796-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aa796-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa796-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aa796-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa796-106">Leia as propriedades e as relações do objeto [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="aa796-106">Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa796-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aa796-107">Prerequisites</span></span>
<span data-ttu-id="aa796-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa796-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa796-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa796-110">Permission type</span></span>|<span data-ttu-id="aa796-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aa796-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa796-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa796-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aa796-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa796-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="aa796-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa796-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa796-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa796-115">Not supported.</span></span>|
|<span data-ttu-id="aa796-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa796-116">Application</span></span>|<span data-ttu-id="aa796-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa796-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa796-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa796-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aa796-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="aa796-119">Optional query parameters</span></span>
<span data-ttu-id="aa796-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="aa796-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa796-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa796-121">Request headers</span></span>
|<span data-ttu-id="aa796-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aa796-122">Header</span></span>|<span data-ttu-id="aa796-123">Valor</span><span class="sxs-lookup"><span data-stu-id="aa796-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa796-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa796-124">Authorization</span></span>|<span data-ttu-id="aa796-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa796-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa796-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aa796-126">Accept</span></span>|<span data-ttu-id="aa796-127">application/json</span><span class="sxs-lookup"><span data-stu-id="aa796-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa796-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa796-128">Request body</span></span>
<span data-ttu-id="aa796-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aa796-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa796-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa796-130">Response</span></span>
<span data-ttu-id="aa796-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa796-131">If successful, this method returns a `200 OK` response code and [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa796-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa796-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa796-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa796-133">Request</span></span>
<span data-ttu-id="aa796-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa796-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

### <a name="response"></a><span data-ttu-id="aa796-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa796-135">Response</span></span>
<span data-ttu-id="aa796-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aa796-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 594

{
  "value": {
    "@odata.type": "#microsoft.graph.remoteActionAudit",
    "id": "477f8d24-8d24-477f-248d-7f47248d7f47",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
    "action": "factoryReset",
    "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
    "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
    "deviceIMEI": "Device IMEI value",
    "actionState": "pending",
    "managedDeviceId": "Managed Device Id value"
  }
}
```




