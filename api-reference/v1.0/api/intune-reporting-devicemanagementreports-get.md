---
title: Obter deviceManagementReports
description: Leia propriedades e relações do objeto deviceManagementReports.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fb9cf59d3bcf42ec0a1fc6a68c7ec0cc65a68579
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758510"
---
# <a name="get-devicemanagementreports"></a><span data-ttu-id="5039d-103">Obter deviceManagementReports</span><span class="sxs-lookup"><span data-stu-id="5039d-103">Get deviceManagementReports</span></span>

<span data-ttu-id="5039d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5039d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5039d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5039d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5039d-106">Leia propriedades e relações do [objeto deviceManagementReports.](../resources/intune-reporting-devicemanagementreports.md)</span><span class="sxs-lookup"><span data-stu-id="5039d-106">Read properties and relationships of the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5039d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5039d-107">Prerequisites</span></span>
<span data-ttu-id="5039d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5039d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5039d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5039d-110">Permission type</span></span>|<span data-ttu-id="5039d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5039d-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5039d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5039d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5039d-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5039d-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5039d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5039d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5039d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5039d-115">Not supported.</span></span>|
|<span data-ttu-id="5039d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5039d-116">Application</span></span>|<span data-ttu-id="5039d-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5039d-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5039d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5039d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5039d-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5039d-119">Optional query parameters</span></span>
<span data-ttu-id="5039d-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5039d-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5039d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5039d-121">Request headers</span></span>
|<span data-ttu-id="5039d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5039d-122">Header</span></span>|<span data-ttu-id="5039d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="5039d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5039d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5039d-124">Authorization</span></span>|<span data-ttu-id="5039d-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5039d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5039d-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5039d-126">Accept</span></span>|<span data-ttu-id="5039d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5039d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5039d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5039d-128">Request body</span></span>
<span data-ttu-id="5039d-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5039d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5039d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5039d-130">Response</span></span>
<span data-ttu-id="5039d-131">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5039d-131">If successful, this method returns a `200 OK` response code and [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5039d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5039d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5039d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5039d-133">Request</span></span>
<span data-ttu-id="5039d-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5039d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/reports
```

### <a name="response"></a><span data-ttu-id="5039d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5039d-135">Response</span></span>
<span data-ttu-id="5039d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5039d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 137

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementReports",
    "id": "d6a697d3-97d3-d6a6-d397-a6d6d397a6d6"
  }
}
```




