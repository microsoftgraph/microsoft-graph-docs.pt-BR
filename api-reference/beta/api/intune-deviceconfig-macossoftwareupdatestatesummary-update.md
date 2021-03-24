---
title: Atualizar macOSSoftwareUpdateStateSummary
description: Atualize as propriedades de um objeto macOSSoftwareUpdateStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 405f1590c2f21a2de14a9611136f17c2b24ce0ba
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132601"
---
# <a name="update-macossoftwareupdatestatesummary"></a><span data-ttu-id="4ec73-103">Atualizar macOSSoftwareUpdateStateSummary</span><span class="sxs-lookup"><span data-stu-id="4ec73-103">Update macOSSoftwareUpdateStateSummary</span></span>

<span data-ttu-id="4ec73-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ec73-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ec73-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4ec73-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ec73-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4ec73-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ec73-107">Atualize as propriedades de [um objeto macOSSoftwareUpdateStateSummary.](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="4ec73-107">Update the properties of a [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ec73-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4ec73-108">Prerequisites</span></span>
<span data-ttu-id="4ec73-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ec73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ec73-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ec73-111">Permission type</span></span>|<span data-ttu-id="4ec73-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4ec73-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ec73-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ec73-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4ec73-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ec73-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4ec73-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ec73-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ec73-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ec73-116">Not supported.</span></span>|
|<span data-ttu-id="4ec73-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ec73-117">Application</span></span>|<span data-ttu-id="4ec73-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ec73-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ec73-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ec73-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}/updateStateSummaries/{macOSSoftwareUpdateStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="4ec73-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ec73-120">Request headers</span></span>
|<span data-ttu-id="4ec73-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4ec73-121">Header</span></span>|<span data-ttu-id="4ec73-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4ec73-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ec73-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ec73-123">Authorization</span></span>|<span data-ttu-id="4ec73-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ec73-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ec73-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4ec73-125">Accept</span></span>|<span data-ttu-id="4ec73-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4ec73-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ec73-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ec73-127">Request body</span></span>
<span data-ttu-id="4ec73-128">No corpo da solicitação, fornece uma representação JSON para o [objeto macOSSoftwareUpdateStateSummary.](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="4ec73-128">In the request body, supply a JSON representation for the [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) object.</span></span>

<span data-ttu-id="4ec73-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="4ec73-129">The following table shows the properties that are required when you create the [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md).</span></span>

|<span data-ttu-id="4ec73-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ec73-130">Property</span></span>|<span data-ttu-id="4ec73-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ec73-131">Type</span></span>|<span data-ttu-id="4ec73-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ec73-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ec73-133">id</span><span class="sxs-lookup"><span data-stu-id="4ec73-133">id</span></span>|<span data-ttu-id="4ec73-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ec73-134">String</span></span>|<span data-ttu-id="4ec73-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4ec73-135">Key of the entity.</span></span>|
|<span data-ttu-id="4ec73-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4ec73-136">displayName</span></span>|<span data-ttu-id="4ec73-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ec73-137">String</span></span>|<span data-ttu-id="4ec73-138">Nome acessível humano da atualização de software</span><span class="sxs-lookup"><span data-stu-id="4ec73-138">Human readable name of the software update</span></span>|
|<span data-ttu-id="4ec73-139">productKey</span><span class="sxs-lookup"><span data-stu-id="4ec73-139">productKey</span></span>|<span data-ttu-id="4ec73-140">String</span><span class="sxs-lookup"><span data-stu-id="4ec73-140">String</span></span>|<span data-ttu-id="4ec73-141">Chave do produto da atualização de software.</span><span class="sxs-lookup"><span data-stu-id="4ec73-141">Product key of the software update.</span></span>|
|<span data-ttu-id="4ec73-142">updateCategory</span><span class="sxs-lookup"><span data-stu-id="4ec73-142">updateCategory</span></span>|[<span data-ttu-id="4ec73-143">macOSSoftwareUpdateCategory</span><span class="sxs-lookup"><span data-stu-id="4ec73-143">macOSSoftwareUpdateCategory</span></span>](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|<span data-ttu-id="4ec73-144">Categoria de atualização de software.</span><span class="sxs-lookup"><span data-stu-id="4ec73-144">Software update category.</span></span> <span data-ttu-id="4ec73-145">Os valores possíveis são: `critical`, `configurationDataFile`, `firmware`, `other`.</span><span class="sxs-lookup"><span data-stu-id="4ec73-145">Possible values are: `critical`, `configurationDataFile`, `firmware`, `other`.</span></span>|
|<span data-ttu-id="4ec73-146">updateVersion</span><span class="sxs-lookup"><span data-stu-id="4ec73-146">updateVersion</span></span>|<span data-ttu-id="4ec73-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ec73-147">String</span></span>|<span data-ttu-id="4ec73-148">Versão da atualização de software</span><span class="sxs-lookup"><span data-stu-id="4ec73-148">Version of the software update</span></span>|
|<span data-ttu-id="4ec73-149">state</span><span class="sxs-lookup"><span data-stu-id="4ec73-149">state</span></span>|[<span data-ttu-id="4ec73-150">macOSSoftwareUpdateState</span><span class="sxs-lookup"><span data-stu-id="4ec73-150">macOSSoftwareUpdateState</span></span>](../resources/intune-deviceconfig-macossoftwareupdatestate.md)|<span data-ttu-id="4ec73-151">Estado da atualização de software.</span><span class="sxs-lookup"><span data-stu-id="4ec73-151">State of the software update.</span></span> <span data-ttu-id="4ec73-152">Os valores possíveis são: `success` , , , , , , , , , `downloading` , , `downloaded` , , , `installing` `idle` `available` , `scheduled` `downloadFailed` `downloadInsufficientSpace` `downloadInsufficientPower` `downloadInsufficientNetwork` `installInsufficientSpace` `installInsufficientPower` `installFailed` `commandFailed` .</span><span class="sxs-lookup"><span data-stu-id="4ec73-152">Possible values are: `success`, `downloading`, `downloaded`, `installing`, `idle`, `available`, `scheduled`, `downloadFailed`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installInsufficientSpace`, `installInsufficientPower`, `installFailed`, `commandFailed`.</span></span>|
|<span data-ttu-id="4ec73-153">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ec73-153">lastUpdatedDateTime</span></span>|<span data-ttu-id="4ec73-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ec73-154">DateTimeOffset</span></span>|<span data-ttu-id="4ec73-155">Última data em que o relatório para este dispositivo e a chave do produto foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="4ec73-155">Last date time the report for this device and product key was updated.</span></span>|



## <a name="response"></a><span data-ttu-id="4ec73-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ec73-156">Response</span></span>
<span data-ttu-id="4ec73-157">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ec73-157">If successful, this method returns a `200 OK` response code and an updated [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ec73-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ec73-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ec73-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ec73-159">Request</span></span>
<span data-ttu-id="4ec73-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ec73-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}/updateStateSummaries/{macOSSoftwareUpdateStateSummaryId}
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

### <a name="response"></a><span data-ttu-id="4ec73-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ec73-161">Response</span></span>
<span data-ttu-id="4ec73-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ec73-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




