---
title: Atualizar deviceManagementExportJob
description: Atualize as propriedades de um objeto deviceManagementExportJob.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ff338167a92062d57393228ff5861d04c6420e3b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442379"
---
# <a name="update-devicemanagementexportjob"></a><span data-ttu-id="13d1f-103">Atualizar deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="13d1f-103">Update deviceManagementExportJob</span></span>

<span data-ttu-id="13d1f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13d1f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13d1f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="13d1f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13d1f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="13d1f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13d1f-107">Atualize as propriedades de [um objeto deviceManagementExportJob.](../resources/intune-reporting-devicemanagementexportjob.md)</span><span class="sxs-lookup"><span data-stu-id="13d1f-107">Update the properties of a [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13d1f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="13d1f-108">Prerequisites</span></span>
<span data-ttu-id="13d1f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13d1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13d1f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13d1f-111">Permission type</span></span>|<span data-ttu-id="13d1f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="13d1f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13d1f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13d1f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13d1f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13d1f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="13d1f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13d1f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13d1f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13d1f-116">Not supported.</span></span>|
|<span data-ttu-id="13d1f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13d1f-117">Application</span></span>|<span data-ttu-id="13d1f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13d1f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13d1f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13d1f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
```

## <a name="request-headers"></a><span data-ttu-id="13d1f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13d1f-120">Request headers</span></span>
|<span data-ttu-id="13d1f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="13d1f-121">Header</span></span>|<span data-ttu-id="13d1f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="13d1f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13d1f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="13d1f-123">Authorization</span></span>|<span data-ttu-id="13d1f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13d1f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13d1f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="13d1f-125">Accept</span></span>|<span data-ttu-id="13d1f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13d1f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13d1f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13d1f-127">Request body</span></span>
<span data-ttu-id="13d1f-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementExportJob.](../resources/intune-reporting-devicemanagementexportjob.md)</span><span class="sxs-lookup"><span data-stu-id="13d1f-128">In the request body, supply a JSON representation for the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

<span data-ttu-id="13d1f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md).</span><span class="sxs-lookup"><span data-stu-id="13d1f-129">The following table shows the properties that are required when you create the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md).</span></span>

|<span data-ttu-id="13d1f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13d1f-130">Property</span></span>|<span data-ttu-id="13d1f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="13d1f-131">Type</span></span>|<span data-ttu-id="13d1f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="13d1f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13d1f-133">id</span><span class="sxs-lookup"><span data-stu-id="13d1f-133">id</span></span>|<span data-ttu-id="13d1f-134">String</span><span class="sxs-lookup"><span data-stu-id="13d1f-134">String</span></span>|<span data-ttu-id="13d1f-135">Identificador exclusivo dessa entidade</span><span class="sxs-lookup"><span data-stu-id="13d1f-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="13d1f-136">reportName</span><span class="sxs-lookup"><span data-stu-id="13d1f-136">reportName</span></span>|<span data-ttu-id="13d1f-137">String</span><span class="sxs-lookup"><span data-stu-id="13d1f-137">String</span></span>|<span data-ttu-id="13d1f-138">Nome do relatório</span><span class="sxs-lookup"><span data-stu-id="13d1f-138">Name of the report</span></span>|
|<span data-ttu-id="13d1f-139">filter</span><span class="sxs-lookup"><span data-stu-id="13d1f-139">filter</span></span>|<span data-ttu-id="13d1f-140">String</span><span class="sxs-lookup"><span data-stu-id="13d1f-140">String</span></span>|<span data-ttu-id="13d1f-141">Filtros aplicados no relatório</span><span class="sxs-lookup"><span data-stu-id="13d1f-141">Filters applied on the report</span></span>|
|<span data-ttu-id="13d1f-142">select</span><span class="sxs-lookup"><span data-stu-id="13d1f-142">select</span></span>|<span data-ttu-id="13d1f-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="13d1f-143">String collection</span></span>|<span data-ttu-id="13d1f-144">Colunas selecionadas no relatório</span><span class="sxs-lookup"><span data-stu-id="13d1f-144">Columns selected from the report</span></span>|
|<span data-ttu-id="13d1f-145">formato</span><span class="sxs-lookup"><span data-stu-id="13d1f-145">format</span></span>|[<span data-ttu-id="13d1f-146">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="13d1f-146">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="13d1f-147">Formato do relatório exportado.</span><span class="sxs-lookup"><span data-stu-id="13d1f-147">Format of the exported report.</span></span> <span data-ttu-id="13d1f-148">Os valores possíveis são: `csv` e `pdf`.</span><span class="sxs-lookup"><span data-stu-id="13d1f-148">Possible values are: `csv`, `pdf`.</span></span>|
|<span data-ttu-id="13d1f-149">snapshotId</span><span class="sxs-lookup"><span data-stu-id="13d1f-149">snapshotId</span></span>|<span data-ttu-id="13d1f-150">String</span><span class="sxs-lookup"><span data-stu-id="13d1f-150">String</span></span>|<span data-ttu-id="13d1f-151">Um instantâneo é um subconjunto identificável do conjuntos de dados representado pelo ReportName.</span><span class="sxs-lookup"><span data-stu-id="13d1f-151">A snapshot is an identifiable subset of the dataset represented by the ReportName.</span></span> <span data-ttu-id="13d1f-152">Uma id sessionId ou CachedReportConfiguration pode ser usada aqui.</span><span class="sxs-lookup"><span data-stu-id="13d1f-152">A sessionId or CachedReportConfiguration id can be used here.</span></span> <span data-ttu-id="13d1f-153">Se uma sessionId for especificada, Filter, Select e OrderBy serão aplicados aos dados representados pela sessionId.</span><span class="sxs-lookup"><span data-stu-id="13d1f-153">If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId.</span></span> <span data-ttu-id="13d1f-154">Filter, Select e OrderBy não podem ser especificados juntamente com uma id CachedReportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="13d1f-154">Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.</span></span>|
|<span data-ttu-id="13d1f-155">localizationType</span><span class="sxs-lookup"><span data-stu-id="13d1f-155">localizationType</span></span>|[<span data-ttu-id="13d1f-156">deviceManagementExportJobLocalizationType</span><span class="sxs-lookup"><span data-stu-id="13d1f-156">deviceManagementExportJobLocalizationType</span></span>](../resources/intune-reporting-devicemanagementexportjoblocalizationtype.md)|<span data-ttu-id="13d1f-157">Configura como o trabalho de exportação solicitado é localizado.</span><span class="sxs-lookup"><span data-stu-id="13d1f-157">Configures how the requested export job is localized.</span></span> <span data-ttu-id="13d1f-158">Os valores possíveis são: `localizedValuesAsAdditionalColumn` e `replaceLocalizableValues`.</span><span class="sxs-lookup"><span data-stu-id="13d1f-158">Possible values are: `localizedValuesAsAdditionalColumn`, `replaceLocalizableValues`.</span></span>|
|<span data-ttu-id="13d1f-159">status</span><span class="sxs-lookup"><span data-stu-id="13d1f-159">status</span></span>|[<span data-ttu-id="13d1f-160">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="13d1f-160">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="13d1f-161">Status do trabalho de exportação.</span><span class="sxs-lookup"><span data-stu-id="13d1f-161">Status of the export job.</span></span> <span data-ttu-id="13d1f-162">Os valores possíveis são: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="13d1f-162">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="13d1f-163">url</span><span class="sxs-lookup"><span data-stu-id="13d1f-163">url</span></span>|<span data-ttu-id="13d1f-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13d1f-164">String</span></span>|<span data-ttu-id="13d1f-165">Local temporário do relatório exportado</span><span class="sxs-lookup"><span data-stu-id="13d1f-165">Temporary location of the exported report</span></span>|
|<span data-ttu-id="13d1f-166">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="13d1f-166">requestDateTime</span></span>|<span data-ttu-id="13d1f-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13d1f-167">DateTimeOffset</span></span>|<span data-ttu-id="13d1f-168">Hora em que o relatório exportado foi solicitado</span><span class="sxs-lookup"><span data-stu-id="13d1f-168">Time that the exported report was requested</span></span>|
|<span data-ttu-id="13d1f-169">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="13d1f-169">expirationDateTime</span></span>|<span data-ttu-id="13d1f-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13d1f-170">DateTimeOffset</span></span>|<span data-ttu-id="13d1f-171">Tempo em que o relatório exportado expira</span><span class="sxs-lookup"><span data-stu-id="13d1f-171">Time that the exported report expires</span></span>|



## <a name="response"></a><span data-ttu-id="13d1f-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="13d1f-172">Response</span></span>
<span data-ttu-id="13d1f-173">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13d1f-173">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13d1f-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13d1f-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="13d1f-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13d1f-175">Request</span></span>
<span data-ttu-id="13d1f-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13d1f-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
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

### <a name="response"></a><span data-ttu-id="13d1f-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="13d1f-177">Response</span></span>
<span data-ttu-id="13d1f-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13d1f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




