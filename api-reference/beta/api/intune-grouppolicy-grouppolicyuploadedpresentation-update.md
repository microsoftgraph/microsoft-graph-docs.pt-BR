---
title: Atualizar groupPolicyUploadedPresentation
description: Atualiza as propriedades de um objeto groupPolicyUploadedPresentation.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1477903f2dea9179f4691fddf933b6f8491102de
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42463746"
---
# <a name="update-grouppolicyuploadedpresentation"></a><span data-ttu-id="78e79-103">Atualizar groupPolicyUploadedPresentation</span><span class="sxs-lookup"><span data-stu-id="78e79-103">Update groupPolicyUploadedPresentation</span></span>

<span data-ttu-id="78e79-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="78e79-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78e79-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="78e79-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78e79-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="78e79-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78e79-107">Atualiza as propriedades de um objeto [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="78e79-107">Update the properties of a [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78e79-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="78e79-108">Prerequisites</span></span>
<span data-ttu-id="78e79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78e79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78e79-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78e79-111">Permission type</span></span>|<span data-ttu-id="78e79-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="78e79-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78e79-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78e79-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78e79-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78e79-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="78e79-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78e79-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78e79-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78e79-116">Not supported.</span></span>|
|<span data-ttu-id="78e79-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78e79-117">Application</span></span>|<span data-ttu-id="78e79-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78e79-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="78e79-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78e79-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="78e79-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78e79-120">Request headers</span></span>
|<span data-ttu-id="78e79-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="78e79-121">Header</span></span>|<span data-ttu-id="78e79-122">Valor</span><span class="sxs-lookup"><span data-stu-id="78e79-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78e79-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="78e79-123">Authorization</span></span>|<span data-ttu-id="78e79-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78e79-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78e79-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="78e79-125">Accept</span></span>|<span data-ttu-id="78e79-126">application/json</span><span class="sxs-lookup"><span data-stu-id="78e79-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78e79-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78e79-127">Request body</span></span>
<span data-ttu-id="78e79-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="78e79-128">In the request body, supply a JSON representation for the [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object.</span></span>

<span data-ttu-id="78e79-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md).</span><span class="sxs-lookup"><span data-stu-id="78e79-129">The following table shows the properties that are required when you create the [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md).</span></span>

|<span data-ttu-id="78e79-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78e79-130">Property</span></span>|<span data-ttu-id="78e79-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="78e79-131">Type</span></span>|<span data-ttu-id="78e79-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="78e79-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78e79-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="78e79-133">label</span></span>|<span data-ttu-id="78e79-134">String</span><span class="sxs-lookup"><span data-stu-id="78e79-134">String</span></span>|<span data-ttu-id="78e79-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="78e79-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="78e79-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="78e79-136">The default value is empty.</span></span> <span data-ttu-id="78e79-137">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="78e79-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="78e79-138">id</span><span class="sxs-lookup"><span data-stu-id="78e79-138">id</span></span>|<span data-ttu-id="78e79-139">String</span><span class="sxs-lookup"><span data-stu-id="78e79-139">String</span></span>|<span data-ttu-id="78e79-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="78e79-140">Key of the entity.</span></span> <span data-ttu-id="78e79-141">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="78e79-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="78e79-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="78e79-142">lastModifiedDateTime</span></span>|<span data-ttu-id="78e79-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78e79-143">DateTimeOffset</span></span>|<span data-ttu-id="78e79-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="78e79-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="78e79-145">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="78e79-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|



## <a name="response"></a><span data-ttu-id="78e79-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="78e79-146">Response</span></span>
<span data-ttu-id="78e79-147">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78e79-147">If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78e79-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78e79-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="78e79-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78e79-149">Request</span></span>
<span data-ttu-id="78e79-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78e79-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedPresentation",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="78e79-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="78e79-151">Response</span></span>
<span data-ttu-id="78e79-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="78e79-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 213

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedPresentation",
  "label": "Label value",
  "id": "b9f611e8-11e8-b9f6-e811-f6b9e811f6b9",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





