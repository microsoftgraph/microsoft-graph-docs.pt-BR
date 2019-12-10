---
title: Criar deviceManagementExportJob
description: Criar um novo objeto deviceManagementExportJob.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a1552a722a5dd33c987ea137ed1be42675074a49
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940345"
---
# <a name="create-devicemanagementexportjob"></a><span data-ttu-id="35694-103">Criar deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="35694-103">Create deviceManagementExportJob</span></span>

> <span data-ttu-id="35694-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="35694-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35694-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="35694-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35694-106">Criar um novo objeto [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) .</span><span class="sxs-lookup"><span data-stu-id="35694-106">Create a new [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35694-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="35694-107">Prerequisites</span></span>
<span data-ttu-id="35694-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35694-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35694-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35694-110">Permission type</span></span>|<span data-ttu-id="35694-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="35694-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35694-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35694-112">Delegated (work or school account)</span></span>|<span data-ttu-id="35694-113">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="35694-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="35694-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35694-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35694-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35694-115">Not supported.</span></span>|
|<span data-ttu-id="35694-116">Application</span><span class="sxs-lookup"><span data-stu-id="35694-116">Application</span></span>|<span data-ttu-id="35694-117">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="35694-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="35694-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35694-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/exportJobs
```

## <a name="request-headers"></a><span data-ttu-id="35694-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35694-119">Request headers</span></span>
|<span data-ttu-id="35694-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="35694-120">Header</span></span>|<span data-ttu-id="35694-121">Valor</span><span class="sxs-lookup"><span data-stu-id="35694-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35694-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="35694-122">Authorization</span></span>|<span data-ttu-id="35694-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35694-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35694-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="35694-124">Accept</span></span>|<span data-ttu-id="35694-125">application/json</span><span class="sxs-lookup"><span data-stu-id="35694-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35694-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35694-126">Request body</span></span>
<span data-ttu-id="35694-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementExportJob.</span><span class="sxs-lookup"><span data-stu-id="35694-127">In the request body, supply a JSON representation for the deviceManagementExportJob object.</span></span>

<span data-ttu-id="35694-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementExportJob.</span><span class="sxs-lookup"><span data-stu-id="35694-128">The following table shows the properties that are required when you create the deviceManagementExportJob.</span></span>

|<span data-ttu-id="35694-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35694-129">Property</span></span>|<span data-ttu-id="35694-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="35694-130">Type</span></span>|<span data-ttu-id="35694-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="35694-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35694-132">id</span><span class="sxs-lookup"><span data-stu-id="35694-132">id</span></span>|<span data-ttu-id="35694-133">String</span><span class="sxs-lookup"><span data-stu-id="35694-133">String</span></span>|<span data-ttu-id="35694-134">Identificador exclusivo para esta entidade</span><span class="sxs-lookup"><span data-stu-id="35694-134">Unique identifier for this entity</span></span>|
|<span data-ttu-id="35694-135">reportName</span><span class="sxs-lookup"><span data-stu-id="35694-135">reportName</span></span>|<span data-ttu-id="35694-136">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="35694-136">String</span></span>|<span data-ttu-id="35694-137">Nome do relatório</span><span class="sxs-lookup"><span data-stu-id="35694-137">Name of the report</span></span>|
|<span data-ttu-id="35694-138">filter</span><span class="sxs-lookup"><span data-stu-id="35694-138">filter</span></span>|<span data-ttu-id="35694-139">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="35694-139">String</span></span>|<span data-ttu-id="35694-140">Filtros aplicados no relatório</span><span class="sxs-lookup"><span data-stu-id="35694-140">Filters applied on the report</span></span>|
|<span data-ttu-id="35694-141">select</span><span class="sxs-lookup"><span data-stu-id="35694-141">select</span></span>|<span data-ttu-id="35694-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="35694-142">String collection</span></span>|<span data-ttu-id="35694-143">Colunas selecionadas do relatório</span><span class="sxs-lookup"><span data-stu-id="35694-143">Columns selected from the report</span></span>|
|<span data-ttu-id="35694-144">formato</span><span class="sxs-lookup"><span data-stu-id="35694-144">format</span></span>|[<span data-ttu-id="35694-145">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="35694-145">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="35694-146">Formato do relatório exportado.</span><span class="sxs-lookup"><span data-stu-id="35694-146">Format of the exported report.</span></span> <span data-ttu-id="35694-147">Os valores possíveis são: `csv` e `pdf`.</span><span class="sxs-lookup"><span data-stu-id="35694-147">Possible values are: `csv`, `pdf`.</span></span>|
|<span data-ttu-id="35694-148">instantâneoid</span><span class="sxs-lookup"><span data-stu-id="35694-148">snapshotId</span></span>|<span data-ttu-id="35694-149">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="35694-149">String</span></span>|<span data-ttu-id="35694-150">Um instantâneo é um subconjunto identificável do DataSet representado pelo ReportName.</span><span class="sxs-lookup"><span data-stu-id="35694-150">A snapshot is an identifiable subset of the dataset represented by the ReportName.</span></span> <span data-ttu-id="35694-151">Uma ID de Identificação_da_sessão ou CachedReportConfiguration pode ser usada aqui.</span><span class="sxs-lookup"><span data-stu-id="35694-151">A sessionId or CachedReportConfiguration id can be used here.</span></span> <span data-ttu-id="35694-152">Se uma Identificação_da_sessão for especificada, Filter, Select e OrderBy serão aplicadas aos dados representados pela Identificação_da_sessão.</span><span class="sxs-lookup"><span data-stu-id="35694-152">If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId.</span></span> <span data-ttu-id="35694-153">Filter, Select e OrderBy não podem ser especificados junto com uma ID CachedReportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="35694-153">Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.</span></span>|
|<span data-ttu-id="35694-154">status</span><span class="sxs-lookup"><span data-stu-id="35694-154">status</span></span>|[<span data-ttu-id="35694-155">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="35694-155">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="35694-156">Status do trabalho de exportação.</span><span class="sxs-lookup"><span data-stu-id="35694-156">Status of the export job.</span></span> <span data-ttu-id="35694-157">Os valores possíveis são: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="35694-157">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="35694-158">url</span><span class="sxs-lookup"><span data-stu-id="35694-158">url</span></span>|<span data-ttu-id="35694-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35694-159">String</span></span>|<span data-ttu-id="35694-160">Local temporário do relatório exportado</span><span class="sxs-lookup"><span data-stu-id="35694-160">Temporary location of the exported report</span></span>|
|<span data-ttu-id="35694-161">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="35694-161">requestDateTime</span></span>|<span data-ttu-id="35694-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35694-162">DateTimeOffset</span></span>|<span data-ttu-id="35694-163">Hora em que o relatório exportado foi solicitado</span><span class="sxs-lookup"><span data-stu-id="35694-163">Time that the exported report was requested</span></span>|
|<span data-ttu-id="35694-164">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="35694-164">expirationDateTime</span></span>|<span data-ttu-id="35694-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35694-165">DateTimeOffset</span></span>|<span data-ttu-id="35694-166">Hora em que o relatório exportado expira</span><span class="sxs-lookup"><span data-stu-id="35694-166">Time that the exported report expires</span></span>|



## <a name="response"></a><span data-ttu-id="35694-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="35694-167">Response</span></span>
<span data-ttu-id="35694-168">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35694-168">If successful, this method returns a `201 Created` response code and a [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35694-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35694-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="35694-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35694-170">Request</span></span>
<span data-ttu-id="35694-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="35694-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/exportJobs
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

### <a name="response"></a><span data-ttu-id="35694-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="35694-172">Response</span></span>
<span data-ttu-id="35694-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="35694-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





