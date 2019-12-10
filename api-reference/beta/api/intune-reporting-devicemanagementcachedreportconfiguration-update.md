---
title: Atualizar deviceManagementCachedReportConfiguration
description: Atualiza as propriedades de um objeto deviceManagementCachedReportConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bbb8bd9b270e145c6df88782fcac638f08922738
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940352"
---
# <a name="update-devicemanagementcachedreportconfiguration"></a><span data-ttu-id="9bf12-103">Atualizar deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="9bf12-103">Update deviceManagementCachedReportConfiguration</span></span>

> <span data-ttu-id="9bf12-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9bf12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bf12-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9bf12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bf12-106">Atualiza as propriedades de um objeto [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9bf12-106">Update the properties of a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9bf12-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9bf12-107">Prerequisites</span></span>
<span data-ttu-id="9bf12-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bf12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bf12-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9bf12-110">Permission type</span></span>|<span data-ttu-id="9bf12-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9bf12-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bf12-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9bf12-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9bf12-113">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9bf12-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9bf12-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9bf12-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bf12-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bf12-115">Not supported.</span></span>|
|<span data-ttu-id="9bf12-116">Application</span><span class="sxs-lookup"><span data-stu-id="9bf12-116">Application</span></span>|<span data-ttu-id="9bf12-117">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9bf12-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bf12-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9bf12-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9bf12-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9bf12-119">Request headers</span></span>
|<span data-ttu-id="9bf12-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9bf12-120">Header</span></span>|<span data-ttu-id="9bf12-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9bf12-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bf12-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9bf12-122">Authorization</span></span>|<span data-ttu-id="9bf12-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9bf12-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bf12-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9bf12-124">Accept</span></span>|<span data-ttu-id="9bf12-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9bf12-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bf12-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9bf12-126">Request body</span></span>
<span data-ttu-id="9bf12-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9bf12-127">In the request body, supply a JSON representation for the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

<span data-ttu-id="9bf12-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9bf12-128">The following table shows the properties that are required when you create the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md).</span></span>

|<span data-ttu-id="9bf12-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9bf12-129">Property</span></span>|<span data-ttu-id="9bf12-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bf12-130">Type</span></span>|<span data-ttu-id="9bf12-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bf12-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bf12-132">id</span><span class="sxs-lookup"><span data-stu-id="9bf12-132">id</span></span>|<span data-ttu-id="9bf12-133">String</span><span class="sxs-lookup"><span data-stu-id="9bf12-133">String</span></span>|<span data-ttu-id="9bf12-134">Identificador exclusivo para esta entidade</span><span class="sxs-lookup"><span data-stu-id="9bf12-134">Unique identifier for this entity</span></span>|
|<span data-ttu-id="9bf12-135">reportName</span><span class="sxs-lookup"><span data-stu-id="9bf12-135">reportName</span></span>|<span data-ttu-id="9bf12-136">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="9bf12-136">String</span></span>|<span data-ttu-id="9bf12-137">Nome do relatório</span><span class="sxs-lookup"><span data-stu-id="9bf12-137">Name of the report</span></span>|
|<span data-ttu-id="9bf12-138">filter</span><span class="sxs-lookup"><span data-stu-id="9bf12-138">filter</span></span>|<span data-ttu-id="9bf12-139">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="9bf12-139">String</span></span>|<span data-ttu-id="9bf12-140">Filtros aplicados na criação de relatórios.</span><span class="sxs-lookup"><span data-stu-id="9bf12-140">Filters applied on report creation.</span></span>|
|<span data-ttu-id="9bf12-141">select</span><span class="sxs-lookup"><span data-stu-id="9bf12-141">select</span></span>|<span data-ttu-id="9bf12-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bf12-142">String collection</span></span>|<span data-ttu-id="9bf12-143">Colunas selecionadas do relatório</span><span class="sxs-lookup"><span data-stu-id="9bf12-143">Columns selected from the report</span></span>|
|<span data-ttu-id="9bf12-144">Classificadoporativado</span><span class="sxs-lookup"><span data-stu-id="9bf12-144">orderBy</span></span>|<span data-ttu-id="9bf12-145">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bf12-145">String collection</span></span>|<span data-ttu-id="9bf12-146">Ordenação de colunas no relatório</span><span class="sxs-lookup"><span data-stu-id="9bf12-146">Ordering of columns in the report</span></span>|
|<span data-ttu-id="9bf12-147">status</span><span class="sxs-lookup"><span data-stu-id="9bf12-147">status</span></span>|[<span data-ttu-id="9bf12-148">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="9bf12-148">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="9bf12-149">Status do relatório em cache.</span><span class="sxs-lookup"><span data-stu-id="9bf12-149">Status of the cached report.</span></span> <span data-ttu-id="9bf12-150">Os valores possíveis são: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="9bf12-150">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="9bf12-151">lastRefreshDateTime</span><span class="sxs-lookup"><span data-stu-id="9bf12-151">lastRefreshDateTime</span></span>|<span data-ttu-id="9bf12-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bf12-152">DateTimeOffset</span></span>|<span data-ttu-id="9bf12-153">Hora em que o relatório em cache foi atualizado pela última vez</span><span class="sxs-lookup"><span data-stu-id="9bf12-153">Time that the cached report was last refreshed</span></span>|
|<span data-ttu-id="9bf12-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9bf12-154">expirationDateTime</span></span>|<span data-ttu-id="9bf12-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bf12-155">DateTimeOffset</span></span>|<span data-ttu-id="9bf12-156">Hora em que o relatório em cache expira</span><span class="sxs-lookup"><span data-stu-id="9bf12-156">Time that the cached report expires</span></span>|



## <a name="response"></a><span data-ttu-id="9bf12-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bf12-157">Response</span></span>
<span data-ttu-id="9bf12-158">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9bf12-158">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bf12-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9bf12-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="9bf12-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bf12-160">Request</span></span>
<span data-ttu-id="9bf12-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9bf12-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
Content-type: application/json
Content-length: 385

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
  "status": "notStarted",
  "lastRefreshDateTime": "2016-12-31T23:58:49.97047-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```

### <a name="response"></a><span data-ttu-id="9bf12-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bf12-162">Response</span></span>
<span data-ttu-id="9bf12-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9bf12-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 434

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
  "status": "notStarted",
  "lastRefreshDateTime": "2016-12-31T23:58:49.97047-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```





