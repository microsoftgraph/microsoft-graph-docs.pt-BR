---
title: Atualizar deviceManagementExportJob
description: Atualiza as propriedades de um objeto deviceManagementExportJob.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2609727b57fb4242169d135e3eb7a205db10ef03
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43454400"
---
# <a name="update-devicemanagementexportjob"></a><span data-ttu-id="1d438-103">Atualizar deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="1d438-103">Update deviceManagementExportJob</span></span>

<span data-ttu-id="1d438-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d438-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d438-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1d438-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d438-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1d438-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d438-107">Atualiza as propriedades de um objeto [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) .</span><span class="sxs-lookup"><span data-stu-id="1d438-107">Update the properties of a [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d438-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1d438-108">Prerequisites</span></span>
<span data-ttu-id="1d438-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d438-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d438-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d438-111">Permission type</span></span>|<span data-ttu-id="1d438-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1d438-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d438-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d438-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1d438-114">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1d438-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1d438-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d438-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d438-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d438-116">Not supported.</span></span>|
|<span data-ttu-id="1d438-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d438-117">Application</span></span>|<span data-ttu-id="1d438-118">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1d438-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d438-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d438-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
```

## <a name="request-headers"></a><span data-ttu-id="1d438-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d438-120">Request headers</span></span>
|<span data-ttu-id="1d438-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1d438-121">Header</span></span>|<span data-ttu-id="1d438-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1d438-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d438-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d438-123">Authorization</span></span>|<span data-ttu-id="1d438-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d438-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d438-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1d438-125">Accept</span></span>|<span data-ttu-id="1d438-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1d438-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d438-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d438-127">Request body</span></span>
<span data-ttu-id="1d438-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) .</span><span class="sxs-lookup"><span data-stu-id="1d438-128">In the request body, supply a JSON representation for the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

<span data-ttu-id="1d438-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md).</span><span class="sxs-lookup"><span data-stu-id="1d438-129">The following table shows the properties that are required when you create the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md).</span></span>

|<span data-ttu-id="1d438-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d438-130">Property</span></span>|<span data-ttu-id="1d438-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d438-131">Type</span></span>|<span data-ttu-id="1d438-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d438-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d438-133">id</span><span class="sxs-lookup"><span data-stu-id="1d438-133">id</span></span>|<span data-ttu-id="1d438-134">String</span><span class="sxs-lookup"><span data-stu-id="1d438-134">String</span></span>|<span data-ttu-id="1d438-135">Identificador exclusivo para esta entidade</span><span class="sxs-lookup"><span data-stu-id="1d438-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="1d438-136">reportName</span><span class="sxs-lookup"><span data-stu-id="1d438-136">reportName</span></span>|<span data-ttu-id="1d438-137">String</span><span class="sxs-lookup"><span data-stu-id="1d438-137">String</span></span>|<span data-ttu-id="1d438-138">Nome do relatório</span><span class="sxs-lookup"><span data-stu-id="1d438-138">Name of the report</span></span>|
|<span data-ttu-id="1d438-139">filter</span><span class="sxs-lookup"><span data-stu-id="1d438-139">filter</span></span>|<span data-ttu-id="1d438-140">String</span><span class="sxs-lookup"><span data-stu-id="1d438-140">String</span></span>|<span data-ttu-id="1d438-141">Filtros aplicados no relatório</span><span class="sxs-lookup"><span data-stu-id="1d438-141">Filters applied on the report</span></span>|
|<span data-ttu-id="1d438-142">select</span><span class="sxs-lookup"><span data-stu-id="1d438-142">select</span></span>|<span data-ttu-id="1d438-143">Coleção String</span><span class="sxs-lookup"><span data-stu-id="1d438-143">String collection</span></span>|<span data-ttu-id="1d438-144">Colunas selecionadas do relatório</span><span class="sxs-lookup"><span data-stu-id="1d438-144">Columns selected from the report</span></span>|
|<span data-ttu-id="1d438-145">formato</span><span class="sxs-lookup"><span data-stu-id="1d438-145">format</span></span>|[<span data-ttu-id="1d438-146">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="1d438-146">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="1d438-147">Formato do relatório exportado.</span><span class="sxs-lookup"><span data-stu-id="1d438-147">Format of the exported report.</span></span> <span data-ttu-id="1d438-148">Os valores possíveis são: `csv` e `pdf`.</span><span class="sxs-lookup"><span data-stu-id="1d438-148">Possible values are: `csv`, `pdf`.</span></span>|
|<span data-ttu-id="1d438-149">instantâneoid</span><span class="sxs-lookup"><span data-stu-id="1d438-149">snapshotId</span></span>|<span data-ttu-id="1d438-150">String</span><span class="sxs-lookup"><span data-stu-id="1d438-150">String</span></span>|<span data-ttu-id="1d438-151">Um instantâneo é um subconjunto identificável do DataSet representado pelo ReportName.</span><span class="sxs-lookup"><span data-stu-id="1d438-151">A snapshot is an identifiable subset of the dataset represented by the ReportName.</span></span> <span data-ttu-id="1d438-152">Uma ID de Identificação_da_sessão ou CachedReportConfiguration pode ser usada aqui.</span><span class="sxs-lookup"><span data-stu-id="1d438-152">A sessionId or CachedReportConfiguration id can be used here.</span></span> <span data-ttu-id="1d438-153">Se uma Identificação_da_sessão for especificada, Filter, Select e OrderBy serão aplicadas aos dados representados pela Identificação_da_sessão.</span><span class="sxs-lookup"><span data-stu-id="1d438-153">If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId.</span></span> <span data-ttu-id="1d438-154">Filter, Select e OrderBy não podem ser especificados junto com uma ID CachedReportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1d438-154">Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.</span></span>|
|<span data-ttu-id="1d438-155">status</span><span class="sxs-lookup"><span data-stu-id="1d438-155">status</span></span>|[<span data-ttu-id="1d438-156">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="1d438-156">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="1d438-157">Status do trabalho de exportação.</span><span class="sxs-lookup"><span data-stu-id="1d438-157">Status of the export job.</span></span> <span data-ttu-id="1d438-158">Os valores possíveis são: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="1d438-158">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="1d438-159">url</span><span class="sxs-lookup"><span data-stu-id="1d438-159">url</span></span>|<span data-ttu-id="1d438-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d438-160">String</span></span>|<span data-ttu-id="1d438-161">Local temporário do relatório exportado</span><span class="sxs-lookup"><span data-stu-id="1d438-161">Temporary location of the exported report</span></span>|
|<span data-ttu-id="1d438-162">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="1d438-162">requestDateTime</span></span>|<span data-ttu-id="1d438-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d438-163">DateTimeOffset</span></span>|<span data-ttu-id="1d438-164">Hora em que o relatório exportado foi solicitado</span><span class="sxs-lookup"><span data-stu-id="1d438-164">Time that the exported report was requested</span></span>|
|<span data-ttu-id="1d438-165">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1d438-165">expirationDateTime</span></span>|<span data-ttu-id="1d438-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d438-166">DateTimeOffset</span></span>|<span data-ttu-id="1d438-167">Hora em que o relatório exportado expira</span><span class="sxs-lookup"><span data-stu-id="1d438-167">Time that the exported report expires</span></span>|



## <a name="response"></a><span data-ttu-id="1d438-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d438-168">Response</span></span>
<span data-ttu-id="1d438-169">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d438-169">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d438-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d438-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d438-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d438-171">Request</span></span>
<span data-ttu-id="1d438-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d438-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
Content-type: application/json
Content-length: 404

{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "format": "pdf",
  "snapshotId": "Snapshot Id value",
  "status": "notStarted",
  "url": "Url value",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```

### <a name="response"></a><span data-ttu-id="1d438-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d438-173">Response</span></span>
<span data-ttu-id="1d438-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1d438-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 453

{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "id": "9ddfb995-b995-9ddf-95b9-df9d95b9df9d",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "format": "pdf",
  "snapshotId": "Snapshot Id value",
  "status": "notStarted",
  "url": "Url value",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```



