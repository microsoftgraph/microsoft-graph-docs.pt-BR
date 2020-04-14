---
title: Criar groupPolicyPresentationCheckBox
description: Criar um novo objeto groupPolicyPresentationCheckBox.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7215f64140e20c9af12624b7a659037e7afb1aed
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43377952"
---
# <a name="create-grouppolicypresentationcheckbox"></a><span data-ttu-id="7ce6e-103">Criar groupPolicyPresentationCheckBox</span><span class="sxs-lookup"><span data-stu-id="7ce6e-103">Create groupPolicyPresentationCheckBox</span></span>

<span data-ttu-id="7ce6e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ce6e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ce6e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7ce6e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ce6e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7ce6e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ce6e-107">Criar um novo objeto [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .</span><span class="sxs-lookup"><span data-stu-id="7ce6e-107">Create a new [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ce6e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7ce6e-108">Prerequisites</span></span>
<span data-ttu-id="7ce6e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ce6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ce6e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ce6e-111">Permission type</span></span>|<span data-ttu-id="7ce6e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7ce6e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ce6e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ce6e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7ce6e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ce6e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7ce6e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ce6e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ce6e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ce6e-116">Not supported.</span></span>|
|<span data-ttu-id="7ce6e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ce6e-117">Application</span></span>|<span data-ttu-id="7ce6e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ce6e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ce6e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ce6e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="7ce6e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ce6e-120">Request headers</span></span>
|<span data-ttu-id="7ce6e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7ce6e-121">Header</span></span>|<span data-ttu-id="7ce6e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7ce6e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ce6e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ce6e-123">Authorization</span></span>|<span data-ttu-id="7ce6e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ce6e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ce6e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7ce6e-125">Accept</span></span>|<span data-ttu-id="7ce6e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7ce6e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ce6e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ce6e-127">Request body</span></span>
<span data-ttu-id="7ce6e-128">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyPresentationCheckBox.</span><span class="sxs-lookup"><span data-stu-id="7ce6e-128">In the request body, supply a JSON representation for the groupPolicyPresentationCheckBox object.</span></span>

<span data-ttu-id="7ce6e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyPresentationCheckBox.</span><span class="sxs-lookup"><span data-stu-id="7ce6e-129">The following table shows the properties that are required when you create the groupPolicyPresentationCheckBox.</span></span>

|<span data-ttu-id="7ce6e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ce6e-130">Property</span></span>|<span data-ttu-id="7ce6e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ce6e-131">Type</span></span>|<span data-ttu-id="7ce6e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ce6e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ce6e-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="7ce6e-133">label</span></span>|<span data-ttu-id="7ce6e-134">String</span><span class="sxs-lookup"><span data-stu-id="7ce6e-134">String</span></span>|<span data-ttu-id="7ce6e-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="7ce6e-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="7ce6e-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="7ce6e-136">The default value is empty.</span></span> <span data-ttu-id="7ce6e-137">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="7ce6e-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="7ce6e-138">id</span><span class="sxs-lookup"><span data-stu-id="7ce6e-138">id</span></span>|<span data-ttu-id="7ce6e-139">String</span><span class="sxs-lookup"><span data-stu-id="7ce6e-139">String</span></span>|<span data-ttu-id="7ce6e-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7ce6e-140">Key of the entity.</span></span> <span data-ttu-id="7ce6e-141">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="7ce6e-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="7ce6e-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ce6e-142">lastModifiedDateTime</span></span>|<span data-ttu-id="7ce6e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ce6e-143">DateTimeOffset</span></span>|<span data-ttu-id="7ce6e-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="7ce6e-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="7ce6e-145">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="7ce6e-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="7ce6e-146">defaultChecked</span><span class="sxs-lookup"><span data-stu-id="7ce6e-146">defaultChecked</span></span>|<span data-ttu-id="7ce6e-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ce6e-147">Boolean</span></span>|<span data-ttu-id="7ce6e-148">Valor padrão da caixa de seleção.</span><span class="sxs-lookup"><span data-stu-id="7ce6e-148">Default value for the check box.</span></span> <span data-ttu-id="7ce6e-149">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="7ce6e-149">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="7ce6e-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ce6e-150">Response</span></span>
<span data-ttu-id="7ce6e-151">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ce6e-151">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ce6e-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ce6e-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ce6e-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ce6e-153">Request</span></span>
<span data-ttu-id="7ce6e-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ce6e-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "Label value",
  "defaultChecked": true
}
```

### <a name="response"></a><span data-ttu-id="7ce6e-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ce6e-155">Response</span></span>
<span data-ttu-id="7ce6e-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ce6e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 240

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "Label value",
  "id": "7748190f-190f-7748-0f19-48770f194877",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultChecked": true
}
```



