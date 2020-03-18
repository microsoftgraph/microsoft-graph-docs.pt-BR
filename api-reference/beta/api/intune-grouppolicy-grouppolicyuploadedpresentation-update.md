---
title: Atualizar groupPolicyUploadedPresentation
description: Atualiza as propriedades de um objeto groupPolicyUploadedPresentation.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 244cc9206679416cdfee4c7aee61d68b3de4de44
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803698"
---
# <a name="update-grouppolicyuploadedpresentation"></a><span data-ttu-id="1a1ad-103">Atualizar groupPolicyUploadedPresentation</span><span class="sxs-lookup"><span data-stu-id="1a1ad-103">Update groupPolicyUploadedPresentation</span></span>

> <span data-ttu-id="1a1ad-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1a1ad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a1ad-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1a1ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a1ad-106">Atualiza as propriedades de um objeto [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="1a1ad-106">Update the properties of a [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a1ad-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1a1ad-107">Prerequisites</span></span>
<span data-ttu-id="1a1ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a1ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a1ad-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a1ad-110">Permission type</span></span>|<span data-ttu-id="1a1ad-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1a1ad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a1ad-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a1ad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1a1ad-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a1ad-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1a1ad-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a1ad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a1ad-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a1ad-115">Not supported.</span></span>|
|<span data-ttu-id="1a1ad-116">Application</span><span class="sxs-lookup"><span data-stu-id="1a1ad-116">Application</span></span>|<span data-ttu-id="1a1ad-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a1ad-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a1ad-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a1ad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="1a1ad-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a1ad-119">Request headers</span></span>
|<span data-ttu-id="1a1ad-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1a1ad-120">Header</span></span>|<span data-ttu-id="1a1ad-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1a1ad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a1ad-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a1ad-122">Authorization</span></span>|<span data-ttu-id="1a1ad-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a1ad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a1ad-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1a1ad-124">Accept</span></span>|<span data-ttu-id="1a1ad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1a1ad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a1ad-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a1ad-126">Request body</span></span>
<span data-ttu-id="1a1ad-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="1a1ad-127">In the request body, supply a JSON representation for the [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object.</span></span>

<span data-ttu-id="1a1ad-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md).</span><span class="sxs-lookup"><span data-stu-id="1a1ad-128">The following table shows the properties that are required when you create the [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md).</span></span>

|<span data-ttu-id="1a1ad-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a1ad-129">Property</span></span>|<span data-ttu-id="1a1ad-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a1ad-130">Type</span></span>|<span data-ttu-id="1a1ad-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a1ad-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a1ad-132">rótulo</span><span class="sxs-lookup"><span data-stu-id="1a1ad-132">label</span></span>|<span data-ttu-id="1a1ad-133">String</span><span class="sxs-lookup"><span data-stu-id="1a1ad-133">String</span></span>|<span data-ttu-id="1a1ad-134">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="1a1ad-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="1a1ad-135">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="1a1ad-135">The default value is empty.</span></span> <span data-ttu-id="1a1ad-136">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="1a1ad-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="1a1ad-137">id</span><span class="sxs-lookup"><span data-stu-id="1a1ad-137">id</span></span>|<span data-ttu-id="1a1ad-138">String</span><span class="sxs-lookup"><span data-stu-id="1a1ad-138">String</span></span>|<span data-ttu-id="1a1ad-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1a1ad-139">Key of the entity.</span></span> <span data-ttu-id="1a1ad-140">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="1a1ad-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="1a1ad-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a1ad-141">lastModifiedDateTime</span></span>|<span data-ttu-id="1a1ad-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a1ad-142">DateTimeOffset</span></span>|<span data-ttu-id="1a1ad-143">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="1a1ad-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="1a1ad-144">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="1a1ad-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|



## <a name="response"></a><span data-ttu-id="1a1ad-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a1ad-145">Response</span></span>
<span data-ttu-id="1a1ad-146">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a1ad-146">If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a1ad-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1a1ad-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a1ad-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a1ad-148">Request</span></span>
<span data-ttu-id="1a1ad-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a1ad-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedPresentation",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="1a1ad-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a1ad-150">Response</span></span>
<span data-ttu-id="1a1ad-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1a1ad-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




