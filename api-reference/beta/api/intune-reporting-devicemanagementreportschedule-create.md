---
title: Criar deviceManagementReportSchedule
description: Criar um novo objeto deviceManagementReportSchedule.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0f91038e518550b9ebfc50d59c3a0168d8e489cd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49257622"
---
# <a name="create-devicemanagementreportschedule"></a><span data-ttu-id="6c7b8-103">Criar deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="6c7b8-103">Create deviceManagementReportSchedule</span></span>

<span data-ttu-id="6c7b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c7b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c7b8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6c7b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c7b8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6c7b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c7b8-107">Criar um novo objeto [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) .</span><span class="sxs-lookup"><span data-stu-id="6c7b8-107">Create a new [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c7b8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6c7b8-108">Prerequisites</span></span>
<span data-ttu-id="6c7b8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c7b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c7b8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c7b8-111">Permission type</span></span>|<span data-ttu-id="6c7b8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6c7b8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c7b8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c7b8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6c7b8-114">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6c7b8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6c7b8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c7b8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c7b8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c7b8-116">Not supported.</span></span>|
|<span data-ttu-id="6c7b8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c7b8-117">Application</span></span>|<span data-ttu-id="6c7b8-118">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6c7b8-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c7b8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c7b8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/reportSchedules
```

## <a name="request-headers"></a><span data-ttu-id="6c7b8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c7b8-120">Request headers</span></span>
|<span data-ttu-id="6c7b8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6c7b8-121">Header</span></span>|<span data-ttu-id="6c7b8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6c7b8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c7b8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c7b8-123">Authorization</span></span>|<span data-ttu-id="6c7b8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c7b8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c7b8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6c7b8-125">Accept</span></span>|<span data-ttu-id="6c7b8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6c7b8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c7b8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c7b8-127">Request body</span></span>
<span data-ttu-id="6c7b8-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementReportSchedule.</span><span class="sxs-lookup"><span data-stu-id="6c7b8-128">In the request body, supply a JSON representation for the deviceManagementReportSchedule object.</span></span>

<span data-ttu-id="6c7b8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementReportSchedule.</span><span class="sxs-lookup"><span data-stu-id="6c7b8-129">The following table shows the properties that are required when you create the deviceManagementReportSchedule.</span></span>

|<span data-ttu-id="6c7b8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c7b8-130">Property</span></span>|<span data-ttu-id="6c7b8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c7b8-131">Type</span></span>|<span data-ttu-id="6c7b8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c7b8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c7b8-133">id</span><span class="sxs-lookup"><span data-stu-id="6c7b8-133">id</span></span>|<span data-ttu-id="6c7b8-134">String</span><span class="sxs-lookup"><span data-stu-id="6c7b8-134">String</span></span>|<span data-ttu-id="6c7b8-135">Identificador exclusivo para esta entidade</span><span class="sxs-lookup"><span data-stu-id="6c7b8-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="6c7b8-136">reportScheduleName</span><span class="sxs-lookup"><span data-stu-id="6c7b8-136">reportScheduleName</span></span>|<span data-ttu-id="6c7b8-137">String</span><span class="sxs-lookup"><span data-stu-id="6c7b8-137">String</span></span>|<span data-ttu-id="6c7b8-138">Nome da agenda</span><span class="sxs-lookup"><span data-stu-id="6c7b8-138">Name of the schedule</span></span>|
|<span data-ttu-id="6c7b8-139">assunto</span><span class="sxs-lookup"><span data-stu-id="6c7b8-139">subject</span></span>|<span data-ttu-id="6c7b8-140">String</span><span class="sxs-lookup"><span data-stu-id="6c7b8-140">String</span></span>|<span data-ttu-id="6c7b8-141">Assunto dos relatórios agendados que são entregues</span><span class="sxs-lookup"><span data-stu-id="6c7b8-141">Subject of the scheduled reports that are delivered</span></span>|
|<span data-ttu-id="6c7b8-142">email</span><span class="sxs-lookup"><span data-stu-id="6c7b8-142">emails</span></span>|<span data-ttu-id="6c7b8-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c7b8-143">String collection</span></span>|<span data-ttu-id="6c7b8-144">Emails para os quais os relatórios agendados são entregues</span><span class="sxs-lookup"><span data-stu-id="6c7b8-144">Emails to which the scheduled reports are delivered</span></span>|
|<span data-ttu-id="6c7b8-145">recurrence</span><span class="sxs-lookup"><span data-stu-id="6c7b8-145">recurrence</span></span>|[<span data-ttu-id="6c7b8-146">deviceManagementScheduledReportRecurrence</span><span class="sxs-lookup"><span data-stu-id="6c7b8-146">deviceManagementScheduledReportRecurrence</span></span>](../resources/intune-reporting-devicemanagementscheduledreportrecurrence.md)|<span data-ttu-id="6c7b8-147">Frequência da entrega de relatórios agendados.</span><span class="sxs-lookup"><span data-stu-id="6c7b8-147">Frequency of scheduled report delivery.</span></span> <span data-ttu-id="6c7b8-148">Os valores possíveis são: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="6c7b8-148">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="6c7b8-149">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6c7b8-149">startDateTime</span></span>|<span data-ttu-id="6c7b8-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c7b8-150">DateTimeOffset</span></span>|<span data-ttu-id="6c7b8-151">Hora de início da entrega dos relatórios agendados</span><span class="sxs-lookup"><span data-stu-id="6c7b8-151">Time that the delivery of the scheduled reports starts</span></span>|
|<span data-ttu-id="6c7b8-152">endDateTime</span><span class="sxs-lookup"><span data-stu-id="6c7b8-152">endDateTime</span></span>|<span data-ttu-id="6c7b8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c7b8-153">DateTimeOffset</span></span>|<span data-ttu-id="6c7b8-154">Hora em que a entrega dos relatórios agendados termina</span><span class="sxs-lookup"><span data-stu-id="6c7b8-154">Time that the delivery of the scheduled reports ends</span></span>|
|<span data-ttu-id="6c7b8-155">userId</span><span class="sxs-lookup"><span data-stu-id="6c7b8-155">userId</span></span>|<span data-ttu-id="6c7b8-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c7b8-156">String</span></span>|<span data-ttu-id="6c7b8-157">A ID do usuário que criou o relatório</span><span class="sxs-lookup"><span data-stu-id="6c7b8-157">The Id of the User who created the report</span></span>|
|<span data-ttu-id="6c7b8-158">reportName</span><span class="sxs-lookup"><span data-stu-id="6c7b8-158">reportName</span></span>|<span data-ttu-id="6c7b8-159">String</span><span class="sxs-lookup"><span data-stu-id="6c7b8-159">String</span></span>|<span data-ttu-id="6c7b8-160">Nome do relatório</span><span class="sxs-lookup"><span data-stu-id="6c7b8-160">Name of the report</span></span>|
|<span data-ttu-id="6c7b8-161">filter</span><span class="sxs-lookup"><span data-stu-id="6c7b8-161">filter</span></span>|<span data-ttu-id="6c7b8-162">String</span><span class="sxs-lookup"><span data-stu-id="6c7b8-162">String</span></span>|<span data-ttu-id="6c7b8-163">Filtros aplicados no relatório</span><span class="sxs-lookup"><span data-stu-id="6c7b8-163">Filters applied on the report</span></span>|
|<span data-ttu-id="6c7b8-164">select</span><span class="sxs-lookup"><span data-stu-id="6c7b8-164">select</span></span>|<span data-ttu-id="6c7b8-165">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c7b8-165">String collection</span></span>|<span data-ttu-id="6c7b8-166">Colunas selecionadas do relatório</span><span class="sxs-lookup"><span data-stu-id="6c7b8-166">Columns selected from the report</span></span>|
|<span data-ttu-id="6c7b8-167">Classificadoporativado</span><span class="sxs-lookup"><span data-stu-id="6c7b8-167">orderBy</span></span>|<span data-ttu-id="6c7b8-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c7b8-168">String collection</span></span>|<span data-ttu-id="6c7b8-169">Ordenação de colunas no relatório</span><span class="sxs-lookup"><span data-stu-id="6c7b8-169">Ordering of columns in the report</span></span>|
|<span data-ttu-id="6c7b8-170">formato</span><span class="sxs-lookup"><span data-stu-id="6c7b8-170">format</span></span>|[<span data-ttu-id="6c7b8-171">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="6c7b8-171">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="6c7b8-172">Formato do relatório agendado.</span><span class="sxs-lookup"><span data-stu-id="6c7b8-172">Format of the scheduled report.</span></span> <span data-ttu-id="6c7b8-173">Os valores possíveis são: `csv` e `pdf`.</span><span class="sxs-lookup"><span data-stu-id="6c7b8-173">Possible values are: `csv`, `pdf`.</span></span>|



## <a name="response"></a><span data-ttu-id="6c7b8-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c7b8-174">Response</span></span>
<span data-ttu-id="6c7b8-175">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c7b8-175">If successful, this method returns a `201 Created` response code and a [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c7b8-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c7b8-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c7b8-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c7b8-177">Request</span></span>
<span data-ttu-id="6c7b8-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c7b8-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6c7b8-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c7b8-179">Response</span></span>
<span data-ttu-id="6c7b8-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c7b8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




