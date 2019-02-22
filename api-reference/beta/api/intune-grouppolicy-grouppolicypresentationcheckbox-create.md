---
title: Criar groupPolicyPresentationCheckBox
description: Criar um novo objeto groupPolicyPresentationCheckBox.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6704ca00d90bab5679e0ab3bc5840272a6d0bc6e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159644"
---
# <a name="create-grouppolicypresentationcheckbox"></a><span data-ttu-id="db228-103">Criar groupPolicyPresentationCheckBox</span><span class="sxs-lookup"><span data-stu-id="db228-103">Create groupPolicyPresentationCheckBox</span></span>

> <span data-ttu-id="db228-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="db228-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db228-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="db228-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db228-106">Criar um novo objeto [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .</span><span class="sxs-lookup"><span data-stu-id="db228-106">Create a new [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db228-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="db228-107">Prerequisites</span></span>
<span data-ttu-id="db228-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="db228-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="db228-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db228-110">Permission type</span></span>|<span data-ttu-id="db228-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="db228-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db228-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db228-112">Delegated (work or school account)</span></span>|<span data-ttu-id="db228-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db228-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="db228-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db228-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db228-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db228-115">Not supported.</span></span>|
|<span data-ttu-id="db228-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db228-116">Application</span></span>|<span data-ttu-id="db228-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db228-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db228-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db228-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="db228-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db228-119">Request headers</span></span>
|<span data-ttu-id="db228-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="db228-120">Header</span></span>|<span data-ttu-id="db228-121">Valor</span><span class="sxs-lookup"><span data-stu-id="db228-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db228-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="db228-122">Authorization</span></span>|<span data-ttu-id="db228-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db228-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db228-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="db228-124">Accept</span></span>|<span data-ttu-id="db228-125">application/json</span><span class="sxs-lookup"><span data-stu-id="db228-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db228-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db228-126">Request body</span></span>
<span data-ttu-id="db228-127">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyPresentationCheckBox.</span><span class="sxs-lookup"><span data-stu-id="db228-127">In the request body, supply a JSON representation for the groupPolicyPresentationCheckBox object.</span></span>

<span data-ttu-id="db228-128">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyPresentationCheckBox.</span><span class="sxs-lookup"><span data-stu-id="db228-128">The following table shows the properties that are required when you create the groupPolicyPresentationCheckBox.</span></span>

|<span data-ttu-id="db228-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db228-129">Property</span></span>|<span data-ttu-id="db228-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="db228-130">Type</span></span>|<span data-ttu-id="db228-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="db228-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db228-132">rótulo</span><span class="sxs-lookup"><span data-stu-id="db228-132">label</span></span>|<span data-ttu-id="db228-133">String</span><span class="sxs-lookup"><span data-stu-id="db228-133">String</span></span>|<span data-ttu-id="db228-134">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="db228-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="db228-135">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="db228-135">The default value is empty.</span></span> <span data-ttu-id="db228-136">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="db228-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="db228-137">id</span><span class="sxs-lookup"><span data-stu-id="db228-137">id</span></span>|<span data-ttu-id="db228-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db228-138">String</span></span>|<span data-ttu-id="db228-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="db228-139">Key of the entity.</span></span> <span data-ttu-id="db228-140">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="db228-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="db228-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db228-141">lastModifiedDateTime</span></span>|<span data-ttu-id="db228-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db228-142">DateTimeOffset</span></span>|<span data-ttu-id="db228-143">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="db228-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="db228-144">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="db228-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="db228-145">defaultChecked</span><span class="sxs-lookup"><span data-stu-id="db228-145">defaultChecked</span></span>|<span data-ttu-id="db228-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="db228-146">Boolean</span></span>|<span data-ttu-id="db228-147">Valor padrão da caixa de seleção.</span><span class="sxs-lookup"><span data-stu-id="db228-147">Default value for the check box.</span></span> <span data-ttu-id="db228-148">O valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="db228-148">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="db228-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="db228-149">Response</span></span>
<span data-ttu-id="db228-150">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db228-150">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db228-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db228-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="db228-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db228-152">Request</span></span>
<span data-ttu-id="db228-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="db228-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="db228-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="db228-154">Response</span></span>
<span data-ttu-id="db228-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db228-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




