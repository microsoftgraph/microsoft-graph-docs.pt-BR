---
title: Criar groupPolicyPresentationMultiTextBox
description: Criar um novo objeto groupPolicyPresentationMultiTextBox.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5615488ce6b4e5a7e4d477192b19aedf047f4c22
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783329"
---
# <a name="create-grouppolicypresentationmultitextbox"></a><span data-ttu-id="089ea-103">Criar groupPolicyPresentationMultiTextBox</span><span class="sxs-lookup"><span data-stu-id="089ea-103">Create groupPolicyPresentationMultiTextBox</span></span>

> <span data-ttu-id="089ea-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="089ea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="089ea-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="089ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="089ea-106">Criar um novo objeto [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="089ea-106">Create a new [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="089ea-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="089ea-107">Prerequisites</span></span>
<span data-ttu-id="089ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="089ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="089ea-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="089ea-110">Permission type</span></span>|<span data-ttu-id="089ea-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="089ea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="089ea-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="089ea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="089ea-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="089ea-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="089ea-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="089ea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="089ea-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="089ea-115">Not supported.</span></span>|
|<span data-ttu-id="089ea-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="089ea-116">Application</span></span>|<span data-ttu-id="089ea-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="089ea-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="089ea-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="089ea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="089ea-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="089ea-119">Request headers</span></span>
|<span data-ttu-id="089ea-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="089ea-120">Header</span></span>|<span data-ttu-id="089ea-121">Valor</span><span class="sxs-lookup"><span data-stu-id="089ea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="089ea-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="089ea-122">Authorization</span></span>|<span data-ttu-id="089ea-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="089ea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="089ea-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="089ea-124">Accept</span></span>|<span data-ttu-id="089ea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="089ea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="089ea-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="089ea-126">Request body</span></span>
<span data-ttu-id="089ea-127">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyPresentationMultiTextBox.</span><span class="sxs-lookup"><span data-stu-id="089ea-127">In the request body, supply a JSON representation for the groupPolicyPresentationMultiTextBox object.</span></span>

<span data-ttu-id="089ea-128">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyPresentationMultiTextBox.</span><span class="sxs-lookup"><span data-stu-id="089ea-128">The following table shows the properties that are required when you create the groupPolicyPresentationMultiTextBox.</span></span>

|<span data-ttu-id="089ea-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="089ea-129">Property</span></span>|<span data-ttu-id="089ea-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="089ea-130">Type</span></span>|<span data-ttu-id="089ea-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="089ea-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="089ea-132">rótulo</span><span class="sxs-lookup"><span data-stu-id="089ea-132">label</span></span>|<span data-ttu-id="089ea-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="089ea-133">String</span></span>|<span data-ttu-id="089ea-134">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="089ea-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="089ea-135">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="089ea-135">The default value is empty.</span></span> <span data-ttu-id="089ea-136">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="089ea-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="089ea-137">id</span><span class="sxs-lookup"><span data-stu-id="089ea-137">id</span></span>|<span data-ttu-id="089ea-138">String</span><span class="sxs-lookup"><span data-stu-id="089ea-138">String</span></span>|<span data-ttu-id="089ea-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="089ea-139">Key of the entity.</span></span> <span data-ttu-id="089ea-140">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="089ea-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="089ea-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="089ea-141">lastModifiedDateTime</span></span>|<span data-ttu-id="089ea-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="089ea-142">DateTimeOffset</span></span>|<span data-ttu-id="089ea-143">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="089ea-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="089ea-144">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="089ea-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="089ea-145">obrigatório</span><span class="sxs-lookup"><span data-stu-id="089ea-145">required</span></span>|<span data-ttu-id="089ea-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="089ea-146">Boolean</span></span>|<span data-ttu-id="089ea-147">Requisito para inserir um valor na caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="089ea-147">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="089ea-148">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="089ea-148">Default value is false.</span></span>|
|<span data-ttu-id="089ea-149">maxLength</span><span class="sxs-lookup"><span data-stu-id="089ea-149">maxLength</span></span>|<span data-ttu-id="089ea-150">Int64</span><span class="sxs-lookup"><span data-stu-id="089ea-150">Int64</span></span>|<span data-ttu-id="089ea-151">Um inteiro sem sinal que especifica o número máximo de caracteres de texto.</span><span class="sxs-lookup"><span data-stu-id="089ea-151">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="089ea-152">O valor padrão é 1023.</span><span class="sxs-lookup"><span data-stu-id="089ea-152">Default value is 1023.</span></span>|
|<span data-ttu-id="089ea-153">maxStrings</span><span class="sxs-lookup"><span data-stu-id="089ea-153">maxStrings</span></span>|<span data-ttu-id="089ea-154">Int64</span><span class="sxs-lookup"><span data-stu-id="089ea-154">Int64</span></span>|<span data-ttu-id="089ea-155">Um inteiro sem sinal que especifica o número máximo de cadeias de caracteres.</span><span class="sxs-lookup"><span data-stu-id="089ea-155">An unsigned integer that specifies the maximum number of strings.</span></span> <span data-ttu-id="089ea-156">O valor padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="089ea-156">Default value is 0.</span></span>|



## <a name="response"></a><span data-ttu-id="089ea-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="089ea-157">Response</span></span>
<span data-ttu-id="089ea-158">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="089ea-158">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="089ea-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="089ea-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="089ea-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="089ea-160">Request</span></span>
<span data-ttu-id="089ea-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="089ea-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="089ea-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="089ea-162">Response</span></span>
<span data-ttu-id="089ea-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="089ea-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





