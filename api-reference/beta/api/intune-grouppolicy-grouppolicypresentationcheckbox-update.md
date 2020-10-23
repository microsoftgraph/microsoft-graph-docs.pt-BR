---
title: Atualizar groupPolicyPresentationCheckBox
description: Atualiza as propriedades de um objeto groupPolicyPresentationCheckBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 63f3efd5dbb48875c1d80774a393734369f268fe
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724119"
---
# <a name="update-grouppolicypresentationcheckbox"></a><span data-ttu-id="d1e4d-103">Atualizar groupPolicyPresentationCheckBox</span><span class="sxs-lookup"><span data-stu-id="d1e4d-103">Update groupPolicyPresentationCheckBox</span></span>

<span data-ttu-id="d1e4d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1e4d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1e4d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d1e4d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1e4d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d1e4d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1e4d-107">Atualiza as propriedades de um objeto [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .</span><span class="sxs-lookup"><span data-stu-id="d1e4d-107">Update the properties of a [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1e4d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d1e4d-108">Prerequisites</span></span>
<span data-ttu-id="d1e4d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1e4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1e4d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1e4d-111">Permission type</span></span>|<span data-ttu-id="d1e4d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d1e4d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1e4d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1e4d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d1e4d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1e4d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d1e4d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1e4d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1e4d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1e4d-116">Not supported.</span></span>|
|<span data-ttu-id="d1e4d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1e4d-117">Application</span></span>|<span data-ttu-id="d1e4d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1e4d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1e4d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1e4d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="d1e4d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1e4d-120">Request headers</span></span>
|<span data-ttu-id="d1e4d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d1e4d-121">Header</span></span>|<span data-ttu-id="d1e4d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d1e4d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1e4d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1e4d-123">Authorization</span></span>|<span data-ttu-id="d1e4d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1e4d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1e4d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d1e4d-125">Accept</span></span>|<span data-ttu-id="d1e4d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d1e4d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1e4d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1e4d-127">Request body</span></span>
<span data-ttu-id="d1e4d-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .</span><span class="sxs-lookup"><span data-stu-id="d1e4d-128">In the request body, supply a JSON representation for the [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

<span data-ttu-id="d1e4d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md).</span><span class="sxs-lookup"><span data-stu-id="d1e4d-129">The following table shows the properties that are required when you create the [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md).</span></span>

|<span data-ttu-id="d1e4d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d1e4d-130">Property</span></span>|<span data-ttu-id="d1e4d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1e4d-131">Type</span></span>|<span data-ttu-id="d1e4d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1e4d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1e4d-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="d1e4d-133">label</span></span>|<span data-ttu-id="d1e4d-134">String</span><span class="sxs-lookup"><span data-stu-id="d1e4d-134">String</span></span>|<span data-ttu-id="d1e4d-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="d1e4d-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="d1e4d-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="d1e4d-136">The default value is empty.</span></span> <span data-ttu-id="d1e4d-137">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="d1e4d-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="d1e4d-138">id</span><span class="sxs-lookup"><span data-stu-id="d1e4d-138">id</span></span>|<span data-ttu-id="d1e4d-139">String</span><span class="sxs-lookup"><span data-stu-id="d1e4d-139">String</span></span>|<span data-ttu-id="d1e4d-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d1e4d-140">Key of the entity.</span></span> <span data-ttu-id="d1e4d-141">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="d1e4d-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="d1e4d-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d1e4d-142">lastModifiedDateTime</span></span>|<span data-ttu-id="d1e4d-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1e4d-143">DateTimeOffset</span></span>|<span data-ttu-id="d1e4d-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d1e4d-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="d1e4d-145">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="d1e4d-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="d1e4d-146">defaultChecked</span><span class="sxs-lookup"><span data-stu-id="d1e4d-146">defaultChecked</span></span>|<span data-ttu-id="d1e4d-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="d1e4d-147">Boolean</span></span>|<span data-ttu-id="d1e4d-148">Valor padrão da caixa de seleção.</span><span class="sxs-lookup"><span data-stu-id="d1e4d-148">Default value for the check box.</span></span> <span data-ttu-id="d1e4d-149">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="d1e4d-149">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="d1e4d-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1e4d-150">Response</span></span>
<span data-ttu-id="d1e4d-151">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1e4d-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1e4d-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1e4d-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1e4d-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1e4d-153">Request</span></span>
<span data-ttu-id="d1e4d-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1e4d-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "Label value",
  "defaultChecked": true
}
```

### <a name="response"></a><span data-ttu-id="d1e4d-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1e4d-155">Response</span></span>
<span data-ttu-id="d1e4d-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1e4d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





