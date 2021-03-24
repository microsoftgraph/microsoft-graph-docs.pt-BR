---
title: Criar deviceManagementCachedReportConfiguration
description: Crie um novo objeto deviceManagementCachedReportConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9df14360ac503b20eaf881fb37a79c111c8c2c2a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51124600"
---
# <a name="create-devicemanagementcachedreportconfiguration"></a><span data-ttu-id="49800-103">Criar deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="49800-103">Create deviceManagementCachedReportConfiguration</span></span>

<span data-ttu-id="49800-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49800-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49800-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="49800-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49800-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="49800-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49800-107">Crie um novo [objeto deviceManagementCachedReportConfiguration.](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49800-107">Create a new [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49800-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="49800-108">Prerequisites</span></span>
<span data-ttu-id="49800-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49800-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49800-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49800-111">Permission type</span></span>|<span data-ttu-id="49800-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="49800-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49800-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49800-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49800-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49800-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="49800-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49800-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49800-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49800-116">Not supported.</span></span>|
|<span data-ttu-id="49800-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49800-117">Application</span></span>|<span data-ttu-id="49800-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49800-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49800-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49800-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/cachedReportConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="49800-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49800-120">Request headers</span></span>
|<span data-ttu-id="49800-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="49800-121">Header</span></span>|<span data-ttu-id="49800-122">Valor</span><span class="sxs-lookup"><span data-stu-id="49800-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49800-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="49800-123">Authorization</span></span>|<span data-ttu-id="49800-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49800-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49800-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="49800-125">Accept</span></span>|<span data-ttu-id="49800-126">application/json</span><span class="sxs-lookup"><span data-stu-id="49800-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49800-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49800-127">Request body</span></span>
<span data-ttu-id="49800-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementCachedReportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="49800-128">In the request body, supply a JSON representation for the deviceManagementCachedReportConfiguration object.</span></span>

<span data-ttu-id="49800-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementCachedReportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="49800-129">The following table shows the properties that are required when you create the deviceManagementCachedReportConfiguration.</span></span>

|<span data-ttu-id="49800-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49800-130">Property</span></span>|<span data-ttu-id="49800-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="49800-131">Type</span></span>|<span data-ttu-id="49800-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="49800-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49800-133">id</span><span class="sxs-lookup"><span data-stu-id="49800-133">id</span></span>|<span data-ttu-id="49800-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49800-134">String</span></span>|<span data-ttu-id="49800-135">Identificador exclusivo dessa entidade</span><span class="sxs-lookup"><span data-stu-id="49800-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="49800-136">reportName</span><span class="sxs-lookup"><span data-stu-id="49800-136">reportName</span></span>|<span data-ttu-id="49800-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49800-137">String</span></span>|<span data-ttu-id="49800-138">Nome do relatório</span><span class="sxs-lookup"><span data-stu-id="49800-138">Name of the report</span></span>|
|<span data-ttu-id="49800-139">filter</span><span class="sxs-lookup"><span data-stu-id="49800-139">filter</span></span>|<span data-ttu-id="49800-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49800-140">String</span></span>|<span data-ttu-id="49800-141">Filtros aplicados na criação de relatório.</span><span class="sxs-lookup"><span data-stu-id="49800-141">Filters applied on report creation.</span></span>|
|<span data-ttu-id="49800-142">select</span><span class="sxs-lookup"><span data-stu-id="49800-142">select</span></span>|<span data-ttu-id="49800-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="49800-143">String collection</span></span>|<span data-ttu-id="49800-144">Colunas selecionadas no relatório</span><span class="sxs-lookup"><span data-stu-id="49800-144">Columns selected from the report</span></span>|
|<span data-ttu-id="49800-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="49800-145">orderBy</span></span>|<span data-ttu-id="49800-146">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="49800-146">String collection</span></span>|<span data-ttu-id="49800-147">Ordenação de colunas no relatório</span><span class="sxs-lookup"><span data-stu-id="49800-147">Ordering of columns in the report</span></span>|
|<span data-ttu-id="49800-148">metadados</span><span class="sxs-lookup"><span data-stu-id="49800-148">metadata</span></span>|<span data-ttu-id="49800-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49800-149">String</span></span>|<span data-ttu-id="49800-150">Metadados gerenciados pelo chamador associados ao relatório</span><span class="sxs-lookup"><span data-stu-id="49800-150">Caller-managed metadata associated with the report</span></span>|
|<span data-ttu-id="49800-151">status</span><span class="sxs-lookup"><span data-stu-id="49800-151">status</span></span>|[<span data-ttu-id="49800-152">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="49800-152">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="49800-153">Status do relatório armazenado em cache.</span><span class="sxs-lookup"><span data-stu-id="49800-153">Status of the cached report.</span></span> <span data-ttu-id="49800-154">Os valores possíveis são: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="49800-154">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="49800-155">lastRefreshDateTime</span><span class="sxs-lookup"><span data-stu-id="49800-155">lastRefreshDateTime</span></span>|<span data-ttu-id="49800-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49800-156">DateTimeOffset</span></span>|<span data-ttu-id="49800-157">Hora em que o relatório em cache foi atualizado pela última vez</span><span class="sxs-lookup"><span data-stu-id="49800-157">Time that the cached report was last refreshed</span></span>|
|<span data-ttu-id="49800-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="49800-158">expirationDateTime</span></span>|<span data-ttu-id="49800-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49800-159">DateTimeOffset</span></span>|<span data-ttu-id="49800-160">Tempo em que o relatório armazenado em cache expira</span><span class="sxs-lookup"><span data-stu-id="49800-160">Time that the cached report expires</span></span>|



## <a name="response"></a><span data-ttu-id="49800-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="49800-161">Response</span></span>
<span data-ttu-id="49800-162">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49800-162">If successful, this method returns a `201 Created` response code and a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49800-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49800-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="49800-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49800-164">Request</span></span>
<span data-ttu-id="49800-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49800-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/cachedReportConfigurations
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

### <a name="response"></a><span data-ttu-id="49800-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="49800-166">Response</span></span>
<span data-ttu-id="49800-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49800-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




