---
title: Criar deviceManagementReportSchedule
description: Crie um novo objeto deviceManagementReportSchedule.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a9e29979c0999d05592adaad8e2f19a332a57a8a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134386"
---
# <a name="create-devicemanagementreportschedule"></a><span data-ttu-id="09849-103">Criar deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="09849-103">Create deviceManagementReportSchedule</span></span>

<span data-ttu-id="09849-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09849-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09849-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="09849-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09849-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="09849-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09849-107">Crie um novo [objeto deviceManagementReportSchedule.](../resources/intune-reporting-devicemanagementreportschedule.md)</span><span class="sxs-lookup"><span data-stu-id="09849-107">Create a new [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09849-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="09849-108">Prerequisites</span></span>
<span data-ttu-id="09849-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09849-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09849-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09849-111">Permission type</span></span>|<span data-ttu-id="09849-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="09849-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09849-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09849-113">Delegated (work or school account)</span></span>|<span data-ttu-id="09849-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09849-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="09849-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09849-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09849-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09849-116">Not supported.</span></span>|
|<span data-ttu-id="09849-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09849-117">Application</span></span>|<span data-ttu-id="09849-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09849-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="09849-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09849-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/reportSchedules
```

## <a name="request-headers"></a><span data-ttu-id="09849-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09849-120">Request headers</span></span>
|<span data-ttu-id="09849-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="09849-121">Header</span></span>|<span data-ttu-id="09849-122">Valor</span><span class="sxs-lookup"><span data-stu-id="09849-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09849-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="09849-123">Authorization</span></span>|<span data-ttu-id="09849-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09849-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09849-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="09849-125">Accept</span></span>|<span data-ttu-id="09849-126">application/json</span><span class="sxs-lookup"><span data-stu-id="09849-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09849-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09849-127">Request body</span></span>
<span data-ttu-id="09849-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementReportSchedule.</span><span class="sxs-lookup"><span data-stu-id="09849-128">In the request body, supply a JSON representation for the deviceManagementReportSchedule object.</span></span>

<span data-ttu-id="09849-129">A tabela a seguir mostra as propriedades necessárias ao criar deviceManagementReportSchedule.</span><span class="sxs-lookup"><span data-stu-id="09849-129">The following table shows the properties that are required when you create the deviceManagementReportSchedule.</span></span>

|<span data-ttu-id="09849-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09849-130">Property</span></span>|<span data-ttu-id="09849-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="09849-131">Type</span></span>|<span data-ttu-id="09849-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="09849-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09849-133">id</span><span class="sxs-lookup"><span data-stu-id="09849-133">id</span></span>|<span data-ttu-id="09849-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09849-134">String</span></span>|<span data-ttu-id="09849-135">Identificador exclusivo dessa entidade</span><span class="sxs-lookup"><span data-stu-id="09849-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="09849-136">reportScheduleName</span><span class="sxs-lookup"><span data-stu-id="09849-136">reportScheduleName</span></span>|<span data-ttu-id="09849-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09849-137">String</span></span>|<span data-ttu-id="09849-138">Nome da agenda</span><span class="sxs-lookup"><span data-stu-id="09849-138">Name of the schedule</span></span>|
|<span data-ttu-id="09849-139">assunto</span><span class="sxs-lookup"><span data-stu-id="09849-139">subject</span></span>|<span data-ttu-id="09849-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09849-140">String</span></span>|<span data-ttu-id="09849-141">Assunto dos relatórios agendados que são entregues</span><span class="sxs-lookup"><span data-stu-id="09849-141">Subject of the scheduled reports that are delivered</span></span>|
|<span data-ttu-id="09849-142">emails</span><span class="sxs-lookup"><span data-stu-id="09849-142">emails</span></span>|<span data-ttu-id="09849-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="09849-143">String collection</span></span>|<span data-ttu-id="09849-144">Emails para os quais os relatórios agendados são entregues</span><span class="sxs-lookup"><span data-stu-id="09849-144">Emails to which the scheduled reports are delivered</span></span>|
|<span data-ttu-id="09849-145">recorrência</span><span class="sxs-lookup"><span data-stu-id="09849-145">recurrence</span></span>|[<span data-ttu-id="09849-146">deviceManagementScheduledReportRecurrence</span><span class="sxs-lookup"><span data-stu-id="09849-146">deviceManagementScheduledReportRecurrence</span></span>](../resources/intune-reporting-devicemanagementscheduledreportrecurrence.md)|<span data-ttu-id="09849-147">Frequência de entrega de relatório agendada.</span><span class="sxs-lookup"><span data-stu-id="09849-147">Frequency of scheduled report delivery.</span></span> <span data-ttu-id="09849-148">Os valores possíveis são: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="09849-148">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="09849-149">startDateTime</span><span class="sxs-lookup"><span data-stu-id="09849-149">startDateTime</span></span>|<span data-ttu-id="09849-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09849-150">DateTimeOffset</span></span>|<span data-ttu-id="09849-151">Hora em que a entrega dos relatórios agendados é iniciada</span><span class="sxs-lookup"><span data-stu-id="09849-151">Time that the delivery of the scheduled reports starts</span></span>|
|<span data-ttu-id="09849-152">endDateTime</span><span class="sxs-lookup"><span data-stu-id="09849-152">endDateTime</span></span>|<span data-ttu-id="09849-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09849-153">DateTimeOffset</span></span>|<span data-ttu-id="09849-154">Hora em que a entrega dos relatórios agendados termina</span><span class="sxs-lookup"><span data-stu-id="09849-154">Time that the delivery of the scheduled reports ends</span></span>|
|<span data-ttu-id="09849-155">userId</span><span class="sxs-lookup"><span data-stu-id="09849-155">userId</span></span>|<span data-ttu-id="09849-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09849-156">String</span></span>|<span data-ttu-id="09849-157">A ID do Usuário que criou o relatório</span><span class="sxs-lookup"><span data-stu-id="09849-157">The Id of the User who created the report</span></span>|
|<span data-ttu-id="09849-158">reportName</span><span class="sxs-lookup"><span data-stu-id="09849-158">reportName</span></span>|<span data-ttu-id="09849-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09849-159">String</span></span>|<span data-ttu-id="09849-160">Nome do relatório</span><span class="sxs-lookup"><span data-stu-id="09849-160">Name of the report</span></span>|
|<span data-ttu-id="09849-161">filter</span><span class="sxs-lookup"><span data-stu-id="09849-161">filter</span></span>|<span data-ttu-id="09849-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09849-162">String</span></span>|<span data-ttu-id="09849-163">Filtros aplicados no relatório</span><span class="sxs-lookup"><span data-stu-id="09849-163">Filters applied on the report</span></span>|
|<span data-ttu-id="09849-164">select</span><span class="sxs-lookup"><span data-stu-id="09849-164">select</span></span>|<span data-ttu-id="09849-165">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="09849-165">String collection</span></span>|<span data-ttu-id="09849-166">Colunas selecionadas no relatório</span><span class="sxs-lookup"><span data-stu-id="09849-166">Columns selected from the report</span></span>|
|<span data-ttu-id="09849-167">orderBy</span><span class="sxs-lookup"><span data-stu-id="09849-167">orderBy</span></span>|<span data-ttu-id="09849-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="09849-168">String collection</span></span>|<span data-ttu-id="09849-169">Ordenação de colunas no relatório</span><span class="sxs-lookup"><span data-stu-id="09849-169">Ordering of columns in the report</span></span>|
|<span data-ttu-id="09849-170">formato</span><span class="sxs-lookup"><span data-stu-id="09849-170">format</span></span>|[<span data-ttu-id="09849-171">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="09849-171">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="09849-172">Formato do relatório agendado.</span><span class="sxs-lookup"><span data-stu-id="09849-172">Format of the scheduled report.</span></span> <span data-ttu-id="09849-173">Os valores possíveis são: `csv` e `pdf`.</span><span class="sxs-lookup"><span data-stu-id="09849-173">Possible values are: `csv`, `pdf`.</span></span>|



## <a name="response"></a><span data-ttu-id="09849-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="09849-174">Response</span></span>
<span data-ttu-id="09849-175">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09849-175">If successful, this method returns a `201 Created` response code and a [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09849-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="09849-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="09849-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09849-177">Request</span></span>
<span data-ttu-id="09849-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="09849-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/reportSchedules
Content-type: application/json
Content-length: 539

{
  "@odata.type": "#microsoft.graph.deviceManagementReportSchedule",
  "reportScheduleName": "Report Schedule Name value",
  "subject": "Subject value",
  "emails": [
    "Emails value"
  ],
  "recurrence": "daily",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
  "userId": "User Id value",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "format": "pdf"
}
```

### <a name="response"></a><span data-ttu-id="09849-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="09849-179">Response</span></span>
<span data-ttu-id="09849-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09849-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 588

{
  "@odata.type": "#microsoft.graph.deviceManagementReportSchedule",
  "id": "00bb9785-9785-00bb-8597-bb008597bb00",
  "reportScheduleName": "Report Schedule Name value",
  "subject": "Subject value",
  "emails": [
    "Emails value"
  ],
  "recurrence": "daily",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
  "userId": "User Id value",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "format": "pdf"
}
```




