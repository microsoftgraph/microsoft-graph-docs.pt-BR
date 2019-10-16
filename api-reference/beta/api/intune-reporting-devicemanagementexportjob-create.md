---
title: Criar deviceManagementExportJob
description: Criar um novo objeto deviceManagementExportJob.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2d5ccb6a7c1ea97aa93c88df887156668dcd48a1
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537279"
---
# <a name="create-devicemanagementexportjob"></a><span data-ttu-id="80dcf-103">Criar deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="80dcf-103">Create deviceManagementExportJob</span></span>

> <span data-ttu-id="80dcf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="80dcf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80dcf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="80dcf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80dcf-106">Criar um novo objeto [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) .</span><span class="sxs-lookup"><span data-stu-id="80dcf-106">Create a new [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80dcf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="80dcf-107">Prerequisites</span></span>
<span data-ttu-id="80dcf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80dcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80dcf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80dcf-110">Permission type</span></span>|<span data-ttu-id="80dcf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="80dcf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80dcf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80dcf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="80dcf-113">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="80dcf-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="80dcf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80dcf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80dcf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80dcf-115">Not supported.</span></span>|
|<span data-ttu-id="80dcf-116">Application</span><span class="sxs-lookup"><span data-stu-id="80dcf-116">Application</span></span>|<span data-ttu-id="80dcf-117">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="80dcf-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="80dcf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80dcf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/exportJobs
```

## <a name="request-headers"></a><span data-ttu-id="80dcf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80dcf-119">Request headers</span></span>
|<span data-ttu-id="80dcf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="80dcf-120">Header</span></span>|<span data-ttu-id="80dcf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="80dcf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80dcf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="80dcf-122">Authorization</span></span>|<span data-ttu-id="80dcf-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80dcf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80dcf-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="80dcf-124">Accept</span></span>|<span data-ttu-id="80dcf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="80dcf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80dcf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80dcf-126">Request body</span></span>
<span data-ttu-id="80dcf-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementExportJob.</span><span class="sxs-lookup"><span data-stu-id="80dcf-127">In the request body, supply a JSON representation for the deviceManagementExportJob object.</span></span>

<span data-ttu-id="80dcf-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementExportJob.</span><span class="sxs-lookup"><span data-stu-id="80dcf-128">The following table shows the properties that are required when you create the deviceManagementExportJob.</span></span>

|<span data-ttu-id="80dcf-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80dcf-129">Property</span></span>|<span data-ttu-id="80dcf-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="80dcf-130">Type</span></span>|<span data-ttu-id="80dcf-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="80dcf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80dcf-132">id</span><span class="sxs-lookup"><span data-stu-id="80dcf-132">id</span></span>|<span data-ttu-id="80dcf-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80dcf-133">String</span></span>|<span data-ttu-id="80dcf-134">Identificador exclusivo para esta entidade</span><span class="sxs-lookup"><span data-stu-id="80dcf-134">Unique identifier for this entity</span></span>|
|<span data-ttu-id="80dcf-135">reportName</span><span class="sxs-lookup"><span data-stu-id="80dcf-135">reportName</span></span>|<span data-ttu-id="80dcf-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80dcf-136">String</span></span>|<span data-ttu-id="80dcf-137">Nome do relatório</span><span class="sxs-lookup"><span data-stu-id="80dcf-137">Name of the report</span></span>|
|<span data-ttu-id="80dcf-138">filter</span><span class="sxs-lookup"><span data-stu-id="80dcf-138">filter</span></span>|<span data-ttu-id="80dcf-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80dcf-139">String</span></span>|<span data-ttu-id="80dcf-140">Filtros aplicados no relatório</span><span class="sxs-lookup"><span data-stu-id="80dcf-140">Filters applied on the report</span></span>|
|<span data-ttu-id="80dcf-141">select</span><span class="sxs-lookup"><span data-stu-id="80dcf-141">select</span></span>|<span data-ttu-id="80dcf-142">String collection</span><span class="sxs-lookup"><span data-stu-id="80dcf-142">String collection</span></span>|<span data-ttu-id="80dcf-143">Colunas selecionadas do relatório</span><span class="sxs-lookup"><span data-stu-id="80dcf-143">Columns selected from the report</span></span>|
|<span data-ttu-id="80dcf-144">Classificadoporativado</span><span class="sxs-lookup"><span data-stu-id="80dcf-144">orderBy</span></span>|<span data-ttu-id="80dcf-145">String collection</span><span class="sxs-lookup"><span data-stu-id="80dcf-145">String collection</span></span>|<span data-ttu-id="80dcf-146">Ordenação de colunas no relatório</span><span class="sxs-lookup"><span data-stu-id="80dcf-146">Ordering of columns in the report</span></span>|
|<span data-ttu-id="80dcf-147">formato</span><span class="sxs-lookup"><span data-stu-id="80dcf-147">format</span></span>|[<span data-ttu-id="80dcf-148">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="80dcf-148">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="80dcf-149">Formato do relatório exportado.</span><span class="sxs-lookup"><span data-stu-id="80dcf-149">Format of the exported report.</span></span> <span data-ttu-id="80dcf-150">Os valores possíveis são: `csv` e `pdf`.</span><span class="sxs-lookup"><span data-stu-id="80dcf-150">Possible values are: `csv`, `pdf`.</span></span>|
|<span data-ttu-id="80dcf-151">instantâneoid</span><span class="sxs-lookup"><span data-stu-id="80dcf-151">snapshotId</span></span>|<span data-ttu-id="80dcf-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80dcf-152">String</span></span>|<span data-ttu-id="80dcf-153">Um instantâneo é um subconjunto identificável do DataSet representado pelo ReportName.</span><span class="sxs-lookup"><span data-stu-id="80dcf-153">A snapshot is an identifiable subset of the dataset represented by the ReportName.</span></span> <span data-ttu-id="80dcf-154">Uma ID de Identificação_da_sessão ou CachedReportConfiguration pode ser usada aqui.</span><span class="sxs-lookup"><span data-stu-id="80dcf-154">A sessionId or CachedReportConfiguration id can be used here.</span></span> <span data-ttu-id="80dcf-155">Se uma Identificação_da_sessão for especificada, Filter, Select e OrderBy serão aplicadas aos dados representados pela Identificação_da_sessão.</span><span class="sxs-lookup"><span data-stu-id="80dcf-155">If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId.</span></span> <span data-ttu-id="80dcf-156">Filter, Select e OrderBy não podem ser especificados junto com uma ID CachedReportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="80dcf-156">Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.</span></span>|
|<span data-ttu-id="80dcf-157">status</span><span class="sxs-lookup"><span data-stu-id="80dcf-157">status</span></span>|[<span data-ttu-id="80dcf-158">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="80dcf-158">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="80dcf-159">Status do trabalho de exportação.</span><span class="sxs-lookup"><span data-stu-id="80dcf-159">Status of the export job.</span></span> <span data-ttu-id="80dcf-160">Os valores possíveis são: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="80dcf-160">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="80dcf-161">url</span><span class="sxs-lookup"><span data-stu-id="80dcf-161">url</span></span>|<span data-ttu-id="80dcf-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80dcf-162">String</span></span>|<span data-ttu-id="80dcf-163">Local temporário do relatório exportado</span><span class="sxs-lookup"><span data-stu-id="80dcf-163">Temporary location of the exported report</span></span>|
|<span data-ttu-id="80dcf-164">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="80dcf-164">requestDateTime</span></span>|<span data-ttu-id="80dcf-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80dcf-165">DateTimeOffset</span></span>|<span data-ttu-id="80dcf-166">Hora em que o relatório exportado foi solicitado</span><span class="sxs-lookup"><span data-stu-id="80dcf-166">Time that the exported report was requested</span></span>|
|<span data-ttu-id="80dcf-167">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="80dcf-167">expirationDateTime</span></span>|<span data-ttu-id="80dcf-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80dcf-168">DateTimeOffset</span></span>|<span data-ttu-id="80dcf-169">Hora em que o relatório exportado expira</span><span class="sxs-lookup"><span data-stu-id="80dcf-169">Time that the exported report expires</span></span>|



## <a name="response"></a><span data-ttu-id="80dcf-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="80dcf-170">Response</span></span>
<span data-ttu-id="80dcf-171">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80dcf-171">If successful, this method returns a `201 Created` response code and a [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80dcf-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80dcf-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="80dcf-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80dcf-173">Request</span></span>
<span data-ttu-id="80dcf-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="80dcf-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/exportJobs
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

### <a name="response"></a><span data-ttu-id="80dcf-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="80dcf-175">Response</span></span>
<span data-ttu-id="80dcf-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80dcf-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






