---
title: Atualizar deviceManagementReports
description: Atualiza as propriedades de um objeto deviceManagementReports.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 49043d957ca0f0e5e30b69abd9524b54a68d025c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459103"
---
# <a name="update-devicemanagementreports"></a><span data-ttu-id="099e4-103">Atualizar deviceManagementReports</span><span class="sxs-lookup"><span data-stu-id="099e4-103">Update deviceManagementReports</span></span>

<span data-ttu-id="099e4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="099e4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="099e4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="099e4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="099e4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="099e4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="099e4-107">Atualiza as propriedades de um objeto [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) .</span><span class="sxs-lookup"><span data-stu-id="099e4-107">Update the properties of a [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="099e4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="099e4-108">Prerequisites</span></span>
<span data-ttu-id="099e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="099e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="099e4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="099e4-111">Permission type</span></span>|<span data-ttu-id="099e4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="099e4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="099e4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="099e4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="099e4-114">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="099e4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="099e4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="099e4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="099e4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="099e4-116">Not supported.</span></span>|
|<span data-ttu-id="099e4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="099e4-117">Application</span></span>|<span data-ttu-id="099e4-118">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="099e4-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="099e4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="099e4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports
```

## <a name="request-headers"></a><span data-ttu-id="099e4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="099e4-120">Request headers</span></span>
|<span data-ttu-id="099e4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="099e4-121">Header</span></span>|<span data-ttu-id="099e4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="099e4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="099e4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="099e4-123">Authorization</span></span>|<span data-ttu-id="099e4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="099e4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="099e4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="099e4-125">Accept</span></span>|<span data-ttu-id="099e4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="099e4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="099e4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="099e4-127">Request body</span></span>
<span data-ttu-id="099e4-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) .</span><span class="sxs-lookup"><span data-stu-id="099e4-128">In the request body, supply a JSON representation for the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

<span data-ttu-id="099e4-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md).</span><span class="sxs-lookup"><span data-stu-id="099e4-129">The following table shows the properties that are required when you create the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md).</span></span>

|<span data-ttu-id="099e4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="099e4-130">Property</span></span>|<span data-ttu-id="099e4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="099e4-131">Type</span></span>|<span data-ttu-id="099e4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="099e4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="099e4-133">id</span><span class="sxs-lookup"><span data-stu-id="099e4-133">id</span></span>|<span data-ttu-id="099e4-134">String</span><span class="sxs-lookup"><span data-stu-id="099e4-134">String</span></span>|<span data-ttu-id="099e4-135">Identificador exclusivo para esta entidade</span><span class="sxs-lookup"><span data-stu-id="099e4-135">Unique identifier for this entity</span></span>|



## <a name="response"></a><span data-ttu-id="099e4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="099e4-136">Response</span></span>
<span data-ttu-id="099e4-137">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="099e4-137">If successful, this method returns a `200 OK` response code and an updated [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="099e4-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="099e4-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="099e4-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="099e4-139">Request</span></span>
<span data-ttu-id="099e4-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="099e4-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.deviceManagementReports"
}
```

### <a name="response"></a><span data-ttu-id="099e4-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="099e4-141">Response</span></span>
<span data-ttu-id="099e4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="099e4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "d6a697d3-97d3-d6a6-d397-a6d6d397a6d6"
}
```





