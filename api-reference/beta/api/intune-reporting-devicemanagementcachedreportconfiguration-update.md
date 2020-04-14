---
title: Atualizar deviceManagementCachedReportConfiguration
description: Atualiza as propriedades de um objeto deviceManagementCachedReportConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e7672fde7ce169fecc4063da75b5ac3649af3a82
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445143"
---
# <a name="update-devicemanagementcachedreportconfiguration"></a><span data-ttu-id="f7b4c-103">Atualizar deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="f7b4c-103">Update deviceManagementCachedReportConfiguration</span></span>

<span data-ttu-id="f7b4c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7b4c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7b4c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f7b4c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7b4c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f7b4c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7b4c-107">Atualiza as propriedades de um objeto [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f7b4c-107">Update the properties of a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7b4c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f7b4c-108">Prerequisites</span></span>
<span data-ttu-id="f7b4c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7b4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7b4c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7b4c-111">Permission type</span></span>|<span data-ttu-id="f7b4c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f7b4c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7b4c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7b4c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7b4c-114">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f7b4c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f7b4c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7b4c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7b4c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7b4c-116">Not supported.</span></span>|
|<span data-ttu-id="f7b4c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7b4c-117">Application</span></span>|<span data-ttu-id="f7b4c-118">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f7b4c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7b4c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7b4c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f7b4c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7b4c-120">Request headers</span></span>
|<span data-ttu-id="f7b4c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f7b4c-121">Header</span></span>|<span data-ttu-id="f7b4c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f7b4c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7b4c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7b4c-123">Authorization</span></span>|<span data-ttu-id="f7b4c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7b4c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7b4c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f7b4c-125">Accept</span></span>|<span data-ttu-id="f7b4c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7b4c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7b4c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7b4c-127">Request body</span></span>
<span data-ttu-id="f7b4c-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f7b4c-128">In the request body, supply a JSON representation for the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

<span data-ttu-id="f7b4c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7b4c-129">The following table shows the properties that are required when you create the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md).</span></span>

|<span data-ttu-id="f7b4c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7b4c-130">Property</span></span>|<span data-ttu-id="f7b4c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7b4c-131">Type</span></span>|<span data-ttu-id="f7b4c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7b4c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7b4c-133">id</span><span class="sxs-lookup"><span data-stu-id="f7b4c-133">id</span></span>|<span data-ttu-id="f7b4c-134">String</span><span class="sxs-lookup"><span data-stu-id="f7b4c-134">String</span></span>|<span data-ttu-id="f7b4c-135">Identificador exclusivo para esta entidade</span><span class="sxs-lookup"><span data-stu-id="f7b4c-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="f7b4c-136">reportName</span><span class="sxs-lookup"><span data-stu-id="f7b4c-136">reportName</span></span>|<span data-ttu-id="f7b4c-137">String</span><span class="sxs-lookup"><span data-stu-id="f7b4c-137">String</span></span>|<span data-ttu-id="f7b4c-138">Nome do relatório</span><span class="sxs-lookup"><span data-stu-id="f7b4c-138">Name of the report</span></span>|
|<span data-ttu-id="f7b4c-139">filter</span><span class="sxs-lookup"><span data-stu-id="f7b4c-139">filter</span></span>|<span data-ttu-id="f7b4c-140">String</span><span class="sxs-lookup"><span data-stu-id="f7b4c-140">String</span></span>|<span data-ttu-id="f7b4c-141">Filtros aplicados na criação de relatórios.</span><span class="sxs-lookup"><span data-stu-id="f7b4c-141">Filters applied on report creation.</span></span>|
|<span data-ttu-id="f7b4c-142">select</span><span class="sxs-lookup"><span data-stu-id="f7b4c-142">select</span></span>|<span data-ttu-id="f7b4c-143">Coleção String</span><span class="sxs-lookup"><span data-stu-id="f7b4c-143">String collection</span></span>|<span data-ttu-id="f7b4c-144">Colunas selecionadas do relatório</span><span class="sxs-lookup"><span data-stu-id="f7b4c-144">Columns selected from the report</span></span>|
|<span data-ttu-id="f7b4c-145">Classificadoporativado</span><span class="sxs-lookup"><span data-stu-id="f7b4c-145">orderBy</span></span>|<span data-ttu-id="f7b4c-146">Coleção String</span><span class="sxs-lookup"><span data-stu-id="f7b4c-146">String collection</span></span>|<span data-ttu-id="f7b4c-147">Ordenação de colunas no relatório</span><span class="sxs-lookup"><span data-stu-id="f7b4c-147">Ordering of columns in the report</span></span>|
|<span data-ttu-id="f7b4c-148">status</span><span class="sxs-lookup"><span data-stu-id="f7b4c-148">status</span></span>|[<span data-ttu-id="f7b4c-149">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="f7b4c-149">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="f7b4c-150">Status do relatório em cache.</span><span class="sxs-lookup"><span data-stu-id="f7b4c-150">Status of the cached report.</span></span> <span data-ttu-id="f7b4c-151">Os valores possíveis são: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="f7b4c-151">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="f7b4c-152">lastRefreshDateTime</span><span class="sxs-lookup"><span data-stu-id="f7b4c-152">lastRefreshDateTime</span></span>|<span data-ttu-id="f7b4c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7b4c-153">DateTimeOffset</span></span>|<span data-ttu-id="f7b4c-154">Hora em que o relatório em cache foi atualizado pela última vez</span><span class="sxs-lookup"><span data-stu-id="f7b4c-154">Time that the cached report was last refreshed</span></span>|
|<span data-ttu-id="f7b4c-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f7b4c-155">expirationDateTime</span></span>|<span data-ttu-id="f7b4c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7b4c-156">DateTimeOffset</span></span>|<span data-ttu-id="f7b4c-157">Hora em que o relatório em cache expira</span><span class="sxs-lookup"><span data-stu-id="f7b4c-157">Time that the cached report expires</span></span>|



## <a name="response"></a><span data-ttu-id="f7b4c-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7b4c-158">Response</span></span>
<span data-ttu-id="f7b4c-159">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7b4c-159">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7b4c-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7b4c-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7b4c-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7b4c-161">Request</span></span>
<span data-ttu-id="f7b4c-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7b4c-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f7b4c-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7b4c-163">Response</span></span>
<span data-ttu-id="f7b4c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7b4c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



