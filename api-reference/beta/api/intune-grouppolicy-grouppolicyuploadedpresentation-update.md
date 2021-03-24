---
title: Atualizar groupPolicyUploadedPresentation
description: Atualize as propriedades de um objeto groupPolicyUploadedPresentation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fd427ea574e8abe971863954c5817321eea14115
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145534"
---
# <a name="update-grouppolicyuploadedpresentation"></a><span data-ttu-id="ea708-103">Atualizar groupPolicyUploadedPresentation</span><span class="sxs-lookup"><span data-stu-id="ea708-103">Update groupPolicyUploadedPresentation</span></span>

<span data-ttu-id="ea708-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea708-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea708-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ea708-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea708-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ea708-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea708-107">Atualize as propriedades de [um objeto groupPolicyUploadedPresentation.](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ea708-107">Update the properties of a [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea708-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ea708-108">Prerequisites</span></span>
<span data-ttu-id="ea708-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea708-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea708-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea708-111">Permission type</span></span>|<span data-ttu-id="ea708-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ea708-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea708-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea708-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea708-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea708-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ea708-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea708-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea708-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea708-116">Not supported.</span></span>|
|<span data-ttu-id="ea708-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea708-117">Application</span></span>|<span data-ttu-id="ea708-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea708-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea708-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea708-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="ea708-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea708-120">Request headers</span></span>
|<span data-ttu-id="ea708-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ea708-121">Header</span></span>|<span data-ttu-id="ea708-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ea708-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea708-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea708-123">Authorization</span></span>|<span data-ttu-id="ea708-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea708-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea708-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ea708-125">Accept</span></span>|<span data-ttu-id="ea708-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ea708-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea708-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea708-127">Request body</span></span>
<span data-ttu-id="ea708-128">No corpo da solicitação, fornece uma representação JSON para [o objeto groupPolicyUploadedPresentation.](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ea708-128">In the request body, supply a JSON representation for the [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object.</span></span>

<span data-ttu-id="ea708-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md).</span><span class="sxs-lookup"><span data-stu-id="ea708-129">The following table shows the properties that are required when you create the [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md).</span></span>

|<span data-ttu-id="ea708-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea708-130">Property</span></span>|<span data-ttu-id="ea708-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea708-131">Type</span></span>|<span data-ttu-id="ea708-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea708-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea708-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="ea708-133">label</span></span>|<span data-ttu-id="ea708-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea708-134">String</span></span>|<span data-ttu-id="ea708-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="ea708-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="ea708-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="ea708-136">The default value is empty.</span></span> <span data-ttu-id="ea708-137">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ea708-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ea708-138">id</span><span class="sxs-lookup"><span data-stu-id="ea708-138">id</span></span>|<span data-ttu-id="ea708-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea708-139">String</span></span>|<span data-ttu-id="ea708-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ea708-140">Key of the entity.</span></span> <span data-ttu-id="ea708-141">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ea708-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ea708-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea708-142">lastModifiedDateTime</span></span>|<span data-ttu-id="ea708-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea708-143">DateTimeOffset</span></span>|<span data-ttu-id="ea708-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ea708-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="ea708-145">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ea708-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ea708-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea708-146">Response</span></span>
<span data-ttu-id="ea708-147">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ea708-147">If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea708-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ea708-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea708-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea708-149">Request</span></span>
<span data-ttu-id="ea708-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea708-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedPresentation",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="ea708-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea708-151">Response</span></span>
<span data-ttu-id="ea708-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ea708-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




