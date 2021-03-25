---
title: Atualizar securityBaselineStateSummary
description: Atualize as propriedades de um objeto securityBaselineStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: de1db7428f19e07f6bf7d349b00d995d93d0a660
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154515"
---
# <a name="update-securitybaselinestatesummary"></a><span data-ttu-id="e5104-103">Atualizar securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="e5104-103">Update securityBaselineStateSummary</span></span>

<span data-ttu-id="e5104-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5104-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5104-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e5104-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5104-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e5104-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5104-107">Atualize as propriedades de [um objeto securityBaselineStateSummary.](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="e5104-107">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5104-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e5104-108">Prerequisites</span></span>
<span data-ttu-id="e5104-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5104-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5104-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5104-111">Permission type</span></span>|<span data-ttu-id="e5104-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5104-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5104-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5104-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5104-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5104-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e5104-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5104-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5104-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5104-116">Not supported.</span></span>|
|<span data-ttu-id="e5104-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5104-117">Application</span></span>|<span data-ttu-id="e5104-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5104-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5104-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5104-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="e5104-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5104-120">Request headers</span></span>
|<span data-ttu-id="e5104-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e5104-121">Header</span></span>|<span data-ttu-id="e5104-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e5104-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5104-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5104-123">Authorization</span></span>|<span data-ttu-id="e5104-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5104-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5104-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e5104-125">Accept</span></span>|<span data-ttu-id="e5104-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5104-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5104-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5104-127">Request body</span></span>
<span data-ttu-id="e5104-128">No corpo da solicitação, fornece uma representação JSON para o [objeto securityBaselineStateSummary.](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="e5104-128">In the request body, supply a JSON representation for the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

<span data-ttu-id="e5104-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e5104-129">The following table shows the properties that are required when you create the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md).</span></span>

|<span data-ttu-id="e5104-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5104-130">Property</span></span>|<span data-ttu-id="e5104-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5104-131">Type</span></span>|<span data-ttu-id="e5104-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5104-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5104-133">id</span><span class="sxs-lookup"><span data-stu-id="e5104-133">id</span></span>|<span data-ttu-id="e5104-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5104-134">String</span></span>|<span data-ttu-id="e5104-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="e5104-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="e5104-136">secureCount</span><span class="sxs-lookup"><span data-stu-id="e5104-136">secureCount</span></span>|<span data-ttu-id="e5104-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e5104-137">Int32</span></span>|<span data-ttu-id="e5104-138">Número de dispositivos seguros</span><span class="sxs-lookup"><span data-stu-id="e5104-138">Number of secure devices</span></span>|
|<span data-ttu-id="e5104-139">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="e5104-139">notSecureCount</span></span>|<span data-ttu-id="e5104-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e5104-140">Int32</span></span>|<span data-ttu-id="e5104-141">Número de dispositivos não seguros</span><span class="sxs-lookup"><span data-stu-id="e5104-141">Number of not secure devices</span></span>|
|<span data-ttu-id="e5104-142">unknownCount</span><span class="sxs-lookup"><span data-stu-id="e5104-142">unknownCount</span></span>|<span data-ttu-id="e5104-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e5104-143">Int32</span></span>|<span data-ttu-id="e5104-144">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="e5104-144">Number of unknown devices</span></span>|
|<span data-ttu-id="e5104-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="e5104-145">errorCount</span></span>|<span data-ttu-id="e5104-146">Int32</span><span class="sxs-lookup"><span data-stu-id="e5104-146">Int32</span></span>|<span data-ttu-id="e5104-147">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="e5104-147">Number of error devices</span></span>|
|<span data-ttu-id="e5104-148">conflictCount</span><span class="sxs-lookup"><span data-stu-id="e5104-148">conflictCount</span></span>|<span data-ttu-id="e5104-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e5104-149">Int32</span></span>|<span data-ttu-id="e5104-150">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="e5104-150">Number of conflict devices</span></span>|
|<span data-ttu-id="e5104-151">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="e5104-151">notApplicableCount</span></span>|<span data-ttu-id="e5104-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e5104-152">Int32</span></span>|<span data-ttu-id="e5104-153">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="e5104-153">Number of not applicable devices</span></span>|



## <a name="response"></a><span data-ttu-id="e5104-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5104-154">Response</span></span>
<span data-ttu-id="e5104-155">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5104-155">If successful, this method returns a `200 OK` response code and an updated [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5104-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5104-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5104-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5104-157">Request</span></span>
<span data-ttu-id="e5104-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5104-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
Content-type: application/json
Content-length: 213

{
  "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2
}
```

### <a name="response"></a><span data-ttu-id="e5104-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5104-159">Response</span></span>
<span data-ttu-id="e5104-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e5104-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 262

{
  "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
  "id": "a4da796f-796f-a4da-6f79-daa46f79daa4",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2
}
```




