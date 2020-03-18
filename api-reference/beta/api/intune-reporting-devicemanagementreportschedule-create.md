---
title: Criar deviceManagementReportSchedule
description: Criar um novo objeto deviceManagementReportSchedule.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9da17410312e4d4aeb98f535328df5923439bf22
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801345"
---
# <a name="create-devicemanagementreportschedule"></a><span data-ttu-id="ca758-103">Criar deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="ca758-103">Create deviceManagementReportSchedule</span></span>

> <span data-ttu-id="ca758-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ca758-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca758-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ca758-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca758-106">Criar um novo objeto [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) .</span><span class="sxs-lookup"><span data-stu-id="ca758-106">Create a new [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca758-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ca758-107">Prerequisites</span></span>
<span data-ttu-id="ca758-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca758-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca758-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca758-110">Permission type</span></span>|<span data-ttu-id="ca758-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ca758-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca758-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca758-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ca758-113">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ca758-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ca758-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca758-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca758-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca758-115">Not supported.</span></span>|
|<span data-ttu-id="ca758-116">Application</span><span class="sxs-lookup"><span data-stu-id="ca758-116">Application</span></span>|<span data-ttu-id="ca758-117">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ca758-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca758-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca758-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/reportSchedules
```

## <a name="request-headers"></a><span data-ttu-id="ca758-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca758-119">Request headers</span></span>
|<span data-ttu-id="ca758-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ca758-120">Header</span></span>|<span data-ttu-id="ca758-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ca758-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca758-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca758-122">Authorization</span></span>|<span data-ttu-id="ca758-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca758-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca758-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ca758-124">Accept</span></span>|<span data-ttu-id="ca758-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ca758-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca758-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca758-126">Request body</span></span>
<span data-ttu-id="ca758-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementReportSchedule.</span><span class="sxs-lookup"><span data-stu-id="ca758-127">In the request body, supply a JSON representation for the deviceManagementReportSchedule object.</span></span>

<span data-ttu-id="ca758-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementReportSchedule.</span><span class="sxs-lookup"><span data-stu-id="ca758-128">The following table shows the properties that are required when you create the deviceManagementReportSchedule.</span></span>

|<span data-ttu-id="ca758-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca758-129">Property</span></span>|<span data-ttu-id="ca758-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca758-130">Type</span></span>|<span data-ttu-id="ca758-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca758-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca758-132">id</span><span class="sxs-lookup"><span data-stu-id="ca758-132">id</span></span>|<span data-ttu-id="ca758-133">String</span><span class="sxs-lookup"><span data-stu-id="ca758-133">String</span></span>|<span data-ttu-id="ca758-134">Identificador exclusivo para esta entidade</span><span class="sxs-lookup"><span data-stu-id="ca758-134">Unique identifier for this entity</span></span>|
|<span data-ttu-id="ca758-135">reportScheduleName</span><span class="sxs-lookup"><span data-stu-id="ca758-135">reportScheduleName</span></span>|<span data-ttu-id="ca758-136">String</span><span class="sxs-lookup"><span data-stu-id="ca758-136">String</span></span>|<span data-ttu-id="ca758-137">Nome da agenda</span><span class="sxs-lookup"><span data-stu-id="ca758-137">Name of the schedule</span></span>|
|<span data-ttu-id="ca758-138">assunto</span><span class="sxs-lookup"><span data-stu-id="ca758-138">subject</span></span>|<span data-ttu-id="ca758-139">String</span><span class="sxs-lookup"><span data-stu-id="ca758-139">String</span></span>|<span data-ttu-id="ca758-140">Assunto dos relatórios agendados que são entregues</span><span class="sxs-lookup"><span data-stu-id="ca758-140">Subject of the scheduled reports that are delivered</span></span>|
|<span data-ttu-id="ca758-141">email</span><span class="sxs-lookup"><span data-stu-id="ca758-141">emails</span></span>|<span data-ttu-id="ca758-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca758-142">String collection</span></span>|<span data-ttu-id="ca758-143">Emails para os quais os relatórios agendados são entregues</span><span class="sxs-lookup"><span data-stu-id="ca758-143">Emails to which the scheduled reports are delivered</span></span>|
|<span data-ttu-id="ca758-144">recurrence</span><span class="sxs-lookup"><span data-stu-id="ca758-144">recurrence</span></span>|[<span data-ttu-id="ca758-145">deviceManagementScheduledReportRecurrence</span><span class="sxs-lookup"><span data-stu-id="ca758-145">deviceManagementScheduledReportRecurrence</span></span>](../resources/intune-reporting-devicemanagementscheduledreportrecurrence.md)|<span data-ttu-id="ca758-146">Frequência da entrega de relatórios agendados.</span><span class="sxs-lookup"><span data-stu-id="ca758-146">Frequency of scheduled report delivery.</span></span> <span data-ttu-id="ca758-147">Os valores possíveis são: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="ca758-147">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="ca758-148">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ca758-148">startDateTime</span></span>|<span data-ttu-id="ca758-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca758-149">DateTimeOffset</span></span>|<span data-ttu-id="ca758-150">Hora de início da entrega dos relatórios agendados</span><span class="sxs-lookup"><span data-stu-id="ca758-150">Time that the delivery of the scheduled reports starts</span></span>|
|<span data-ttu-id="ca758-151">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ca758-151">endDateTime</span></span>|<span data-ttu-id="ca758-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca758-152">DateTimeOffset</span></span>|<span data-ttu-id="ca758-153">Hora em que a entrega dos relatórios agendados termina</span><span class="sxs-lookup"><span data-stu-id="ca758-153">Time that the delivery of the scheduled reports ends</span></span>|
|<span data-ttu-id="ca758-154">userId</span><span class="sxs-lookup"><span data-stu-id="ca758-154">userId</span></span>|<span data-ttu-id="ca758-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca758-155">String</span></span>|<span data-ttu-id="ca758-156">A ID do usuário que criou o relatório</span><span class="sxs-lookup"><span data-stu-id="ca758-156">The Id of the User who created the report</span></span>|
|<span data-ttu-id="ca758-157">reportName</span><span class="sxs-lookup"><span data-stu-id="ca758-157">reportName</span></span>|<span data-ttu-id="ca758-158">String</span><span class="sxs-lookup"><span data-stu-id="ca758-158">String</span></span>|<span data-ttu-id="ca758-159">Nome do relatório</span><span class="sxs-lookup"><span data-stu-id="ca758-159">Name of the report</span></span>|
|<span data-ttu-id="ca758-160">filter</span><span class="sxs-lookup"><span data-stu-id="ca758-160">filter</span></span>|<span data-ttu-id="ca758-161">String</span><span class="sxs-lookup"><span data-stu-id="ca758-161">String</span></span>|<span data-ttu-id="ca758-162">Filtros aplicados no relatório</span><span class="sxs-lookup"><span data-stu-id="ca758-162">Filters applied on the report</span></span>|
|<span data-ttu-id="ca758-163">select</span><span class="sxs-lookup"><span data-stu-id="ca758-163">select</span></span>|<span data-ttu-id="ca758-164">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca758-164">String collection</span></span>|<span data-ttu-id="ca758-165">Colunas selecionadas do relatório</span><span class="sxs-lookup"><span data-stu-id="ca758-165">Columns selected from the report</span></span>|
|<span data-ttu-id="ca758-166">Classificadoporativado</span><span class="sxs-lookup"><span data-stu-id="ca758-166">orderBy</span></span>|<span data-ttu-id="ca758-167">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca758-167">String collection</span></span>|<span data-ttu-id="ca758-168">Ordenação de colunas no relatório</span><span class="sxs-lookup"><span data-stu-id="ca758-168">Ordering of columns in the report</span></span>|
|<span data-ttu-id="ca758-169">formato</span><span class="sxs-lookup"><span data-stu-id="ca758-169">format</span></span>|[<span data-ttu-id="ca758-170">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="ca758-170">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="ca758-171">Formato do relatório agendado.</span><span class="sxs-lookup"><span data-stu-id="ca758-171">Format of the scheduled report.</span></span> <span data-ttu-id="ca758-172">Os valores possíveis são: `csv` e `pdf`.</span><span class="sxs-lookup"><span data-stu-id="ca758-172">Possible values are: `csv`, `pdf`.</span></span>|



## <a name="response"></a><span data-ttu-id="ca758-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca758-173">Response</span></span>
<span data-ttu-id="ca758-174">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca758-174">If successful, this method returns a `201 Created` response code and a [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca758-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca758-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca758-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca758-176">Request</span></span>
<span data-ttu-id="ca758-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca758-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ca758-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca758-178">Response</span></span>
<span data-ttu-id="ca758-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca758-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




