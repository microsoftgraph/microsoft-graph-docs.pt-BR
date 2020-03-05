---
title: Criar groupPolicyPresentationMultiTextBox
description: Criar um novo objeto groupPolicyPresentationMultiTextBox.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4d7ba2d5f5466f6b59a06af7fe92ed4939bacdea
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42464565"
---
# <a name="create-grouppolicypresentationmultitextbox"></a><span data-ttu-id="92e49-103">Criar groupPolicyPresentationMultiTextBox</span><span class="sxs-lookup"><span data-stu-id="92e49-103">Create groupPolicyPresentationMultiTextBox</span></span>

<span data-ttu-id="92e49-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="92e49-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92e49-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="92e49-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92e49-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92e49-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92e49-107">Criar um novo objeto [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="92e49-107">Create a new [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92e49-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92e49-108">Prerequisites</span></span>
<span data-ttu-id="92e49-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92e49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92e49-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92e49-111">Permission type</span></span>|<span data-ttu-id="92e49-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="92e49-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92e49-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92e49-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92e49-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92e49-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="92e49-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92e49-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92e49-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92e49-116">Not supported.</span></span>|
|<span data-ttu-id="92e49-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92e49-117">Application</span></span>|<span data-ttu-id="92e49-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92e49-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92e49-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92e49-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="92e49-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92e49-120">Request headers</span></span>
|<span data-ttu-id="92e49-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92e49-121">Header</span></span>|<span data-ttu-id="92e49-122">Valor</span><span class="sxs-lookup"><span data-stu-id="92e49-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92e49-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="92e49-123">Authorization</span></span>|<span data-ttu-id="92e49-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92e49-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92e49-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92e49-125">Accept</span></span>|<span data-ttu-id="92e49-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92e49-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92e49-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92e49-127">Request body</span></span>
<span data-ttu-id="92e49-128">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyPresentationMultiTextBox.</span><span class="sxs-lookup"><span data-stu-id="92e49-128">In the request body, supply a JSON representation for the groupPolicyPresentationMultiTextBox object.</span></span>

<span data-ttu-id="92e49-129">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyPresentationMultiTextBox.</span><span class="sxs-lookup"><span data-stu-id="92e49-129">The following table shows the properties that are required when you create the groupPolicyPresentationMultiTextBox.</span></span>

|<span data-ttu-id="92e49-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92e49-130">Property</span></span>|<span data-ttu-id="92e49-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="92e49-131">Type</span></span>|<span data-ttu-id="92e49-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="92e49-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92e49-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="92e49-133">label</span></span>|<span data-ttu-id="92e49-134">String</span><span class="sxs-lookup"><span data-stu-id="92e49-134">String</span></span>|<span data-ttu-id="92e49-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="92e49-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="92e49-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="92e49-136">The default value is empty.</span></span> <span data-ttu-id="92e49-137">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="92e49-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="92e49-138">id</span><span class="sxs-lookup"><span data-stu-id="92e49-138">id</span></span>|<span data-ttu-id="92e49-139">String</span><span class="sxs-lookup"><span data-stu-id="92e49-139">String</span></span>|<span data-ttu-id="92e49-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="92e49-140">Key of the entity.</span></span> <span data-ttu-id="92e49-141">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="92e49-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="92e49-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="92e49-142">lastModifiedDateTime</span></span>|<span data-ttu-id="92e49-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92e49-143">DateTimeOffset</span></span>|<span data-ttu-id="92e49-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="92e49-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="92e49-145">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="92e49-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="92e49-146">obrigatório</span><span class="sxs-lookup"><span data-stu-id="92e49-146">required</span></span>|<span data-ttu-id="92e49-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="92e49-147">Boolean</span></span>|<span data-ttu-id="92e49-148">Requisito para inserir um valor na caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="92e49-148">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="92e49-149">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="92e49-149">Default value is false.</span></span>|
|<span data-ttu-id="92e49-150">maxLength</span><span class="sxs-lookup"><span data-stu-id="92e49-150">maxLength</span></span>|<span data-ttu-id="92e49-151">Int64</span><span class="sxs-lookup"><span data-stu-id="92e49-151">Int64</span></span>|<span data-ttu-id="92e49-152">Um inteiro sem sinal que especifica o número máximo de caracteres de texto.</span><span class="sxs-lookup"><span data-stu-id="92e49-152">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="92e49-153">O valor padrão é 1023.</span><span class="sxs-lookup"><span data-stu-id="92e49-153">Default value is 1023.</span></span>|
|<span data-ttu-id="92e49-154">maxStrings</span><span class="sxs-lookup"><span data-stu-id="92e49-154">maxStrings</span></span>|<span data-ttu-id="92e49-155">Int64</span><span class="sxs-lookup"><span data-stu-id="92e49-155">Int64</span></span>|<span data-ttu-id="92e49-156">Um inteiro sem sinal que especifica o número máximo de cadeias de caracteres.</span><span class="sxs-lookup"><span data-stu-id="92e49-156">An unsigned integer that specifies the maximum number of strings.</span></span> <span data-ttu-id="92e49-157">O valor padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="92e49-157">Default value is 0.</span></span>|



## <a name="response"></a><span data-ttu-id="92e49-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="92e49-158">Response</span></span>
<span data-ttu-id="92e49-159">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92e49-159">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92e49-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92e49-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="92e49-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92e49-161">Request</span></span>
<span data-ttu-id="92e49-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92e49-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
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

### <a name="response"></a><span data-ttu-id="92e49-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="92e49-163">Response</span></span>
<span data-ttu-id="92e49-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92e49-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





