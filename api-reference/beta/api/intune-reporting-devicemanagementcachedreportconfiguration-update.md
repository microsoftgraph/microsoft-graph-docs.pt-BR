---
title: Atualizar deviceManagementCachedReportConfiguration
description: Atualiza as propriedades de um objeto deviceManagementCachedReportConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0f43a7b91931ba777909df75facb91d488033ca9
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791339"
---
# <a name="update-devicemanagementcachedreportconfiguration"></a><span data-ttu-id="5330e-103">Atualizar deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="5330e-103">Update deviceManagementCachedReportConfiguration</span></span>

<span data-ttu-id="5330e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5330e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5330e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5330e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5330e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5330e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5330e-107">Atualiza as propriedades de um objeto [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5330e-107">Update the properties of a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5330e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5330e-108">Prerequisites</span></span>
<span data-ttu-id="5330e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5330e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5330e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5330e-111">Permission type</span></span>|<span data-ttu-id="5330e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5330e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5330e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5330e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5330e-114">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5330e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5330e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5330e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5330e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5330e-116">Not supported.</span></span>|
|<span data-ttu-id="5330e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5330e-117">Application</span></span>|<span data-ttu-id="5330e-118">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5330e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5330e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5330e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5330e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5330e-120">Request headers</span></span>
|<span data-ttu-id="5330e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5330e-121">Header</span></span>|<span data-ttu-id="5330e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5330e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5330e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5330e-123">Authorization</span></span>|<span data-ttu-id="5330e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5330e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5330e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5330e-125">Accept</span></span>|<span data-ttu-id="5330e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5330e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5330e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5330e-127">Request body</span></span>
<span data-ttu-id="5330e-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5330e-128">In the request body, supply a JSON representation for the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

<span data-ttu-id="5330e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5330e-129">The following table shows the properties that are required when you create the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md).</span></span>

|<span data-ttu-id="5330e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5330e-130">Property</span></span>|<span data-ttu-id="5330e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5330e-131">Type</span></span>|<span data-ttu-id="5330e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5330e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5330e-133">id</span><span class="sxs-lookup"><span data-stu-id="5330e-133">id</span></span>|<span data-ttu-id="5330e-134">String</span><span class="sxs-lookup"><span data-stu-id="5330e-134">String</span></span>|<span data-ttu-id="5330e-135">Identificador exclusivo para esta entidade</span><span class="sxs-lookup"><span data-stu-id="5330e-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="5330e-136">reportName</span><span class="sxs-lookup"><span data-stu-id="5330e-136">reportName</span></span>|<span data-ttu-id="5330e-137">String</span><span class="sxs-lookup"><span data-stu-id="5330e-137">String</span></span>|<span data-ttu-id="5330e-138">Nome do relatório</span><span class="sxs-lookup"><span data-stu-id="5330e-138">Name of the report</span></span>|
|<span data-ttu-id="5330e-139">filter</span><span class="sxs-lookup"><span data-stu-id="5330e-139">filter</span></span>|<span data-ttu-id="5330e-140">String</span><span class="sxs-lookup"><span data-stu-id="5330e-140">String</span></span>|<span data-ttu-id="5330e-141">Filtros aplicados na criação de relatórios.</span><span class="sxs-lookup"><span data-stu-id="5330e-141">Filters applied on report creation.</span></span>|
|<span data-ttu-id="5330e-142">select</span><span class="sxs-lookup"><span data-stu-id="5330e-142">select</span></span>|<span data-ttu-id="5330e-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5330e-143">String collection</span></span>|<span data-ttu-id="5330e-144">Colunas selecionadas do relatório</span><span class="sxs-lookup"><span data-stu-id="5330e-144">Columns selected from the report</span></span>|
|<span data-ttu-id="5330e-145">Classificadoporativado</span><span class="sxs-lookup"><span data-stu-id="5330e-145">orderBy</span></span>|<span data-ttu-id="5330e-146">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5330e-146">String collection</span></span>|<span data-ttu-id="5330e-147">Ordenação de colunas no relatório</span><span class="sxs-lookup"><span data-stu-id="5330e-147">Ordering of columns in the report</span></span>|
|<span data-ttu-id="5330e-148">los</span><span class="sxs-lookup"><span data-stu-id="5330e-148">metadata</span></span>|<span data-ttu-id="5330e-149">String</span><span class="sxs-lookup"><span data-stu-id="5330e-149">String</span></span>|<span data-ttu-id="5330e-150">Metadados gerenciados pelo chamador associados ao relatório</span><span class="sxs-lookup"><span data-stu-id="5330e-150">Caller-managed metadata associated with the report</span></span>|
|<span data-ttu-id="5330e-151">status</span><span class="sxs-lookup"><span data-stu-id="5330e-151">status</span></span>|[<span data-ttu-id="5330e-152">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="5330e-152">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="5330e-153">Status do relatório em cache.</span><span class="sxs-lookup"><span data-stu-id="5330e-153">Status of the cached report.</span></span> <span data-ttu-id="5330e-154">Os valores possíveis são: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="5330e-154">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="5330e-155">lastRefreshDateTime</span><span class="sxs-lookup"><span data-stu-id="5330e-155">lastRefreshDateTime</span></span>|<span data-ttu-id="5330e-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5330e-156">DateTimeOffset</span></span>|<span data-ttu-id="5330e-157">Hora em que o relatório em cache foi atualizado pela última vez</span><span class="sxs-lookup"><span data-stu-id="5330e-157">Time that the cached report was last refreshed</span></span>|
|<span data-ttu-id="5330e-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5330e-158">expirationDateTime</span></span>|<span data-ttu-id="5330e-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5330e-159">DateTimeOffset</span></span>|<span data-ttu-id="5330e-160">Hora em que o relatório em cache expira</span><span class="sxs-lookup"><span data-stu-id="5330e-160">Time that the cached report expires</span></span>|



## <a name="response"></a><span data-ttu-id="5330e-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="5330e-161">Response</span></span>
<span data-ttu-id="5330e-162">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5330e-162">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5330e-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5330e-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="5330e-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5330e-164">Request</span></span>
<span data-ttu-id="5330e-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5330e-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
Content-type: application/json
Content-length: 418

{
  "@odata.type": "#microsoft.graph.deviceManagementCachedReportConfiguration",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "metadata": "Metadata value",
  "status": "notStarted",
  "lastRefreshDateTime": "2016-12-31T23:58:49.97047-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```

### <a name="response"></a><span data-ttu-id="5330e-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="5330e-166">Response</span></span>
<span data-ttu-id="5330e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5330e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 467

{
  "@odata.type": "#microsoft.graph.deviceManagementCachedReportConfiguration",
  "id": "46947722-7722-4694-2277-944622779446",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "metadata": "Metadata value",
  "status": "notStarted",
  "lastRefreshDateTime": "2016-12-31T23:58:49.97047-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```



