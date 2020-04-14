---
title: Criar groupPolicyUploadedPresentation
description: Criar um novo objeto groupPolicyUploadedPresentation.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0fd0a371d2eadee9769be4cf3b5a738ce97e9831
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440872"
---
# <a name="create-grouppolicyuploadedpresentation"></a><span data-ttu-id="33a01-103">Criar groupPolicyUploadedPresentation</span><span class="sxs-lookup"><span data-stu-id="33a01-103">Create groupPolicyUploadedPresentation</span></span>

<span data-ttu-id="33a01-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33a01-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="33a01-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="33a01-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33a01-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="33a01-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33a01-107">Criar um novo objeto [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="33a01-107">Create a new [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33a01-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="33a01-108">Prerequisites</span></span>
<span data-ttu-id="33a01-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33a01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33a01-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33a01-111">Permission type</span></span>|<span data-ttu-id="33a01-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="33a01-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33a01-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33a01-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33a01-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33a01-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="33a01-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33a01-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33a01-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33a01-116">Not supported.</span></span>|
|<span data-ttu-id="33a01-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33a01-117">Application</span></span>|<span data-ttu-id="33a01-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33a01-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="33a01-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33a01-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="33a01-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33a01-120">Request headers</span></span>
|<span data-ttu-id="33a01-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="33a01-121">Header</span></span>|<span data-ttu-id="33a01-122">Valor</span><span class="sxs-lookup"><span data-stu-id="33a01-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33a01-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="33a01-123">Authorization</span></span>|<span data-ttu-id="33a01-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33a01-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33a01-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="33a01-125">Accept</span></span>|<span data-ttu-id="33a01-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33a01-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33a01-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33a01-127">Request body</span></span>
<span data-ttu-id="33a01-128">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyUploadedPresentation.</span><span class="sxs-lookup"><span data-stu-id="33a01-128">In the request body, supply a JSON representation for the groupPolicyUploadedPresentation object.</span></span>

<span data-ttu-id="33a01-129">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyUploadedPresentation.</span><span class="sxs-lookup"><span data-stu-id="33a01-129">The following table shows the properties that are required when you create the groupPolicyUploadedPresentation.</span></span>

|<span data-ttu-id="33a01-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33a01-130">Property</span></span>|<span data-ttu-id="33a01-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="33a01-131">Type</span></span>|<span data-ttu-id="33a01-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="33a01-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33a01-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="33a01-133">label</span></span>|<span data-ttu-id="33a01-134">String</span><span class="sxs-lookup"><span data-stu-id="33a01-134">String</span></span>|<span data-ttu-id="33a01-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="33a01-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="33a01-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="33a01-136">The default value is empty.</span></span> <span data-ttu-id="33a01-137">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="33a01-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="33a01-138">id</span><span class="sxs-lookup"><span data-stu-id="33a01-138">id</span></span>|<span data-ttu-id="33a01-139">String</span><span class="sxs-lookup"><span data-stu-id="33a01-139">String</span></span>|<span data-ttu-id="33a01-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="33a01-140">Key of the entity.</span></span> <span data-ttu-id="33a01-141">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="33a01-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="33a01-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33a01-142">lastModifiedDateTime</span></span>|<span data-ttu-id="33a01-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33a01-143">DateTimeOffset</span></span>|<span data-ttu-id="33a01-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="33a01-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="33a01-145">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="33a01-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|



## <a name="response"></a><span data-ttu-id="33a01-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="33a01-146">Response</span></span>
<span data-ttu-id="33a01-147">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33a01-147">If successful, this method returns a `201 Created` response code and a [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33a01-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33a01-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="33a01-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33a01-149">Request</span></span>
<span data-ttu-id="33a01-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33a01-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedPresentation",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="33a01-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="33a01-151">Response</span></span>
<span data-ttu-id="33a01-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33a01-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 213

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedPresentation",
  "label": "Label value",
  "id": "b9f611e8-11e8-b9f6-e811-f6b9e811f6b9",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```



