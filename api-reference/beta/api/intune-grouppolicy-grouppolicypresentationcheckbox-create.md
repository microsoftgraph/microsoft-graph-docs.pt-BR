---
title: Criar groupPolicyPresentationCheckBox
description: Crie um novo objeto groupPolicyPresentationCheckBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 01aa0db90883a469685edacd839188dcea5235b7
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141999"
---
# <a name="create-grouppolicypresentationcheckbox"></a><span data-ttu-id="73632-103">Criar groupPolicyPresentationCheckBox</span><span class="sxs-lookup"><span data-stu-id="73632-103">Create groupPolicyPresentationCheckBox</span></span>

<span data-ttu-id="73632-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73632-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73632-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="73632-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73632-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="73632-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73632-107">Crie um novo [objeto groupPolicyPresentationCheckBox.](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)</span><span class="sxs-lookup"><span data-stu-id="73632-107">Create a new [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73632-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="73632-108">Prerequisites</span></span>
<span data-ttu-id="73632-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73632-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73632-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73632-111">Permission type</span></span>|<span data-ttu-id="73632-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="73632-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73632-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73632-113">Delegated (work or school account)</span></span>|<span data-ttu-id="73632-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73632-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="73632-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73632-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73632-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73632-116">Not supported.</span></span>|
|<span data-ttu-id="73632-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73632-117">Application</span></span>|<span data-ttu-id="73632-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73632-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="73632-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73632-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="73632-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73632-120">Request headers</span></span>
|<span data-ttu-id="73632-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="73632-121">Header</span></span>|<span data-ttu-id="73632-122">Valor</span><span class="sxs-lookup"><span data-stu-id="73632-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73632-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="73632-123">Authorization</span></span>|<span data-ttu-id="73632-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73632-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73632-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="73632-125">Accept</span></span>|<span data-ttu-id="73632-126">application/json</span><span class="sxs-lookup"><span data-stu-id="73632-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73632-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73632-127">Request body</span></span>
<span data-ttu-id="73632-128">No corpo da solicitação, fornece uma representação JSON para o objeto groupPolicyPresentationCheckBox.</span><span class="sxs-lookup"><span data-stu-id="73632-128">In the request body, supply a JSON representation for the groupPolicyPresentationCheckBox object.</span></span>

<span data-ttu-id="73632-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o groupPolicyPresentationCheckBox.</span><span class="sxs-lookup"><span data-stu-id="73632-129">The following table shows the properties that are required when you create the groupPolicyPresentationCheckBox.</span></span>

|<span data-ttu-id="73632-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73632-130">Property</span></span>|<span data-ttu-id="73632-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="73632-131">Type</span></span>|<span data-ttu-id="73632-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="73632-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73632-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="73632-133">label</span></span>|<span data-ttu-id="73632-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73632-134">String</span></span>|<span data-ttu-id="73632-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="73632-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="73632-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="73632-136">The default value is empty.</span></span> <span data-ttu-id="73632-137">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="73632-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="73632-138">id</span><span class="sxs-lookup"><span data-stu-id="73632-138">id</span></span>|<span data-ttu-id="73632-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73632-139">String</span></span>|<span data-ttu-id="73632-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="73632-140">Key of the entity.</span></span> <span data-ttu-id="73632-141">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="73632-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="73632-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73632-142">lastModifiedDateTime</span></span>|<span data-ttu-id="73632-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73632-143">DateTimeOffset</span></span>|<span data-ttu-id="73632-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="73632-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="73632-145">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="73632-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="73632-146">defaultChecked</span><span class="sxs-lookup"><span data-stu-id="73632-146">defaultChecked</span></span>|<span data-ttu-id="73632-147">Booleano</span><span class="sxs-lookup"><span data-stu-id="73632-147">Boolean</span></span>|<span data-ttu-id="73632-148">Valor padrão da caixa de seleção.</span><span class="sxs-lookup"><span data-stu-id="73632-148">Default value for the check box.</span></span> <span data-ttu-id="73632-149">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="73632-149">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="73632-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="73632-150">Response</span></span>
<span data-ttu-id="73632-151">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73632-151">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73632-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73632-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="73632-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73632-153">Request</span></span>
<span data-ttu-id="73632-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="73632-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="73632-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="73632-155">Response</span></span>
<span data-ttu-id="73632-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73632-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




