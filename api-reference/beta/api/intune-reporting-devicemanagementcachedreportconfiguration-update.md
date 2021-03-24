---
title: Atualizar deviceManagementCachedReportConfiguration
description: Atualize as propriedades de um objeto deviceManagementCachedReportConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7b9304713a7b7d278991f8dd9ea07ecaece8f4bb
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123389"
---
# <a name="update-devicemanagementcachedreportconfiguration"></a><span data-ttu-id="0f76c-103">Atualizar deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="0f76c-103">Update deviceManagementCachedReportConfiguration</span></span>

<span data-ttu-id="0f76c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f76c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f76c-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0f76c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f76c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0f76c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f76c-107">Atualize as propriedades de [um objeto deviceManagementCachedReportConfiguration.](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f76c-107">Update the properties of a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f76c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0f76c-108">Prerequisites</span></span>
<span data-ttu-id="0f76c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f76c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f76c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f76c-111">Permission type</span></span>|<span data-ttu-id="0f76c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f76c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f76c-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f76c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0f76c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f76c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0f76c-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f76c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f76c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f76c-116">Not supported.</span></span>|
|<span data-ttu-id="0f76c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f76c-117">Application</span></span>|<span data-ttu-id="0f76c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f76c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f76c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f76c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0f76c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f76c-120">Request headers</span></span>
|<span data-ttu-id="0f76c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0f76c-121">Header</span></span>|<span data-ttu-id="0f76c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0f76c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f76c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f76c-123">Authorization</span></span>|<span data-ttu-id="0f76c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f76c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f76c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0f76c-125">Accept</span></span>|<span data-ttu-id="0f76c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f76c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f76c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f76c-127">Request body</span></span>
<span data-ttu-id="0f76c-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementCachedReportConfiguration.](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f76c-128">In the request body, supply a JSON representation for the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

<span data-ttu-id="0f76c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0f76c-129">The following table shows the properties that are required when you create the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md).</span></span>

|<span data-ttu-id="0f76c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f76c-130">Property</span></span>|<span data-ttu-id="0f76c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f76c-131">Type</span></span>|<span data-ttu-id="0f76c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f76c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f76c-133">id</span><span class="sxs-lookup"><span data-stu-id="0f76c-133">id</span></span>|<span data-ttu-id="0f76c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f76c-134">String</span></span>|<span data-ttu-id="0f76c-135">Identificador exclusivo dessa entidade</span><span class="sxs-lookup"><span data-stu-id="0f76c-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="0f76c-136">reportName</span><span class="sxs-lookup"><span data-stu-id="0f76c-136">reportName</span></span>|<span data-ttu-id="0f76c-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f76c-137">String</span></span>|<span data-ttu-id="0f76c-138">Nome do relatório</span><span class="sxs-lookup"><span data-stu-id="0f76c-138">Name of the report</span></span>|
|<span data-ttu-id="0f76c-139">filter</span><span class="sxs-lookup"><span data-stu-id="0f76c-139">filter</span></span>|<span data-ttu-id="0f76c-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f76c-140">String</span></span>|<span data-ttu-id="0f76c-141">Filtros aplicados na criação de relatório.</span><span class="sxs-lookup"><span data-stu-id="0f76c-141">Filters applied on report creation.</span></span>|
|<span data-ttu-id="0f76c-142">select</span><span class="sxs-lookup"><span data-stu-id="0f76c-142">select</span></span>|<span data-ttu-id="0f76c-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f76c-143">String collection</span></span>|<span data-ttu-id="0f76c-144">Colunas selecionadas no relatório</span><span class="sxs-lookup"><span data-stu-id="0f76c-144">Columns selected from the report</span></span>|
|<span data-ttu-id="0f76c-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="0f76c-145">orderBy</span></span>|<span data-ttu-id="0f76c-146">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f76c-146">String collection</span></span>|<span data-ttu-id="0f76c-147">Ordenação de colunas no relatório</span><span class="sxs-lookup"><span data-stu-id="0f76c-147">Ordering of columns in the report</span></span>|
|<span data-ttu-id="0f76c-148">metadados</span><span class="sxs-lookup"><span data-stu-id="0f76c-148">metadata</span></span>|<span data-ttu-id="0f76c-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f76c-149">String</span></span>|<span data-ttu-id="0f76c-150">Metadados gerenciados pelo chamador associados ao relatório</span><span class="sxs-lookup"><span data-stu-id="0f76c-150">Caller-managed metadata associated with the report</span></span>|
|<span data-ttu-id="0f76c-151">status</span><span class="sxs-lookup"><span data-stu-id="0f76c-151">status</span></span>|[<span data-ttu-id="0f76c-152">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="0f76c-152">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="0f76c-153">Status do relatório armazenado em cache.</span><span class="sxs-lookup"><span data-stu-id="0f76c-153">Status of the cached report.</span></span> <span data-ttu-id="0f76c-154">Os valores possíveis são: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="0f76c-154">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="0f76c-155">lastRefreshDateTime</span><span class="sxs-lookup"><span data-stu-id="0f76c-155">lastRefreshDateTime</span></span>|<span data-ttu-id="0f76c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f76c-156">DateTimeOffset</span></span>|<span data-ttu-id="0f76c-157">Hora em que o relatório em cache foi atualizado pela última vez</span><span class="sxs-lookup"><span data-stu-id="0f76c-157">Time that the cached report was last refreshed</span></span>|
|<span data-ttu-id="0f76c-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0f76c-158">expirationDateTime</span></span>|<span data-ttu-id="0f76c-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f76c-159">DateTimeOffset</span></span>|<span data-ttu-id="0f76c-160">Tempo em que o relatório armazenado em cache expira</span><span class="sxs-lookup"><span data-stu-id="0f76c-160">Time that the cached report expires</span></span>|



## <a name="response"></a><span data-ttu-id="0f76c-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f76c-161">Response</span></span>
<span data-ttu-id="0f76c-162">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f76c-162">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f76c-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f76c-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f76c-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f76c-164">Request</span></span>
<span data-ttu-id="0f76c-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f76c-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0f76c-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f76c-166">Response</span></span>
<span data-ttu-id="0f76c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f76c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




