---
title: Atualizar groupPolicyPresentationMultiTextBox
description: Atualiza as propriedades de um objeto groupPolicyPresentationMultiTextBox.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ce98df8c43404516d403eb767d195213ecbe5348
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972358"
---
# <a name="update-grouppolicypresentationmultitextbox"></a><span data-ttu-id="91e84-103">Atualizar groupPolicyPresentationMultiTextBox</span><span class="sxs-lookup"><span data-stu-id="91e84-103">Update groupPolicyPresentationMultiTextBox</span></span>

> <span data-ttu-id="91e84-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="91e84-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91e84-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="91e84-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91e84-106">Atualiza as propriedades de um objeto [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="91e84-106">Update the properties of a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91e84-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="91e84-107">Prerequisites</span></span>
<span data-ttu-id="91e84-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91e84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91e84-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91e84-110">Permission type</span></span>|<span data-ttu-id="91e84-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="91e84-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91e84-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91e84-112">Delegated (work or school account)</span></span>|<span data-ttu-id="91e84-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91e84-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="91e84-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91e84-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91e84-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91e84-115">Not supported.</span></span>|
|<span data-ttu-id="91e84-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91e84-116">Application</span></span>|<span data-ttu-id="91e84-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91e84-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91e84-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91e84-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="91e84-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91e84-119">Request headers</span></span>
|<span data-ttu-id="91e84-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="91e84-120">Header</span></span>|<span data-ttu-id="91e84-121">Valor</span><span class="sxs-lookup"><span data-stu-id="91e84-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91e84-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="91e84-122">Authorization</span></span>|<span data-ttu-id="91e84-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91e84-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91e84-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="91e84-124">Accept</span></span>|<span data-ttu-id="91e84-125">application/json</span><span class="sxs-lookup"><span data-stu-id="91e84-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91e84-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91e84-126">Request body</span></span>
<span data-ttu-id="91e84-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="91e84-127">In the request body, supply a JSON representation for the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

<span data-ttu-id="91e84-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md).</span><span class="sxs-lookup"><span data-stu-id="91e84-128">The following table shows the properties that are required when you create the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md).</span></span>

|<span data-ttu-id="91e84-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91e84-129">Property</span></span>|<span data-ttu-id="91e84-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="91e84-130">Type</span></span>|<span data-ttu-id="91e84-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="91e84-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91e84-132">rótulo</span><span class="sxs-lookup"><span data-stu-id="91e84-132">label</span></span>|<span data-ttu-id="91e84-133">String</span><span class="sxs-lookup"><span data-stu-id="91e84-133">String</span></span>|<span data-ttu-id="91e84-134">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="91e84-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="91e84-135">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="91e84-135">The default value is empty.</span></span> <span data-ttu-id="91e84-136">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="91e84-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="91e84-137">id</span><span class="sxs-lookup"><span data-stu-id="91e84-137">id</span></span>|<span data-ttu-id="91e84-138">String</span><span class="sxs-lookup"><span data-stu-id="91e84-138">String</span></span>|<span data-ttu-id="91e84-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="91e84-139">Key of the entity.</span></span> <span data-ttu-id="91e84-140">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="91e84-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="91e84-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="91e84-141">lastModifiedDateTime</span></span>|<span data-ttu-id="91e84-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91e84-142">DateTimeOffset</span></span>|<span data-ttu-id="91e84-143">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="91e84-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="91e84-144">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="91e84-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="91e84-145">obrigatório</span><span class="sxs-lookup"><span data-stu-id="91e84-145">required</span></span>|<span data-ttu-id="91e84-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="91e84-146">Boolean</span></span>|<span data-ttu-id="91e84-147">Requisito para inserir um valor na caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="91e84-147">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="91e84-148">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="91e84-148">Default value is false.</span></span>|
|<span data-ttu-id="91e84-149">maxLength</span><span class="sxs-lookup"><span data-stu-id="91e84-149">maxLength</span></span>|<span data-ttu-id="91e84-150">Int64</span><span class="sxs-lookup"><span data-stu-id="91e84-150">Int64</span></span>|<span data-ttu-id="91e84-151">Um inteiro sem sinal que especifica o número máximo de caracteres de texto.</span><span class="sxs-lookup"><span data-stu-id="91e84-151">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="91e84-152">O valor padrão é 1023.</span><span class="sxs-lookup"><span data-stu-id="91e84-152">Default value is 1023.</span></span>|
|<span data-ttu-id="91e84-153">maxStrings</span><span class="sxs-lookup"><span data-stu-id="91e84-153">maxStrings</span></span>|<span data-ttu-id="91e84-154">Int64</span><span class="sxs-lookup"><span data-stu-id="91e84-154">Int64</span></span>|<span data-ttu-id="91e84-155">Um inteiro sem sinal que especifica o número máximo de cadeias de caracteres.</span><span class="sxs-lookup"><span data-stu-id="91e84-155">An unsigned integer that specifies the maximum number of strings.</span></span> <span data-ttu-id="91e84-156">O valor padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="91e84-156">Default value is 0.</span></span>|



## <a name="response"></a><span data-ttu-id="91e84-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="91e84-157">Response</span></span>
<span data-ttu-id="91e84-158">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91e84-158">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91e84-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91e84-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="91e84-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91e84-160">Request</span></span>
<span data-ttu-id="91e84-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91e84-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="91e84-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="91e84-162">Response</span></span>
<span data-ttu-id="91e84-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91e84-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




