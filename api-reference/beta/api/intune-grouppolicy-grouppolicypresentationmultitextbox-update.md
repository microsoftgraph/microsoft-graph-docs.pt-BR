---
title: Atualizar groupPolicyPresentationMultiTextBox
description: Atualize as propriedades de um objeto groupPolicyPresentationMultiTextBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 719dd7dd2c47b3e47cc3295e9f4ac8d801931cc0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149503"
---
# <a name="update-grouppolicypresentationmultitextbox"></a><span data-ttu-id="e1fc1-103">Atualizar groupPolicyPresentationMultiTextBox</span><span class="sxs-lookup"><span data-stu-id="e1fc1-103">Update groupPolicyPresentationMultiTextBox</span></span>

<span data-ttu-id="e1fc1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1fc1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1fc1-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e1fc1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1fc1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1fc1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1fc1-107">Atualize as propriedades de [um objeto groupPolicyPresentationMultiTextBox.](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)</span><span class="sxs-lookup"><span data-stu-id="e1fc1-107">Update the properties of a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1fc1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1fc1-108">Prerequisites</span></span>
<span data-ttu-id="e1fc1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1fc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1fc1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1fc1-111">Permission type</span></span>|<span data-ttu-id="e1fc1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1fc1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1fc1-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1fc1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1fc1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1fc1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e1fc1-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1fc1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1fc1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1fc1-116">Not supported.</span></span>|
|<span data-ttu-id="e1fc1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1fc1-117">Application</span></span>|<span data-ttu-id="e1fc1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1fc1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1fc1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1fc1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="e1fc1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1fc1-120">Request headers</span></span>
|<span data-ttu-id="e1fc1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1fc1-121">Header</span></span>|<span data-ttu-id="e1fc1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e1fc1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1fc1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1fc1-123">Authorization</span></span>|<span data-ttu-id="e1fc1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1fc1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1fc1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1fc1-125">Accept</span></span>|<span data-ttu-id="e1fc1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1fc1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1fc1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1fc1-127">Request body</span></span>
<span data-ttu-id="e1fc1-128">No corpo da solicitação, fornece uma representação JSON para o [objeto groupPolicyPresentationMultiTextBox.](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)</span><span class="sxs-lookup"><span data-stu-id="e1fc1-128">In the request body, supply a JSON representation for the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

<span data-ttu-id="e1fc1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md).</span><span class="sxs-lookup"><span data-stu-id="e1fc1-129">The following table shows the properties that are required when you create the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md).</span></span>

|<span data-ttu-id="e1fc1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1fc1-130">Property</span></span>|<span data-ttu-id="e1fc1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1fc1-131">Type</span></span>|<span data-ttu-id="e1fc1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1fc1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1fc1-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="e1fc1-133">label</span></span>|<span data-ttu-id="e1fc1-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1fc1-134">String</span></span>|<span data-ttu-id="e1fc1-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="e1fc1-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="e1fc1-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="e1fc1-136">The default value is empty.</span></span> <span data-ttu-id="e1fc1-137">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="e1fc1-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="e1fc1-138">id</span><span class="sxs-lookup"><span data-stu-id="e1fc1-138">id</span></span>|<span data-ttu-id="e1fc1-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1fc1-139">String</span></span>|<span data-ttu-id="e1fc1-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e1fc1-140">Key of the entity.</span></span> <span data-ttu-id="e1fc1-141">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="e1fc1-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="e1fc1-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1fc1-142">lastModifiedDateTime</span></span>|<span data-ttu-id="e1fc1-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1fc1-143">DateTimeOffset</span></span>|<span data-ttu-id="e1fc1-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e1fc1-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="e1fc1-145">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="e1fc1-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="e1fc1-146">obrigatório</span><span class="sxs-lookup"><span data-stu-id="e1fc1-146">required</span></span>|<span data-ttu-id="e1fc1-147">Booleano</span><span class="sxs-lookup"><span data-stu-id="e1fc1-147">Boolean</span></span>|<span data-ttu-id="e1fc1-148">Requisito para inserir um valor na caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="e1fc1-148">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="e1fc1-149">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="e1fc1-149">Default value is false.</span></span>|
|<span data-ttu-id="e1fc1-150">maxLength</span><span class="sxs-lookup"><span data-stu-id="e1fc1-150">maxLength</span></span>|<span data-ttu-id="e1fc1-151">Int64</span><span class="sxs-lookup"><span data-stu-id="e1fc1-151">Int64</span></span>|<span data-ttu-id="e1fc1-152">Um inteiro não assinado que especifica o número máximo de caracteres de texto.</span><span class="sxs-lookup"><span data-stu-id="e1fc1-152">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="e1fc1-153">O valor padrão é 1023.</span><span class="sxs-lookup"><span data-stu-id="e1fc1-153">Default value is 1023.</span></span>|
|<span data-ttu-id="e1fc1-154">maxStrings</span><span class="sxs-lookup"><span data-stu-id="e1fc1-154">maxStrings</span></span>|<span data-ttu-id="e1fc1-155">Int64</span><span class="sxs-lookup"><span data-stu-id="e1fc1-155">Int64</span></span>|<span data-ttu-id="e1fc1-156">Um inteiro não assinado que especifica o número máximo de cadeias de caracteres.</span><span class="sxs-lookup"><span data-stu-id="e1fc1-156">An unsigned integer that specifies the maximum number of strings.</span></span> <span data-ttu-id="e1fc1-157">O valor padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="e1fc1-157">Default value is 0.</span></span>|



## <a name="response"></a><span data-ttu-id="e1fc1-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1fc1-158">Response</span></span>
<span data-ttu-id="e1fc1-159">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1fc1-159">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1fc1-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1fc1-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1fc1-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1fc1-161">Request</span></span>
<span data-ttu-id="e1fc1-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1fc1-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 165

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "label": "Label value",
  "required": true,
  "maxLength": 9,
  "maxStrings": 10
}
```

### <a name="response"></a><span data-ttu-id="e1fc1-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1fc1-163">Response</span></span>
<span data-ttu-id="e1fc1-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1fc1-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 278

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "label": "Label value",
  "id": "381ac035-c035-381a-35c0-1a3835c01a38",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "required": true,
  "maxLength": 9,
  "maxStrings": 10
}
```




