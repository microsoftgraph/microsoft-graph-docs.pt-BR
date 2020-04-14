---
title: Criar deviceManagementCachedReportConfiguration
description: Criar um novo objeto deviceManagementCachedReportConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bf67c0409dae250af6cabc24de186879f3b3cedf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445204"
---
# <a name="create-devicemanagementcachedreportconfiguration"></a><span data-ttu-id="824f7-103">Criar deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="824f7-103">Create deviceManagementCachedReportConfiguration</span></span>

<span data-ttu-id="824f7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="824f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="824f7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="824f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="824f7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="824f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="824f7-107">Criar um novo objeto [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="824f7-107">Create a new [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="824f7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="824f7-108">Prerequisites</span></span>
<span data-ttu-id="824f7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="824f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="824f7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="824f7-111">Permission type</span></span>|<span data-ttu-id="824f7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="824f7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="824f7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="824f7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="824f7-114">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="824f7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="824f7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="824f7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="824f7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="824f7-116">Not supported.</span></span>|
|<span data-ttu-id="824f7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="824f7-117">Application</span></span>|<span data-ttu-id="824f7-118">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="824f7-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="824f7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="824f7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/cachedReportConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="824f7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="824f7-120">Request headers</span></span>
|<span data-ttu-id="824f7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="824f7-121">Header</span></span>|<span data-ttu-id="824f7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="824f7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="824f7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="824f7-123">Authorization</span></span>|<span data-ttu-id="824f7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="824f7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="824f7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="824f7-125">Accept</span></span>|<span data-ttu-id="824f7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="824f7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="824f7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="824f7-127">Request body</span></span>
<span data-ttu-id="824f7-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementCachedReportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="824f7-128">In the request body, supply a JSON representation for the deviceManagementCachedReportConfiguration object.</span></span>

<span data-ttu-id="824f7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementCachedReportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="824f7-129">The following table shows the properties that are required when you create the deviceManagementCachedReportConfiguration.</span></span>

|<span data-ttu-id="824f7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="824f7-130">Property</span></span>|<span data-ttu-id="824f7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="824f7-131">Type</span></span>|<span data-ttu-id="824f7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="824f7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="824f7-133">id</span><span class="sxs-lookup"><span data-stu-id="824f7-133">id</span></span>|<span data-ttu-id="824f7-134">String</span><span class="sxs-lookup"><span data-stu-id="824f7-134">String</span></span>|<span data-ttu-id="824f7-135">Identificador exclusivo para esta entidade</span><span class="sxs-lookup"><span data-stu-id="824f7-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="824f7-136">reportName</span><span class="sxs-lookup"><span data-stu-id="824f7-136">reportName</span></span>|<span data-ttu-id="824f7-137">String</span><span class="sxs-lookup"><span data-stu-id="824f7-137">String</span></span>|<span data-ttu-id="824f7-138">Nome do relatório</span><span class="sxs-lookup"><span data-stu-id="824f7-138">Name of the report</span></span>|
|<span data-ttu-id="824f7-139">filter</span><span class="sxs-lookup"><span data-stu-id="824f7-139">filter</span></span>|<span data-ttu-id="824f7-140">String</span><span class="sxs-lookup"><span data-stu-id="824f7-140">String</span></span>|<span data-ttu-id="824f7-141">Filtros aplicados na criação de relatórios.</span><span class="sxs-lookup"><span data-stu-id="824f7-141">Filters applied on report creation.</span></span>|
|<span data-ttu-id="824f7-142">select</span><span class="sxs-lookup"><span data-stu-id="824f7-142">select</span></span>|<span data-ttu-id="824f7-143">Coleção String</span><span class="sxs-lookup"><span data-stu-id="824f7-143">String collection</span></span>|<span data-ttu-id="824f7-144">Colunas selecionadas do relatório</span><span class="sxs-lookup"><span data-stu-id="824f7-144">Columns selected from the report</span></span>|
|<span data-ttu-id="824f7-145">Classificadoporativado</span><span class="sxs-lookup"><span data-stu-id="824f7-145">orderBy</span></span>|<span data-ttu-id="824f7-146">Coleção String</span><span class="sxs-lookup"><span data-stu-id="824f7-146">String collection</span></span>|<span data-ttu-id="824f7-147">Ordenação de colunas no relatório</span><span class="sxs-lookup"><span data-stu-id="824f7-147">Ordering of columns in the report</span></span>|
|<span data-ttu-id="824f7-148">status</span><span class="sxs-lookup"><span data-stu-id="824f7-148">status</span></span>|[<span data-ttu-id="824f7-149">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="824f7-149">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="824f7-150">Status do relatório em cache.</span><span class="sxs-lookup"><span data-stu-id="824f7-150">Status of the cached report.</span></span> <span data-ttu-id="824f7-151">Os valores possíveis são: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="824f7-151">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="824f7-152">lastRefreshDateTime</span><span class="sxs-lookup"><span data-stu-id="824f7-152">lastRefreshDateTime</span></span>|<span data-ttu-id="824f7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="824f7-153">DateTimeOffset</span></span>|<span data-ttu-id="824f7-154">Hora em que o relatório em cache foi atualizado pela última vez</span><span class="sxs-lookup"><span data-stu-id="824f7-154">Time that the cached report was last refreshed</span></span>|
|<span data-ttu-id="824f7-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="824f7-155">expirationDateTime</span></span>|<span data-ttu-id="824f7-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="824f7-156">DateTimeOffset</span></span>|<span data-ttu-id="824f7-157">Hora em que o relatório em cache expira</span><span class="sxs-lookup"><span data-stu-id="824f7-157">Time that the cached report expires</span></span>|



## <a name="response"></a><span data-ttu-id="824f7-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="824f7-158">Response</span></span>
<span data-ttu-id="824f7-159">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="824f7-159">If successful, this method returns a `201 Created` response code and a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="824f7-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="824f7-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="824f7-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="824f7-161">Request</span></span>
<span data-ttu-id="824f7-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="824f7-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="824f7-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="824f7-163">Response</span></span>
<span data-ttu-id="824f7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="824f7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



