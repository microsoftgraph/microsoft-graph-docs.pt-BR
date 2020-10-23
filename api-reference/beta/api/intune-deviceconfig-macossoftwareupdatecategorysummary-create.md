---
title: Criar macOSSoftwareUpdateCategorySummary
description: Criar um novo objeto macOSSoftwareUpdateCategorySummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 10e3abc075272622cfdb605e8289ee5d2c3633ed
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731824"
---
# <a name="create-macossoftwareupdatecategorysummary"></a><span data-ttu-id="3a1e8-103">Criar macOSSoftwareUpdateCategorySummary</span><span class="sxs-lookup"><span data-stu-id="3a1e8-103">Create macOSSoftwareUpdateCategorySummary</span></span>

<span data-ttu-id="3a1e8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a1e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a1e8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3a1e8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a1e8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3a1e8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a1e8-107">Criar um novo objeto [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) .</span><span class="sxs-lookup"><span data-stu-id="3a1e8-107">Create a new [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a1e8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3a1e8-108">Prerequisites</span></span>
<span data-ttu-id="3a1e8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a1e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a1e8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a1e8-111">Permission type</span></span>|<span data-ttu-id="3a1e8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3a1e8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a1e8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a1e8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a1e8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a1e8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3a1e8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a1e8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a1e8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a1e8-116">Not supported.</span></span>|
|<span data-ttu-id="3a1e8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a1e8-117">Application</span></span>|<span data-ttu-id="3a1e8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a1e8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a1e8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a1e8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries
```

## <a name="request-headers"></a><span data-ttu-id="3a1e8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a1e8-120">Request headers</span></span>
|<span data-ttu-id="3a1e8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3a1e8-121">Header</span></span>|<span data-ttu-id="3a1e8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3a1e8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a1e8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a1e8-123">Authorization</span></span>|<span data-ttu-id="3a1e8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a1e8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a1e8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3a1e8-125">Accept</span></span>|<span data-ttu-id="3a1e8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a1e8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a1e8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a1e8-127">Request body</span></span>
<span data-ttu-id="3a1e8-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSSoftwareUpdateCategorySummary.</span><span class="sxs-lookup"><span data-stu-id="3a1e8-128">In the request body, supply a JSON representation for the macOSSoftwareUpdateCategorySummary object.</span></span>

<span data-ttu-id="3a1e8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSSoftwareUpdateCategorySummary.</span><span class="sxs-lookup"><span data-stu-id="3a1e8-129">The following table shows the properties that are required when you create the macOSSoftwareUpdateCategorySummary.</span></span>

|<span data-ttu-id="3a1e8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a1e8-130">Property</span></span>|<span data-ttu-id="3a1e8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a1e8-131">Type</span></span>|<span data-ttu-id="3a1e8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a1e8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a1e8-133">id</span><span class="sxs-lookup"><span data-stu-id="3a1e8-133">id</span></span>|<span data-ttu-id="3a1e8-134">String</span><span class="sxs-lookup"><span data-stu-id="3a1e8-134">String</span></span>|<span data-ttu-id="3a1e8-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3a1e8-135">Key of the entity.</span></span>|
|<span data-ttu-id="3a1e8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3a1e8-136">displayName</span></span>|<span data-ttu-id="3a1e8-137">String</span><span class="sxs-lookup"><span data-stu-id="3a1e8-137">String</span></span>|<span data-ttu-id="3a1e8-138">O nome do relatório</span><span class="sxs-lookup"><span data-stu-id="3a1e8-138">The name of the report</span></span>|
|<span data-ttu-id="3a1e8-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="3a1e8-139">deviceId</span></span>|<span data-ttu-id="3a1e8-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a1e8-140">String</span></span>|<span data-ttu-id="3a1e8-141">A ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3a1e8-141">The device ID.</span></span>|
|<span data-ttu-id="3a1e8-142">userId</span><span class="sxs-lookup"><span data-stu-id="3a1e8-142">userId</span></span>|<span data-ttu-id="3a1e8-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a1e8-143">String</span></span>|<span data-ttu-id="3a1e8-144">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="3a1e8-144">The user ID.</span></span>|
|<span data-ttu-id="3a1e8-145">updateCategory</span><span class="sxs-lookup"><span data-stu-id="3a1e8-145">updateCategory</span></span>|[<span data-ttu-id="3a1e8-146">macOSSoftwareUpdateCategory</span><span class="sxs-lookup"><span data-stu-id="3a1e8-146">macOSSoftwareUpdateCategory</span></span>](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|<span data-ttu-id="3a1e8-147">Tipo de atualização de software.</span><span class="sxs-lookup"><span data-stu-id="3a1e8-147">Software update type.</span></span> <span data-ttu-id="3a1e8-148">Os valores possíveis são: `critical`, `configurationDataFile`, `firmware`, `other`.</span><span class="sxs-lookup"><span data-stu-id="3a1e8-148">Possible values are: `critical`, `configurationDataFile`, `firmware`, `other`.</span></span>|
|<span data-ttu-id="3a1e8-149">successfulUpdateCount</span><span class="sxs-lookup"><span data-stu-id="3a1e8-149">successfulUpdateCount</span></span>|<span data-ttu-id="3a1e8-150">Int32</span><span class="sxs-lookup"><span data-stu-id="3a1e8-150">Int32</span></span>|<span data-ttu-id="3a1e8-151">Número de atualizações bem-sucedidas no dispositivo</span><span class="sxs-lookup"><span data-stu-id="3a1e8-151">Number of successful updates on the device</span></span>|
|<span data-ttu-id="3a1e8-152">failedUpdateCount</span><span class="sxs-lookup"><span data-stu-id="3a1e8-152">failedUpdateCount</span></span>|<span data-ttu-id="3a1e8-153">Int32</span><span class="sxs-lookup"><span data-stu-id="3a1e8-153">Int32</span></span>|<span data-ttu-id="3a1e8-154">Número de atualizações com falha no dispositivo</span><span class="sxs-lookup"><span data-stu-id="3a1e8-154">Number of failed updates on the device</span></span>|
|<span data-ttu-id="3a1e8-155">totalUpdateCount</span><span class="sxs-lookup"><span data-stu-id="3a1e8-155">totalUpdateCount</span></span>|<span data-ttu-id="3a1e8-156">Int32</span><span class="sxs-lookup"><span data-stu-id="3a1e8-156">Int32</span></span>|<span data-ttu-id="3a1e8-157">Número do total de atualizações no dispositivo</span><span class="sxs-lookup"><span data-stu-id="3a1e8-157">Number of total updates on the device</span></span>|
|<span data-ttu-id="3a1e8-158">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a1e8-158">lastUpdatedDateTime</span></span>|<span data-ttu-id="3a1e8-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a1e8-159">DateTimeOffset</span></span>|<span data-ttu-id="3a1e8-160">Hora da última data em que o relatório para este dispositivo foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="3a1e8-160">Last date time the report for this device was updated.</span></span>|



## <a name="response"></a><span data-ttu-id="3a1e8-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a1e8-161">Response</span></span>
<span data-ttu-id="3a1e8-162">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a1e8-162">If successful, this method returns a `201 Created` response code and a [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a1e8-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a1e8-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a1e8-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a1e8-164">Request</span></span>
<span data-ttu-id="3a1e8-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a1e8-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries
Content-type: application/json
Content-length: 373

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateCategorySummary",
  "displayName": "Display Name value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "updateCategory": "configurationDataFile",
  "successfulUpdateCount": 5,
  "failedUpdateCount": 1,
  "totalUpdateCount": 0,
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```

### <a name="response"></a><span data-ttu-id="3a1e8-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a1e8-166">Response</span></span>
<span data-ttu-id="3a1e8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a1e8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 422

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateCategorySummary",
  "id": "f1fda232-a232-f1fd-32a2-fdf132a2fdf1",
  "displayName": "Display Name value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "updateCategory": "configurationDataFile",
  "successfulUpdateCount": 5,
  "failedUpdateCount": 1,
  "totalUpdateCount": 0,
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```





