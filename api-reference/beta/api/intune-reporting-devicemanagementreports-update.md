---
title: Atualizar deviceManagementReports
description: Atualiza as propriedades de um objeto deviceManagementReports.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7e00e9a9f6e9e3ff2e0586f576a118608388cf27
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801352"
---
# <a name="update-devicemanagementreports"></a><span data-ttu-id="3d891-103">Atualizar deviceManagementReports</span><span class="sxs-lookup"><span data-stu-id="3d891-103">Update deviceManagementReports</span></span>

> <span data-ttu-id="3d891-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3d891-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d891-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3d891-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d891-106">Atualiza as propriedades de um objeto [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) .</span><span class="sxs-lookup"><span data-stu-id="3d891-106">Update the properties of a [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d891-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3d891-107">Prerequisites</span></span>
<span data-ttu-id="3d891-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d891-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d891-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d891-110">Permission type</span></span>|<span data-ttu-id="3d891-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3d891-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d891-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d891-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3d891-113">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3d891-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3d891-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d891-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d891-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d891-115">Not supported.</span></span>|
|<span data-ttu-id="3d891-116">Application</span><span class="sxs-lookup"><span data-stu-id="3d891-116">Application</span></span>|<span data-ttu-id="3d891-117">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3d891-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d891-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d891-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports
```

## <a name="request-headers"></a><span data-ttu-id="3d891-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d891-119">Request headers</span></span>
|<span data-ttu-id="3d891-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3d891-120">Header</span></span>|<span data-ttu-id="3d891-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3d891-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d891-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d891-122">Authorization</span></span>|<span data-ttu-id="3d891-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d891-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d891-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3d891-124">Accept</span></span>|<span data-ttu-id="3d891-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3d891-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d891-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d891-126">Request body</span></span>
<span data-ttu-id="3d891-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) .</span><span class="sxs-lookup"><span data-stu-id="3d891-127">In the request body, supply a JSON representation for the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

<span data-ttu-id="3d891-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md).</span><span class="sxs-lookup"><span data-stu-id="3d891-128">The following table shows the properties that are required when you create the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md).</span></span>

|<span data-ttu-id="3d891-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d891-129">Property</span></span>|<span data-ttu-id="3d891-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d891-130">Type</span></span>|<span data-ttu-id="3d891-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d891-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d891-132">id</span><span class="sxs-lookup"><span data-stu-id="3d891-132">id</span></span>|<span data-ttu-id="3d891-133">String</span><span class="sxs-lookup"><span data-stu-id="3d891-133">String</span></span>|<span data-ttu-id="3d891-134">Identificador exclusivo para esta entidade</span><span class="sxs-lookup"><span data-stu-id="3d891-134">Unique identifier for this entity</span></span>|



## <a name="response"></a><span data-ttu-id="3d891-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d891-135">Response</span></span>
<span data-ttu-id="3d891-136">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d891-136">If successful, this method returns a `200 OK` response code and an updated [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d891-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d891-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d891-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d891-138">Request</span></span>
<span data-ttu-id="3d891-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d891-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.deviceManagementReports"
}
```

### <a name="response"></a><span data-ttu-id="3d891-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d891-140">Response</span></span>
<span data-ttu-id="3d891-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3d891-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "d6a697d3-97d3-d6a6-d397-a6d6d397a6d6"
}
```




