---
title: Criar deviceManagementExportJob
description: Crie um novo objeto deviceManagementExportJob.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9adcc417a208a42eb075103c6f1fe17ebb00e7dd
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755187"
---
# <a name="create-devicemanagementexportjob"></a><span data-ttu-id="77f4b-103">Criar deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="77f4b-103">Create deviceManagementExportJob</span></span>

<span data-ttu-id="77f4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77f4b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77f4b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="77f4b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77f4b-106">Crie um novo [objeto deviceManagementExportJob.](../resources/intune-reporting-devicemanagementexportjob.md)</span><span class="sxs-lookup"><span data-stu-id="77f4b-106">Create a new [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77f4b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="77f4b-107">Prerequisites</span></span>
<span data-ttu-id="77f4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77f4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77f4b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77f4b-110">Permission type</span></span>|<span data-ttu-id="77f4b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77f4b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77f4b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77f4b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="77f4b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77f4b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="77f4b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77f4b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77f4b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77f4b-115">Not supported.</span></span>|
|<span data-ttu-id="77f4b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77f4b-116">Application</span></span>|<span data-ttu-id="77f4b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77f4b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77f4b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77f4b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/exportJobs
```

## <a name="request-headers"></a><span data-ttu-id="77f4b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77f4b-119">Request headers</span></span>
|<span data-ttu-id="77f4b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="77f4b-120">Header</span></span>|<span data-ttu-id="77f4b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="77f4b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77f4b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="77f4b-122">Authorization</span></span>|<span data-ttu-id="77f4b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77f4b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77f4b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="77f4b-124">Accept</span></span>|<span data-ttu-id="77f4b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="77f4b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77f4b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77f4b-126">Request body</span></span>
<span data-ttu-id="77f4b-127">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementExportJob.</span><span class="sxs-lookup"><span data-stu-id="77f4b-127">In the request body, supply a JSON representation for the deviceManagementExportJob object.</span></span>

<span data-ttu-id="77f4b-128">A tabela a seguir mostra as propriedades necessárias ao criar deviceManagementExportJob.</span><span class="sxs-lookup"><span data-stu-id="77f4b-128">The following table shows the properties that are required when you create the deviceManagementExportJob.</span></span>

|<span data-ttu-id="77f4b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77f4b-129">Property</span></span>|<span data-ttu-id="77f4b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="77f4b-130">Type</span></span>|<span data-ttu-id="77f4b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="77f4b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77f4b-132">id</span><span class="sxs-lookup"><span data-stu-id="77f4b-132">id</span></span>|<span data-ttu-id="77f4b-133">String</span><span class="sxs-lookup"><span data-stu-id="77f4b-133">String</span></span>|<span data-ttu-id="77f4b-134">Identificador exclusivo dessa entidade</span><span class="sxs-lookup"><span data-stu-id="77f4b-134">Unique identifier for this entity</span></span>|
|<span data-ttu-id="77f4b-135">reportName</span><span class="sxs-lookup"><span data-stu-id="77f4b-135">reportName</span></span>|<span data-ttu-id="77f4b-136">String</span><span class="sxs-lookup"><span data-stu-id="77f4b-136">String</span></span>|<span data-ttu-id="77f4b-137">Nome do relatório</span><span class="sxs-lookup"><span data-stu-id="77f4b-137">Name of the report</span></span>|
|<span data-ttu-id="77f4b-138">filter</span><span class="sxs-lookup"><span data-stu-id="77f4b-138">filter</span></span>|<span data-ttu-id="77f4b-139">String</span><span class="sxs-lookup"><span data-stu-id="77f4b-139">String</span></span>|<span data-ttu-id="77f4b-140">Filtros aplicados no relatório</span><span class="sxs-lookup"><span data-stu-id="77f4b-140">Filters applied on the report</span></span>|
|<span data-ttu-id="77f4b-141">select</span><span class="sxs-lookup"><span data-stu-id="77f4b-141">select</span></span>|<span data-ttu-id="77f4b-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="77f4b-142">String collection</span></span>|<span data-ttu-id="77f4b-143">Colunas selecionadas no relatório</span><span class="sxs-lookup"><span data-stu-id="77f4b-143">Columns selected from the report</span></span>|
|<span data-ttu-id="77f4b-144">formato</span><span class="sxs-lookup"><span data-stu-id="77f4b-144">format</span></span>|[<span data-ttu-id="77f4b-145">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="77f4b-145">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="77f4b-146">Formato do relatório exportado.</span><span class="sxs-lookup"><span data-stu-id="77f4b-146">Format of the exported report.</span></span> <span data-ttu-id="77f4b-147">Os valores possíveis são: `csv` e `pdf`.</span><span class="sxs-lookup"><span data-stu-id="77f4b-147">Possible values are: `csv`, `pdf`.</span></span>|
|<span data-ttu-id="77f4b-148">snapshotId</span><span class="sxs-lookup"><span data-stu-id="77f4b-148">snapshotId</span></span>|<span data-ttu-id="77f4b-149">String</span><span class="sxs-lookup"><span data-stu-id="77f4b-149">String</span></span>|<span data-ttu-id="77f4b-150">Um instantâneo é um subconjunto identificável do conjuntos de dados representado pelo ReportName.</span><span class="sxs-lookup"><span data-stu-id="77f4b-150">A snapshot is an identifiable subset of the dataset represented by the ReportName.</span></span> <span data-ttu-id="77f4b-151">Uma id sessionId ou CachedReportConfiguration pode ser usada aqui.</span><span class="sxs-lookup"><span data-stu-id="77f4b-151">A sessionId or CachedReportConfiguration id can be used here.</span></span> <span data-ttu-id="77f4b-152">Se uma sessionId for especificada, Filter, Select e OrderBy serão aplicados aos dados representados pela sessionId.</span><span class="sxs-lookup"><span data-stu-id="77f4b-152">If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId.</span></span> <span data-ttu-id="77f4b-153">Filter, Select e OrderBy não podem ser especificados juntamente com uma id CachedReportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="77f4b-153">Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.</span></span>|
|<span data-ttu-id="77f4b-154">localizationType</span><span class="sxs-lookup"><span data-stu-id="77f4b-154">localizationType</span></span>|[<span data-ttu-id="77f4b-155">deviceManagementExportJobLocalizationType</span><span class="sxs-lookup"><span data-stu-id="77f4b-155">deviceManagementExportJobLocalizationType</span></span>](../resources/intune-reporting-devicemanagementexportjoblocalizationtype.md)|<span data-ttu-id="77f4b-156">Configura como o trabalho de exportação solicitado é localizado.</span><span class="sxs-lookup"><span data-stu-id="77f4b-156">Configures how the requested export job is localized.</span></span> <span data-ttu-id="77f4b-157">Os valores possíveis são: `localizedValuesAsAdditionalColumn` e `replaceLocalizableValues`.</span><span class="sxs-lookup"><span data-stu-id="77f4b-157">Possible values are: `localizedValuesAsAdditionalColumn`, `replaceLocalizableValues`.</span></span>|
|<span data-ttu-id="77f4b-158">status</span><span class="sxs-lookup"><span data-stu-id="77f4b-158">status</span></span>|[<span data-ttu-id="77f4b-159">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="77f4b-159">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="77f4b-160">Status do trabalho de exportação.</span><span class="sxs-lookup"><span data-stu-id="77f4b-160">Status of the export job.</span></span> <span data-ttu-id="77f4b-161">Os valores possíveis são: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="77f4b-161">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="77f4b-162">url</span><span class="sxs-lookup"><span data-stu-id="77f4b-162">url</span></span>|<span data-ttu-id="77f4b-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77f4b-163">String</span></span>|<span data-ttu-id="77f4b-164">Local temporário do relatório exportado</span><span class="sxs-lookup"><span data-stu-id="77f4b-164">Temporary location of the exported report</span></span>|
|<span data-ttu-id="77f4b-165">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="77f4b-165">requestDateTime</span></span>|<span data-ttu-id="77f4b-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77f4b-166">DateTimeOffset</span></span>|<span data-ttu-id="77f4b-167">Hora em que o relatório exportado foi solicitado</span><span class="sxs-lookup"><span data-stu-id="77f4b-167">Time that the exported report was requested</span></span>|
|<span data-ttu-id="77f4b-168">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="77f4b-168">expirationDateTime</span></span>|<span data-ttu-id="77f4b-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77f4b-169">DateTimeOffset</span></span>|<span data-ttu-id="77f4b-170">Tempo em que o relatório exportado expira</span><span class="sxs-lookup"><span data-stu-id="77f4b-170">Time that the exported report expires</span></span>|



## <a name="response"></a><span data-ttu-id="77f4b-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="77f4b-171">Response</span></span>
<span data-ttu-id="77f4b-172">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77f4b-172">If successful, this method returns a `201 Created` response code and a [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77f4b-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77f4b-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="77f4b-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77f4b-174">Request</span></span>
<span data-ttu-id="77f4b-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77f4b-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/reports/exportJobs
Content-type: application/json
Content-length: 455

{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "format": "pdf",
  "snapshotId": "Snapshot Id value",
  "localizationType": "replaceLocalizableValues",
  "status": "notStarted",
  "url": "Url value",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```

### <a name="response"></a><span data-ttu-id="77f4b-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="77f4b-176">Response</span></span>
<span data-ttu-id="77f4b-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77f4b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 504

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
  "localizationType": "replaceLocalizableValues",
  "status": "notStarted",
  "url": "Url value",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```




