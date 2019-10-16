---
title: Atualizar deviceManagementExportJob
description: Atualiza as propriedades de um objeto deviceManagementExportJob.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4951d458500a0d6863eebed807aa5e2120496376
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537258"
---
# <a name="update-devicemanagementexportjob"></a><span data-ttu-id="bc070-103">Atualizar deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="bc070-103">Update deviceManagementExportJob</span></span>

> <span data-ttu-id="bc070-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bc070-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc070-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bc070-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc070-106">Atualiza as propriedades de um objeto [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) .</span><span class="sxs-lookup"><span data-stu-id="bc070-106">Update the properties of a [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc070-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bc070-107">Prerequisites</span></span>
<span data-ttu-id="bc070-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc070-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc070-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc070-110">Permission type</span></span>|<span data-ttu-id="bc070-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bc070-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc070-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc070-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bc070-113">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bc070-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bc070-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc070-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc070-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc070-115">Not supported.</span></span>|
|<span data-ttu-id="bc070-116">Application</span><span class="sxs-lookup"><span data-stu-id="bc070-116">Application</span></span>|<span data-ttu-id="bc070-117">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bc070-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc070-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc070-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
```

## <a name="request-headers"></a><span data-ttu-id="bc070-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc070-119">Request headers</span></span>
|<span data-ttu-id="bc070-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bc070-120">Header</span></span>|<span data-ttu-id="bc070-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bc070-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc070-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc070-122">Authorization</span></span>|<span data-ttu-id="bc070-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc070-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc070-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bc070-124">Accept</span></span>|<span data-ttu-id="bc070-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bc070-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc070-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc070-126">Request body</span></span>
<span data-ttu-id="bc070-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) .</span><span class="sxs-lookup"><span data-stu-id="bc070-127">In the request body, supply a JSON representation for the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

<span data-ttu-id="bc070-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md).</span><span class="sxs-lookup"><span data-stu-id="bc070-128">The following table shows the properties that are required when you create the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md).</span></span>

|<span data-ttu-id="bc070-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc070-129">Property</span></span>|<span data-ttu-id="bc070-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc070-130">Type</span></span>|<span data-ttu-id="bc070-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc070-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc070-132">id</span><span class="sxs-lookup"><span data-stu-id="bc070-132">id</span></span>|<span data-ttu-id="bc070-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc070-133">String</span></span>|<span data-ttu-id="bc070-134">Identificador exclusivo para esta entidade</span><span class="sxs-lookup"><span data-stu-id="bc070-134">Unique identifier for this entity</span></span>|
|<span data-ttu-id="bc070-135">reportName</span><span class="sxs-lookup"><span data-stu-id="bc070-135">reportName</span></span>|<span data-ttu-id="bc070-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc070-136">String</span></span>|<span data-ttu-id="bc070-137">Nome do relatório</span><span class="sxs-lookup"><span data-stu-id="bc070-137">Name of the report</span></span>|
|<span data-ttu-id="bc070-138">filter</span><span class="sxs-lookup"><span data-stu-id="bc070-138">filter</span></span>|<span data-ttu-id="bc070-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc070-139">String</span></span>|<span data-ttu-id="bc070-140">Filtros aplicados no relatório</span><span class="sxs-lookup"><span data-stu-id="bc070-140">Filters applied on the report</span></span>|
|<span data-ttu-id="bc070-141">select</span><span class="sxs-lookup"><span data-stu-id="bc070-141">select</span></span>|<span data-ttu-id="bc070-142">String collection</span><span class="sxs-lookup"><span data-stu-id="bc070-142">String collection</span></span>|<span data-ttu-id="bc070-143">Colunas selecionadas do relatório</span><span class="sxs-lookup"><span data-stu-id="bc070-143">Columns selected from the report</span></span>|
|<span data-ttu-id="bc070-144">Classificadoporativado</span><span class="sxs-lookup"><span data-stu-id="bc070-144">orderBy</span></span>|<span data-ttu-id="bc070-145">String collection</span><span class="sxs-lookup"><span data-stu-id="bc070-145">String collection</span></span>|<span data-ttu-id="bc070-146">Ordenação de colunas no relatório</span><span class="sxs-lookup"><span data-stu-id="bc070-146">Ordering of columns in the report</span></span>|
|<span data-ttu-id="bc070-147">formato</span><span class="sxs-lookup"><span data-stu-id="bc070-147">format</span></span>|[<span data-ttu-id="bc070-148">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="bc070-148">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="bc070-149">Formato do relatório exportado.</span><span class="sxs-lookup"><span data-stu-id="bc070-149">Format of the exported report.</span></span> <span data-ttu-id="bc070-150">Os valores possíveis são: `csv` e `pdf`.</span><span class="sxs-lookup"><span data-stu-id="bc070-150">Possible values are: `csv`, `pdf`.</span></span>|
|<span data-ttu-id="bc070-151">instantâneoid</span><span class="sxs-lookup"><span data-stu-id="bc070-151">snapshotId</span></span>|<span data-ttu-id="bc070-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc070-152">String</span></span>|<span data-ttu-id="bc070-153">Um instantâneo é um subconjunto identificável do DataSet representado pelo ReportName.</span><span class="sxs-lookup"><span data-stu-id="bc070-153">A snapshot is an identifiable subset of the dataset represented by the ReportName.</span></span> <span data-ttu-id="bc070-154">Uma ID de Identificação_da_sessão ou CachedReportConfiguration pode ser usada aqui.</span><span class="sxs-lookup"><span data-stu-id="bc070-154">A sessionId or CachedReportConfiguration id can be used here.</span></span> <span data-ttu-id="bc070-155">Se uma Identificação_da_sessão for especificada, Filter, Select e OrderBy serão aplicadas aos dados representados pela Identificação_da_sessão.</span><span class="sxs-lookup"><span data-stu-id="bc070-155">If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId.</span></span> <span data-ttu-id="bc070-156">Filter, Select e OrderBy não podem ser especificados junto com uma ID CachedReportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="bc070-156">Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.</span></span>|
|<span data-ttu-id="bc070-157">status</span><span class="sxs-lookup"><span data-stu-id="bc070-157">status</span></span>|[<span data-ttu-id="bc070-158">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="bc070-158">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="bc070-159">Status do trabalho de exportação.</span><span class="sxs-lookup"><span data-stu-id="bc070-159">Status of the export job.</span></span> <span data-ttu-id="bc070-160">Os valores possíveis são: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="bc070-160">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="bc070-161">url</span><span class="sxs-lookup"><span data-stu-id="bc070-161">url</span></span>|<span data-ttu-id="bc070-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc070-162">String</span></span>|<span data-ttu-id="bc070-163">Local temporário do relatório exportado</span><span class="sxs-lookup"><span data-stu-id="bc070-163">Temporary location of the exported report</span></span>|
|<span data-ttu-id="bc070-164">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="bc070-164">requestDateTime</span></span>|<span data-ttu-id="bc070-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc070-165">DateTimeOffset</span></span>|<span data-ttu-id="bc070-166">Hora em que o relatório exportado foi solicitado</span><span class="sxs-lookup"><span data-stu-id="bc070-166">Time that the exported report was requested</span></span>|
|<span data-ttu-id="bc070-167">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bc070-167">expirationDateTime</span></span>|<span data-ttu-id="bc070-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc070-168">DateTimeOffset</span></span>|<span data-ttu-id="bc070-169">Hora em que o relatório exportado expira</span><span class="sxs-lookup"><span data-stu-id="bc070-169">Time that the exported report expires</span></span>|



## <a name="response"></a><span data-ttu-id="bc070-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc070-170">Response</span></span>
<span data-ttu-id="bc070-171">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc070-171">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc070-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc070-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc070-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc070-173">Request</span></span>
<span data-ttu-id="bc070-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc070-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
Content-type: application/json
Content-length: 448

{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "format": "pdf",
  "snapshotId": "Snapshot Id value",
  "status": "notStarted",
  "url": "Url value",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```

### <a name="response"></a><span data-ttu-id="bc070-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc070-175">Response</span></span>
<span data-ttu-id="bc070-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc070-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 497

{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "id": "9ddfb995-b995-9ddf-95b9-df9d95b9df9d",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "format": "pdf",
  "snapshotId": "Snapshot Id value",
  "status": "notStarted",
  "url": "Url value",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```






