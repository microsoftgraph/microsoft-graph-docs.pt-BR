---
title: Atualizar deviceManagementReports
description: Atualiza as propriedades de um objeto deviceManagementReports.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 034f8a6c67da7a00f1e23ad86d2849a2e38de8bb
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537202"
---
# <a name="update-devicemanagementreports"></a><span data-ttu-id="a77ae-103">Atualizar deviceManagementReports</span><span class="sxs-lookup"><span data-stu-id="a77ae-103">Update deviceManagementReports</span></span>

> <span data-ttu-id="a77ae-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a77ae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a77ae-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a77ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a77ae-106">Atualiza as propriedades de um objeto [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) .</span><span class="sxs-lookup"><span data-stu-id="a77ae-106">Update the properties of a [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a77ae-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a77ae-107">Prerequisites</span></span>
<span data-ttu-id="a77ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a77ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a77ae-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a77ae-110">Permission type</span></span>|<span data-ttu-id="a77ae-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a77ae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a77ae-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a77ae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a77ae-113">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a77ae-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a77ae-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a77ae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a77ae-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a77ae-115">Not supported.</span></span>|
|<span data-ttu-id="a77ae-116">Application</span><span class="sxs-lookup"><span data-stu-id="a77ae-116">Application</span></span>|<span data-ttu-id="a77ae-117">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a77ae-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a77ae-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a77ae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports
```

## <a name="request-headers"></a><span data-ttu-id="a77ae-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a77ae-119">Request headers</span></span>
|<span data-ttu-id="a77ae-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a77ae-120">Header</span></span>|<span data-ttu-id="a77ae-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a77ae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a77ae-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a77ae-122">Authorization</span></span>|<span data-ttu-id="a77ae-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a77ae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a77ae-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a77ae-124">Accept</span></span>|<span data-ttu-id="a77ae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a77ae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a77ae-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a77ae-126">Request body</span></span>
<span data-ttu-id="a77ae-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) .</span><span class="sxs-lookup"><span data-stu-id="a77ae-127">In the request body, supply a JSON representation for the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

<span data-ttu-id="a77ae-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md).</span><span class="sxs-lookup"><span data-stu-id="a77ae-128">The following table shows the properties that are required when you create the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md).</span></span>

|<span data-ttu-id="a77ae-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a77ae-129">Property</span></span>|<span data-ttu-id="a77ae-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a77ae-130">Type</span></span>|<span data-ttu-id="a77ae-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a77ae-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a77ae-132">id</span><span class="sxs-lookup"><span data-stu-id="a77ae-132">id</span></span>|<span data-ttu-id="a77ae-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a77ae-133">String</span></span>|<span data-ttu-id="a77ae-134">Identificador exclusivo para esta entidade</span><span class="sxs-lookup"><span data-stu-id="a77ae-134">Unique identifier for this entity</span></span>|



## <a name="response"></a><span data-ttu-id="a77ae-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a77ae-135">Response</span></span>
<span data-ttu-id="a77ae-136">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a77ae-136">If successful, this method returns a `200 OK` response code and an updated [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a77ae-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a77ae-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="a77ae-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a77ae-138">Request</span></span>
<span data-ttu-id="a77ae-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a77ae-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.deviceManagementReports"
}
```

### <a name="response"></a><span data-ttu-id="a77ae-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a77ae-140">Response</span></span>
<span data-ttu-id="a77ae-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a77ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "d6a697d3-97d3-d6a6-d397-a6d6d397a6d6"
}
```






