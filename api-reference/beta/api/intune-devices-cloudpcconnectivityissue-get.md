---
title: Obter cloudPCConnectivityIssue
description: Leia propriedades e relações do objeto cloudPCConnectivityIssue.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b0a6595d833cb973deb460f39724010a7f70501f
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664812"
---
# <a name="get-cloudpcconnectivityissue"></a><span data-ttu-id="e0ae1-103">Obter cloudPCConnectivityIssue</span><span class="sxs-lookup"><span data-stu-id="e0ae1-103">Get cloudPCConnectivityIssue</span></span>

<span data-ttu-id="e0ae1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0ae1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0ae1-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e0ae1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0ae1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e0ae1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0ae1-107">Leia propriedades e relações do [objeto cloudPCConnectivityIssue.](../resources/intune-devices-cloudpcconnectivityissue.md)</span><span class="sxs-lookup"><span data-stu-id="e0ae1-107">Read properties and relationships of the [cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0ae1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e0ae1-108">Prerequisites</span></span>
<span data-ttu-id="e0ae1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0ae1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0ae1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0ae1-111">Permission type</span></span>|<span data-ttu-id="e0ae1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0ae1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0ae1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0ae1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e0ae1-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0ae1-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e0ae1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0ae1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0ae1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0ae1-116">Not supported.</span></span>|
|<span data-ttu-id="e0ae1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0ae1-117">Application</span></span>|<span data-ttu-id="e0ae1-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0ae1-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0ae1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0ae1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/cloudPCConnectivityIssues/{cloudPCConnectivityIssueId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e0ae1-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e0ae1-120">Optional query parameters</span></span>
<span data-ttu-id="e0ae1-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e0ae1-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0ae1-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0ae1-122">Request headers</span></span>
|<span data-ttu-id="e0ae1-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e0ae1-123">Header</span></span>|<span data-ttu-id="e0ae1-124">Valor</span><span class="sxs-lookup"><span data-stu-id="e0ae1-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0ae1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0ae1-125">Authorization</span></span>|<span data-ttu-id="e0ae1-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0ae1-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0ae1-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e0ae1-127">Accept</span></span>|<span data-ttu-id="e0ae1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e0ae1-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0ae1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0ae1-129">Request body</span></span>
<span data-ttu-id="e0ae1-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e0ae1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0ae1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0ae1-131">Response</span></span>
<span data-ttu-id="e0ae1-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0ae1-132">If successful, this method returns a `200 OK` response code and [cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0ae1-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0ae1-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0ae1-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0ae1-134">Request</span></span>
<span data-ttu-id="e0ae1-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0ae1-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/cloudPCConnectivityIssues/{cloudPCConnectivityIssueId}
```

### <a name="response"></a><span data-ttu-id="e0ae1-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0ae1-136">Response</span></span>
<span data-ttu-id="e0ae1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0ae1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPCConnectivityIssue",
    "id": "e8e2bf5f-bf5f-e8e2-5fbf-e2e85fbfe2e8",
    "deviceId": "Device Id value",
    "errorCode": "Error Code value",
    "errorDateTime": "2016-12-31T23:58:20.6032957-08:00",
    "userId": "User Id value",
    "errorDescription": "Error Description value",
    "recommendedAction": "Recommended Action value"
  }
}
```




