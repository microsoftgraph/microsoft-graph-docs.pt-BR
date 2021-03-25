---
title: Criar deviceManagementExportJob
description: Crie um novo objeto deviceManagementExportJob.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a126023796b92d8158d7875913efff9be6cf9695
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158455"
---
# <a name="create-devicemanagementexportjob"></a><span data-ttu-id="42cc3-103">Criar deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="42cc3-103">Create deviceManagementExportJob</span></span>

<span data-ttu-id="42cc3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42cc3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42cc3-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="42cc3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42cc3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="42cc3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42cc3-107">Crie um novo [objeto deviceManagementExportJob.](../resources/intune-reporting-devicemanagementexportjob.md)</span><span class="sxs-lookup"><span data-stu-id="42cc3-107">Create a new [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42cc3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="42cc3-108">Prerequisites</span></span>
<span data-ttu-id="42cc3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42cc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42cc3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42cc3-111">Permission type</span></span>|<span data-ttu-id="42cc3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42cc3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42cc3-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42cc3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42cc3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42cc3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="42cc3-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42cc3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42cc3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42cc3-116">Not supported.</span></span>|
|<span data-ttu-id="42cc3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42cc3-117">Application</span></span>|<span data-ttu-id="42cc3-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42cc3-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42cc3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42cc3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/exportJobs
```

## <a name="request-headers"></a><span data-ttu-id="42cc3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42cc3-120">Request headers</span></span>
|<span data-ttu-id="42cc3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="42cc3-121">Header</span></span>|<span data-ttu-id="42cc3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="42cc3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42cc3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="42cc3-123">Authorization</span></span>|<span data-ttu-id="42cc3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42cc3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42cc3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="42cc3-125">Accept</span></span>|<span data-ttu-id="42cc3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="42cc3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42cc3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42cc3-127">Request body</span></span>
<span data-ttu-id="42cc3-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementExportJob.</span><span class="sxs-lookup"><span data-stu-id="42cc3-128">In the request body, supply a JSON representation for the deviceManagementExportJob object.</span></span>

<span data-ttu-id="42cc3-129">A tabela a seguir mostra as propriedades necessárias ao criar deviceManagementExportJob.</span><span class="sxs-lookup"><span data-stu-id="42cc3-129">The following table shows the properties that are required when you create the deviceManagementExportJob.</span></span>

|<span data-ttu-id="42cc3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42cc3-130">Property</span></span>|<span data-ttu-id="42cc3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="42cc3-131">Type</span></span>|<span data-ttu-id="42cc3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="42cc3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42cc3-133">id</span><span class="sxs-lookup"><span data-stu-id="42cc3-133">id</span></span>|<span data-ttu-id="42cc3-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42cc3-134">String</span></span>|<span data-ttu-id="42cc3-135">Identificador exclusivo dessa entidade</span><span class="sxs-lookup"><span data-stu-id="42cc3-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="42cc3-136">reportName</span><span class="sxs-lookup"><span data-stu-id="42cc3-136">reportName</span></span>|<span data-ttu-id="42cc3-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42cc3-137">String</span></span>|<span data-ttu-id="42cc3-138">Nome do relatório</span><span class="sxs-lookup"><span data-stu-id="42cc3-138">Name of the report</span></span>|
|<span data-ttu-id="42cc3-139">filter</span><span class="sxs-lookup"><span data-stu-id="42cc3-139">filter</span></span>|<span data-ttu-id="42cc3-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42cc3-140">String</span></span>|<span data-ttu-id="42cc3-141">Filtros aplicados no relatório</span><span class="sxs-lookup"><span data-stu-id="42cc3-141">Filters applied on the report</span></span>|
|<span data-ttu-id="42cc3-142">select</span><span class="sxs-lookup"><span data-stu-id="42cc3-142">select</span></span>|<span data-ttu-id="42cc3-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="42cc3-143">String collection</span></span>|<span data-ttu-id="42cc3-144">Colunas selecionadas no relatório</span><span class="sxs-lookup"><span data-stu-id="42cc3-144">Columns selected from the report</span></span>|
|<span data-ttu-id="42cc3-145">formato</span><span class="sxs-lookup"><span data-stu-id="42cc3-145">format</span></span>|[<span data-ttu-id="42cc3-146">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="42cc3-146">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="42cc3-147">Formato do relatório exportado.</span><span class="sxs-lookup"><span data-stu-id="42cc3-147">Format of the exported report.</span></span> <span data-ttu-id="42cc3-148">Os valores possíveis são: `csv` e `pdf`.</span><span class="sxs-lookup"><span data-stu-id="42cc3-148">Possible values are: `csv`, `pdf`.</span></span>|
|<span data-ttu-id="42cc3-149">snapshotId</span><span class="sxs-lookup"><span data-stu-id="42cc3-149">snapshotId</span></span>|<span data-ttu-id="42cc3-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42cc3-150">String</span></span>|<span data-ttu-id="42cc3-151">Um instantâneo é um subconjunto identificável do conjuntos de dados representado pelo ReportName.</span><span class="sxs-lookup"><span data-stu-id="42cc3-151">A snapshot is an identifiable subset of the dataset represented by the ReportName.</span></span> <span data-ttu-id="42cc3-152">Uma id sessionId ou CachedReportConfiguration pode ser usada aqui.</span><span class="sxs-lookup"><span data-stu-id="42cc3-152">A sessionId or CachedReportConfiguration id can be used here.</span></span> <span data-ttu-id="42cc3-153">Se uma sessionId for especificada, Filter, Select e OrderBy serão aplicados aos dados representados pela sessionId.</span><span class="sxs-lookup"><span data-stu-id="42cc3-153">If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId.</span></span> <span data-ttu-id="42cc3-154">Filter, Select e OrderBy não podem ser especificados juntamente com uma id CachedReportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="42cc3-154">Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.</span></span>|
|<span data-ttu-id="42cc3-155">localizationType</span><span class="sxs-lookup"><span data-stu-id="42cc3-155">localizationType</span></span>|[<span data-ttu-id="42cc3-156">deviceManagementExportJobLocalizationType</span><span class="sxs-lookup"><span data-stu-id="42cc3-156">deviceManagementExportJobLocalizationType</span></span>](../resources/intune-reporting-devicemanagementexportjoblocalizationtype.md)|<span data-ttu-id="42cc3-157">Configura como o trabalho de exportação solicitado é localizado.</span><span class="sxs-lookup"><span data-stu-id="42cc3-157">Configures how the requested export job is localized.</span></span> <span data-ttu-id="42cc3-158">Os valores possíveis são: `localizedValuesAsAdditionalColumn` e `replaceLocalizableValues`.</span><span class="sxs-lookup"><span data-stu-id="42cc3-158">Possible values are: `localizedValuesAsAdditionalColumn`, `replaceLocalizableValues`.</span></span>|
|<span data-ttu-id="42cc3-159">status</span><span class="sxs-lookup"><span data-stu-id="42cc3-159">status</span></span>|[<span data-ttu-id="42cc3-160">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="42cc3-160">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="42cc3-161">Status do trabalho de exportação.</span><span class="sxs-lookup"><span data-stu-id="42cc3-161">Status of the export job.</span></span> <span data-ttu-id="42cc3-162">Os valores possíveis são: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="42cc3-162">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="42cc3-163">url</span><span class="sxs-lookup"><span data-stu-id="42cc3-163">url</span></span>|<span data-ttu-id="42cc3-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42cc3-164">String</span></span>|<span data-ttu-id="42cc3-165">Local temporário do relatório exportado</span><span class="sxs-lookup"><span data-stu-id="42cc3-165">Temporary location of the exported report</span></span>|
|<span data-ttu-id="42cc3-166">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="42cc3-166">requestDateTime</span></span>|<span data-ttu-id="42cc3-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42cc3-167">DateTimeOffset</span></span>|<span data-ttu-id="42cc3-168">Hora em que o relatório exportado foi solicitado</span><span class="sxs-lookup"><span data-stu-id="42cc3-168">Time that the exported report was requested</span></span>|
|<span data-ttu-id="42cc3-169">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="42cc3-169">expirationDateTime</span></span>|<span data-ttu-id="42cc3-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42cc3-170">DateTimeOffset</span></span>|<span data-ttu-id="42cc3-171">Tempo em que o relatório exportado expira</span><span class="sxs-lookup"><span data-stu-id="42cc3-171">Time that the exported report expires</span></span>|



## <a name="response"></a><span data-ttu-id="42cc3-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="42cc3-172">Response</span></span>
<span data-ttu-id="42cc3-173">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42cc3-173">If successful, this method returns a `201 Created` response code and a [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42cc3-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42cc3-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="42cc3-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42cc3-175">Request</span></span>
<span data-ttu-id="42cc3-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42cc3-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/exportJobs
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

### <a name="response"></a><span data-ttu-id="42cc3-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="42cc3-177">Response</span></span>
<span data-ttu-id="42cc3-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42cc3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




