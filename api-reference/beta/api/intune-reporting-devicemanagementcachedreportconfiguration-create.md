---
title: Criar deviceManagementCachedReportConfiguration
description: Criar um novo objeto deviceManagementCachedReportConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3f0447c2ec79d7755ac09c35984c4d68ecc4c275
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801471"
---
# <a name="create-devicemanagementcachedreportconfiguration"></a><span data-ttu-id="7dc8e-103">Criar deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="7dc8e-103">Create deviceManagementCachedReportConfiguration</span></span>

> <span data-ttu-id="7dc8e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7dc8e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7dc8e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7dc8e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7dc8e-106">Criar um novo objeto [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7dc8e-106">Create a new [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7dc8e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7dc8e-107">Prerequisites</span></span>
<span data-ttu-id="7dc8e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dc8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dc8e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7dc8e-110">Permission type</span></span>|<span data-ttu-id="7dc8e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7dc8e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7dc8e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7dc8e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7dc8e-113">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7dc8e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7dc8e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7dc8e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7dc8e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7dc8e-115">Not supported.</span></span>|
|<span data-ttu-id="7dc8e-116">Application</span><span class="sxs-lookup"><span data-stu-id="7dc8e-116">Application</span></span>|<span data-ttu-id="7dc8e-117">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7dc8e-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7dc8e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7dc8e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/cachedReportConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7dc8e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7dc8e-119">Request headers</span></span>
|<span data-ttu-id="7dc8e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7dc8e-120">Header</span></span>|<span data-ttu-id="7dc8e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7dc8e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7dc8e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7dc8e-122">Authorization</span></span>|<span data-ttu-id="7dc8e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7dc8e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7dc8e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7dc8e-124">Accept</span></span>|<span data-ttu-id="7dc8e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7dc8e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7dc8e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7dc8e-126">Request body</span></span>
<span data-ttu-id="7dc8e-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementCachedReportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7dc8e-127">In the request body, supply a JSON representation for the deviceManagementCachedReportConfiguration object.</span></span>

<span data-ttu-id="7dc8e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementCachedReportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7dc8e-128">The following table shows the properties that are required when you create the deviceManagementCachedReportConfiguration.</span></span>

|<span data-ttu-id="7dc8e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7dc8e-129">Property</span></span>|<span data-ttu-id="7dc8e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7dc8e-130">Type</span></span>|<span data-ttu-id="7dc8e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7dc8e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dc8e-132">id</span><span class="sxs-lookup"><span data-stu-id="7dc8e-132">id</span></span>|<span data-ttu-id="7dc8e-133">String</span><span class="sxs-lookup"><span data-stu-id="7dc8e-133">String</span></span>|<span data-ttu-id="7dc8e-134">Identificador exclusivo para esta entidade</span><span class="sxs-lookup"><span data-stu-id="7dc8e-134">Unique identifier for this entity</span></span>|
|<span data-ttu-id="7dc8e-135">reportName</span><span class="sxs-lookup"><span data-stu-id="7dc8e-135">reportName</span></span>|<span data-ttu-id="7dc8e-136">String</span><span class="sxs-lookup"><span data-stu-id="7dc8e-136">String</span></span>|<span data-ttu-id="7dc8e-137">Nome do relatório</span><span class="sxs-lookup"><span data-stu-id="7dc8e-137">Name of the report</span></span>|
|<span data-ttu-id="7dc8e-138">filter</span><span class="sxs-lookup"><span data-stu-id="7dc8e-138">filter</span></span>|<span data-ttu-id="7dc8e-139">String</span><span class="sxs-lookup"><span data-stu-id="7dc8e-139">String</span></span>|<span data-ttu-id="7dc8e-140">Filtros aplicados na criação de relatórios.</span><span class="sxs-lookup"><span data-stu-id="7dc8e-140">Filters applied on report creation.</span></span>|
|<span data-ttu-id="7dc8e-141">select</span><span class="sxs-lookup"><span data-stu-id="7dc8e-141">select</span></span>|<span data-ttu-id="7dc8e-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7dc8e-142">String collection</span></span>|<span data-ttu-id="7dc8e-143">Colunas selecionadas do relatório</span><span class="sxs-lookup"><span data-stu-id="7dc8e-143">Columns selected from the report</span></span>|
|<span data-ttu-id="7dc8e-144">Classificadoporativado</span><span class="sxs-lookup"><span data-stu-id="7dc8e-144">orderBy</span></span>|<span data-ttu-id="7dc8e-145">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7dc8e-145">String collection</span></span>|<span data-ttu-id="7dc8e-146">Ordenação de colunas no relatório</span><span class="sxs-lookup"><span data-stu-id="7dc8e-146">Ordering of columns in the report</span></span>|
|<span data-ttu-id="7dc8e-147">status</span><span class="sxs-lookup"><span data-stu-id="7dc8e-147">status</span></span>|[<span data-ttu-id="7dc8e-148">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="7dc8e-148">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="7dc8e-149">Status do relatório em cache.</span><span class="sxs-lookup"><span data-stu-id="7dc8e-149">Status of the cached report.</span></span> <span data-ttu-id="7dc8e-150">Os valores possíveis são: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="7dc8e-150">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="7dc8e-151">lastRefreshDateTime</span><span class="sxs-lookup"><span data-stu-id="7dc8e-151">lastRefreshDateTime</span></span>|<span data-ttu-id="7dc8e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dc8e-152">DateTimeOffset</span></span>|<span data-ttu-id="7dc8e-153">Hora em que o relatório em cache foi atualizado pela última vez</span><span class="sxs-lookup"><span data-stu-id="7dc8e-153">Time that the cached report was last refreshed</span></span>|
|<span data-ttu-id="7dc8e-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7dc8e-154">expirationDateTime</span></span>|<span data-ttu-id="7dc8e-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dc8e-155">DateTimeOffset</span></span>|<span data-ttu-id="7dc8e-156">Hora em que o relatório em cache expira</span><span class="sxs-lookup"><span data-stu-id="7dc8e-156">Time that the cached report expires</span></span>|



## <a name="response"></a><span data-ttu-id="7dc8e-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dc8e-157">Response</span></span>
<span data-ttu-id="7dc8e-158">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7dc8e-158">If successful, this method returns a `201 Created` response code and a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dc8e-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7dc8e-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="7dc8e-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7dc8e-160">Request</span></span>
<span data-ttu-id="7dc8e-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7dc8e-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/cachedReportConfigurations
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

### <a name="response"></a><span data-ttu-id="7dc8e-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dc8e-162">Response</span></span>
<span data-ttu-id="7dc8e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7dc8e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




