---
title: Criar macOSSoftwareUpdateStateSummary
description: Criar um novo objeto macOSSoftwareUpdateStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e63b0cff6e35194a081edc376abad9462a1f1674
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704884"
---
# <a name="create-macossoftwareupdatestatesummary"></a><span data-ttu-id="5b559-103">Criar macOSSoftwareUpdateStateSummary</span><span class="sxs-lookup"><span data-stu-id="5b559-103">Create macOSSoftwareUpdateStateSummary</span></span>

<span data-ttu-id="5b559-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b559-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b559-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5b559-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b559-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5b559-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b559-107">Criar um novo objeto [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="5b559-107">Create a new [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b559-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5b559-108">Prerequisites</span></span>
<span data-ttu-id="5b559-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b559-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b559-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b559-111">Permission type</span></span>|<span data-ttu-id="5b559-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5b559-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b559-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b559-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b559-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b559-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5b559-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b559-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b559-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b559-116">Not supported.</span></span>|
|<span data-ttu-id="5b559-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b559-117">Application</span></span>|<span data-ttu-id="5b559-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b559-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b559-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b559-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}/updateStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="5b559-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b559-120">Request headers</span></span>
|<span data-ttu-id="5b559-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5b559-121">Header</span></span>|<span data-ttu-id="5b559-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5b559-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b559-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b559-123">Authorization</span></span>|<span data-ttu-id="5b559-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b559-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b559-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5b559-125">Accept</span></span>|<span data-ttu-id="5b559-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5b559-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b559-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b559-127">Request body</span></span>
<span data-ttu-id="5b559-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSSoftwareUpdateStateSummary.</span><span class="sxs-lookup"><span data-stu-id="5b559-128">In the request body, supply a JSON representation for the macOSSoftwareUpdateStateSummary object.</span></span>

<span data-ttu-id="5b559-129">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSSoftwareUpdateStateSummary.</span><span class="sxs-lookup"><span data-stu-id="5b559-129">The following table shows the properties that are required when you create the macOSSoftwareUpdateStateSummary.</span></span>

|<span data-ttu-id="5b559-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b559-130">Property</span></span>|<span data-ttu-id="5b559-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b559-131">Type</span></span>|<span data-ttu-id="5b559-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b559-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b559-133">id</span><span class="sxs-lookup"><span data-stu-id="5b559-133">id</span></span>|<span data-ttu-id="5b559-134">String</span><span class="sxs-lookup"><span data-stu-id="5b559-134">String</span></span>|<span data-ttu-id="5b559-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5b559-135">Key of the entity.</span></span>|
|<span data-ttu-id="5b559-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5b559-136">displayName</span></span>|<span data-ttu-id="5b559-137">String</span><span class="sxs-lookup"><span data-stu-id="5b559-137">String</span></span>|<span data-ttu-id="5b559-138">Nome da atualização de software legível por pessoas</span><span class="sxs-lookup"><span data-stu-id="5b559-138">Human readable name of the software update</span></span>|
|<span data-ttu-id="5b559-139">productKey</span><span class="sxs-lookup"><span data-stu-id="5b559-139">productKey</span></span>|<span data-ttu-id="5b559-140">String</span><span class="sxs-lookup"><span data-stu-id="5b559-140">String</span></span>|<span data-ttu-id="5b559-141">Chave de produto da atualização de software.</span><span class="sxs-lookup"><span data-stu-id="5b559-141">Product key of the software update.</span></span>|
|<span data-ttu-id="5b559-142">updateCategory</span><span class="sxs-lookup"><span data-stu-id="5b559-142">updateCategory</span></span>|[<span data-ttu-id="5b559-143">macOSSoftwareUpdateCategory</span><span class="sxs-lookup"><span data-stu-id="5b559-143">macOSSoftwareUpdateCategory</span></span>](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|<span data-ttu-id="5b559-144">Categoria de atualização de software.</span><span class="sxs-lookup"><span data-stu-id="5b559-144">Software update category.</span></span> <span data-ttu-id="5b559-145">Os valores possíveis são: `critical`, `configurationDataFile`, `firmware`, `other`.</span><span class="sxs-lookup"><span data-stu-id="5b559-145">Possible values are: `critical`, `configurationDataFile`, `firmware`, `other`.</span></span>|
|<span data-ttu-id="5b559-146">updateVersion</span><span class="sxs-lookup"><span data-stu-id="5b559-146">updateVersion</span></span>|<span data-ttu-id="5b559-147">String</span><span class="sxs-lookup"><span data-stu-id="5b559-147">String</span></span>|<span data-ttu-id="5b559-148">Versão da atualização de software</span><span class="sxs-lookup"><span data-stu-id="5b559-148">Version of the software update</span></span>|
|<span data-ttu-id="5b559-149">state</span><span class="sxs-lookup"><span data-stu-id="5b559-149">state</span></span>|[<span data-ttu-id="5b559-150">macOSSoftwareUpdateState</span><span class="sxs-lookup"><span data-stu-id="5b559-150">macOSSoftwareUpdateState</span></span>](../resources/intune-deviceconfig-macossoftwareupdatestate.md)|<span data-ttu-id="5b559-151">Estado da atualização de software.</span><span class="sxs-lookup"><span data-stu-id="5b559-151">State of the software update.</span></span> <span data-ttu-id="5b559-152">Os valores possíveis são:, `success` `downloading` , `downloaded` , `installing` , `idle` , `available` , `scheduled` , `downloadFailed` , `downloadInsufficientSpace` , `downloadInsufficientPower` , `downloadInsufficientNetwork` , `installInsufficientSpace` ,, `installInsufficientPower` `installFailed` `commandFailed` .</span><span class="sxs-lookup"><span data-stu-id="5b559-152">Possible values are: `success`, `downloading`, `downloaded`, `installing`, `idle`, `available`, `scheduled`, `downloadFailed`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installInsufficientSpace`, `installInsufficientPower`, `installFailed`, `commandFailed`.</span></span>|
|<span data-ttu-id="5b559-153">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="5b559-153">lastUpdatedDateTime</span></span>|<span data-ttu-id="5b559-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b559-154">DateTimeOffset</span></span>|<span data-ttu-id="5b559-155">Hora da última data em que o relatório para este dispositivo e chave do produto foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="5b559-155">Last date time the report for this device and product key was updated.</span></span>|



## <a name="response"></a><span data-ttu-id="5b559-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b559-156">Response</span></span>
<span data-ttu-id="5b559-157">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b559-157">If successful, this method returns a `201 Created` response code and a [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b559-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b559-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b559-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b559-159">Request</span></span>
<span data-ttu-id="5b559-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b559-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}/updateStateSummaries
Content-type: application/json
Content-length: 331

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateStateSummary",
  "displayName": "Display Name value",
  "productKey": "Product Key value",
  "updateCategory": "configurationDataFile",
  "updateVersion": "Update Version value",
  "state": "downloading",
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```

### <a name="response"></a><span data-ttu-id="5b559-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b559-161">Response</span></span>
<span data-ttu-id="5b559-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b559-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 380

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateStateSummary",
  "id": "9527a1df-a1df-9527-dfa1-2795dfa12795",
  "displayName": "Display Name value",
  "productKey": "Product Key value",
  "updateCategory": "configurationDataFile",
  "updateVersion": "Update Version value",
  "state": "downloading",
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```





