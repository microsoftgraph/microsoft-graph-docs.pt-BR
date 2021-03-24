---
title: Atualizar macOSSoftwareUpdateCategorySummary
description: Atualize as propriedades de um objeto macOSSoftwareUpdateCategorySummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 92a8f014f94b3639a41ace8d7b40ba30e5a06aa6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131222"
---
# <a name="update-macossoftwareupdatecategorysummary"></a><span data-ttu-id="00203-103">Atualizar macOSSoftwareUpdateCategorySummary</span><span class="sxs-lookup"><span data-stu-id="00203-103">Update macOSSoftwareUpdateCategorySummary</span></span>

<span data-ttu-id="00203-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00203-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00203-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="00203-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00203-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="00203-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00203-107">Atualize as propriedades de [um objeto macOSSoftwareUpdateCategorySummary.](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)</span><span class="sxs-lookup"><span data-stu-id="00203-107">Update the properties of a [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00203-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="00203-108">Prerequisites</span></span>
<span data-ttu-id="00203-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00203-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00203-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00203-111">Permission type</span></span>|<span data-ttu-id="00203-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="00203-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00203-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00203-113">Delegated (work or school account)</span></span>|<span data-ttu-id="00203-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00203-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="00203-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00203-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00203-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00203-116">Not supported.</span></span>|
|<span data-ttu-id="00203-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00203-117">Application</span></span>|<span data-ttu-id="00203-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00203-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="00203-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00203-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="00203-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00203-120">Request headers</span></span>
|<span data-ttu-id="00203-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="00203-121">Header</span></span>|<span data-ttu-id="00203-122">Valor</span><span class="sxs-lookup"><span data-stu-id="00203-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00203-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="00203-123">Authorization</span></span>|<span data-ttu-id="00203-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00203-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00203-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="00203-125">Accept</span></span>|<span data-ttu-id="00203-126">application/json</span><span class="sxs-lookup"><span data-stu-id="00203-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00203-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00203-127">Request body</span></span>
<span data-ttu-id="00203-128">No corpo da solicitação, fornece uma representação JSON para o [objeto macOSSoftwareUpdateCategorySummary.](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)</span><span class="sxs-lookup"><span data-stu-id="00203-128">In the request body, supply a JSON representation for the [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) object.</span></span>

<span data-ttu-id="00203-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md).</span><span class="sxs-lookup"><span data-stu-id="00203-129">The following table shows the properties that are required when you create the [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md).</span></span>

|<span data-ttu-id="00203-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00203-130">Property</span></span>|<span data-ttu-id="00203-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="00203-131">Type</span></span>|<span data-ttu-id="00203-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="00203-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00203-133">id</span><span class="sxs-lookup"><span data-stu-id="00203-133">id</span></span>|<span data-ttu-id="00203-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00203-134">String</span></span>|<span data-ttu-id="00203-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="00203-135">Key of the entity.</span></span>|
|<span data-ttu-id="00203-136">displayName</span><span class="sxs-lookup"><span data-stu-id="00203-136">displayName</span></span>|<span data-ttu-id="00203-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00203-137">String</span></span>|<span data-ttu-id="00203-138">O nome do relatório</span><span class="sxs-lookup"><span data-stu-id="00203-138">The name of the report</span></span>|
|<span data-ttu-id="00203-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="00203-139">deviceId</span></span>|<span data-ttu-id="00203-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00203-140">String</span></span>|<span data-ttu-id="00203-141">A ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00203-141">The device ID.</span></span>|
|<span data-ttu-id="00203-142">userId</span><span class="sxs-lookup"><span data-stu-id="00203-142">userId</span></span>|<span data-ttu-id="00203-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00203-143">String</span></span>|<span data-ttu-id="00203-144">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="00203-144">The user ID.</span></span>|
|<span data-ttu-id="00203-145">updateCategory</span><span class="sxs-lookup"><span data-stu-id="00203-145">updateCategory</span></span>|[<span data-ttu-id="00203-146">macOSSoftwareUpdateCategory</span><span class="sxs-lookup"><span data-stu-id="00203-146">macOSSoftwareUpdateCategory</span></span>](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|<span data-ttu-id="00203-147">Tipo de atualização de software.</span><span class="sxs-lookup"><span data-stu-id="00203-147">Software update type.</span></span> <span data-ttu-id="00203-148">Os valores possíveis são: `critical`, `configurationDataFile`, `firmware`, `other`.</span><span class="sxs-lookup"><span data-stu-id="00203-148">Possible values are: `critical`, `configurationDataFile`, `firmware`, `other`.</span></span>|
|<span data-ttu-id="00203-149">successfulUpdateCount</span><span class="sxs-lookup"><span data-stu-id="00203-149">successfulUpdateCount</span></span>|<span data-ttu-id="00203-150">Int32</span><span class="sxs-lookup"><span data-stu-id="00203-150">Int32</span></span>|<span data-ttu-id="00203-151">Número de atualizações bem-sucedidas no dispositivo</span><span class="sxs-lookup"><span data-stu-id="00203-151">Number of successful updates on the device</span></span>|
|<span data-ttu-id="00203-152">failedUpdateCount</span><span class="sxs-lookup"><span data-stu-id="00203-152">failedUpdateCount</span></span>|<span data-ttu-id="00203-153">Int32</span><span class="sxs-lookup"><span data-stu-id="00203-153">Int32</span></span>|<span data-ttu-id="00203-154">Número de atualizações com falha no dispositivo</span><span class="sxs-lookup"><span data-stu-id="00203-154">Number of failed updates on the device</span></span>|
|<span data-ttu-id="00203-155">totalUpdateCount</span><span class="sxs-lookup"><span data-stu-id="00203-155">totalUpdateCount</span></span>|<span data-ttu-id="00203-156">Int32</span><span class="sxs-lookup"><span data-stu-id="00203-156">Int32</span></span>|<span data-ttu-id="00203-157">Número de atualizações totais no dispositivo</span><span class="sxs-lookup"><span data-stu-id="00203-157">Number of total updates on the device</span></span>|
|<span data-ttu-id="00203-158">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="00203-158">lastUpdatedDateTime</span></span>|<span data-ttu-id="00203-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00203-159">DateTimeOffset</span></span>|<span data-ttu-id="00203-160">Última data em que o relatório deste dispositivo foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="00203-160">Last date time the report for this device was updated.</span></span>|



## <a name="response"></a><span data-ttu-id="00203-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="00203-161">Response</span></span>
<span data-ttu-id="00203-162">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00203-162">If successful, this method returns a `200 OK` response code and an updated [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00203-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="00203-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="00203-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00203-164">Request</span></span>
<span data-ttu-id="00203-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="00203-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}
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

### <a name="response"></a><span data-ttu-id="00203-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="00203-166">Response</span></span>
<span data-ttu-id="00203-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="00203-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




