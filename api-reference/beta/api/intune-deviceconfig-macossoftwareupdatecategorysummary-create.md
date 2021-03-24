---
title: Criar macOSSoftwareUpdateCategorySummary
description: Crie um novo objeto macOSSoftwareUpdateCategorySummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cc47fac234f046d69235af431db9d75dc1093e40
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129710"
---
# <a name="create-macossoftwareupdatecategorysummary"></a><span data-ttu-id="4a928-103">Criar macOSSoftwareUpdateCategorySummary</span><span class="sxs-lookup"><span data-stu-id="4a928-103">Create macOSSoftwareUpdateCategorySummary</span></span>

<span data-ttu-id="4a928-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a928-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4a928-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4a928-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a928-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4a928-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a928-107">Crie um novo [objeto macOSSoftwareUpdateCategorySummary.](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)</span><span class="sxs-lookup"><span data-stu-id="4a928-107">Create a new [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a928-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4a928-108">Prerequisites</span></span>
<span data-ttu-id="4a928-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a928-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a928-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a928-111">Permission type</span></span>|<span data-ttu-id="4a928-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4a928-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a928-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a928-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4a928-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a928-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4a928-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a928-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a928-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a928-116">Not supported.</span></span>|
|<span data-ttu-id="4a928-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a928-117">Application</span></span>|<span data-ttu-id="4a928-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a928-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a928-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a928-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries
```

## <a name="request-headers"></a><span data-ttu-id="4a928-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a928-120">Request headers</span></span>
|<span data-ttu-id="4a928-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4a928-121">Header</span></span>|<span data-ttu-id="4a928-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4a928-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a928-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a928-123">Authorization</span></span>|<span data-ttu-id="4a928-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a928-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a928-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4a928-125">Accept</span></span>|<span data-ttu-id="4a928-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4a928-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a928-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a928-127">Request body</span></span>
<span data-ttu-id="4a928-128">No corpo da solicitação, fornece uma representação JSON para o objeto macOSSoftwareUpdateCategorySummary.</span><span class="sxs-lookup"><span data-stu-id="4a928-128">In the request body, supply a JSON representation for the macOSSoftwareUpdateCategorySummary object.</span></span>

<span data-ttu-id="4a928-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o macOSSoftwareUpdateCategorySummary.</span><span class="sxs-lookup"><span data-stu-id="4a928-129">The following table shows the properties that are required when you create the macOSSoftwareUpdateCategorySummary.</span></span>

|<span data-ttu-id="4a928-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a928-130">Property</span></span>|<span data-ttu-id="4a928-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a928-131">Type</span></span>|<span data-ttu-id="4a928-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a928-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a928-133">id</span><span class="sxs-lookup"><span data-stu-id="4a928-133">id</span></span>|<span data-ttu-id="4a928-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a928-134">String</span></span>|<span data-ttu-id="4a928-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4a928-135">Key of the entity.</span></span>|
|<span data-ttu-id="4a928-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4a928-136">displayName</span></span>|<span data-ttu-id="4a928-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a928-137">String</span></span>|<span data-ttu-id="4a928-138">O nome do relatório</span><span class="sxs-lookup"><span data-stu-id="4a928-138">The name of the report</span></span>|
|<span data-ttu-id="4a928-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="4a928-139">deviceId</span></span>|<span data-ttu-id="4a928-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a928-140">String</span></span>|<span data-ttu-id="4a928-141">A ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4a928-141">The device ID.</span></span>|
|<span data-ttu-id="4a928-142">userId</span><span class="sxs-lookup"><span data-stu-id="4a928-142">userId</span></span>|<span data-ttu-id="4a928-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a928-143">String</span></span>|<span data-ttu-id="4a928-144">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="4a928-144">The user ID.</span></span>|
|<span data-ttu-id="4a928-145">updateCategory</span><span class="sxs-lookup"><span data-stu-id="4a928-145">updateCategory</span></span>|[<span data-ttu-id="4a928-146">macOSSoftwareUpdateCategory</span><span class="sxs-lookup"><span data-stu-id="4a928-146">macOSSoftwareUpdateCategory</span></span>](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|<span data-ttu-id="4a928-147">Tipo de atualização de software.</span><span class="sxs-lookup"><span data-stu-id="4a928-147">Software update type.</span></span> <span data-ttu-id="4a928-148">Os valores possíveis são: `critical`, `configurationDataFile`, `firmware`, `other`.</span><span class="sxs-lookup"><span data-stu-id="4a928-148">Possible values are: `critical`, `configurationDataFile`, `firmware`, `other`.</span></span>|
|<span data-ttu-id="4a928-149">successfulUpdateCount</span><span class="sxs-lookup"><span data-stu-id="4a928-149">successfulUpdateCount</span></span>|<span data-ttu-id="4a928-150">Int32</span><span class="sxs-lookup"><span data-stu-id="4a928-150">Int32</span></span>|<span data-ttu-id="4a928-151">Número de atualizações bem-sucedidas no dispositivo</span><span class="sxs-lookup"><span data-stu-id="4a928-151">Number of successful updates on the device</span></span>|
|<span data-ttu-id="4a928-152">failedUpdateCount</span><span class="sxs-lookup"><span data-stu-id="4a928-152">failedUpdateCount</span></span>|<span data-ttu-id="4a928-153">Int32</span><span class="sxs-lookup"><span data-stu-id="4a928-153">Int32</span></span>|<span data-ttu-id="4a928-154">Número de atualizações com falha no dispositivo</span><span class="sxs-lookup"><span data-stu-id="4a928-154">Number of failed updates on the device</span></span>|
|<span data-ttu-id="4a928-155">totalUpdateCount</span><span class="sxs-lookup"><span data-stu-id="4a928-155">totalUpdateCount</span></span>|<span data-ttu-id="4a928-156">Int32</span><span class="sxs-lookup"><span data-stu-id="4a928-156">Int32</span></span>|<span data-ttu-id="4a928-157">Número de atualizações totais no dispositivo</span><span class="sxs-lookup"><span data-stu-id="4a928-157">Number of total updates on the device</span></span>|
|<span data-ttu-id="4a928-158">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a928-158">lastUpdatedDateTime</span></span>|<span data-ttu-id="4a928-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a928-159">DateTimeOffset</span></span>|<span data-ttu-id="4a928-160">Última data em que o relatório deste dispositivo foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="4a928-160">Last date time the report for this device was updated.</span></span>|



## <a name="response"></a><span data-ttu-id="4a928-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a928-161">Response</span></span>
<span data-ttu-id="4a928-162">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a928-162">If successful, this method returns a `201 Created` response code and a [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a928-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a928-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a928-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a928-164">Request</span></span>
<span data-ttu-id="4a928-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a928-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4a928-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a928-166">Response</span></span>
<span data-ttu-id="4a928-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a928-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




