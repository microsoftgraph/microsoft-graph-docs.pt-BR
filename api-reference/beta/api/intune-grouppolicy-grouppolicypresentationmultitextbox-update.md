---
title: Atualizar groupPolicyPresentationMultiTextBox
description: Atualiza as propriedades de um objeto groupPolicyPresentationMultiTextBox.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 58ebe962fca809662b9ce2380ace610d0184584f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35984886"
---
# <a name="update-grouppolicypresentationmultitextbox"></a><span data-ttu-id="e7fed-103">Atualizar groupPolicyPresentationMultiTextBox</span><span class="sxs-lookup"><span data-stu-id="e7fed-103">Update groupPolicyPresentationMultiTextBox</span></span>

> <span data-ttu-id="e7fed-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e7fed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7fed-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e7fed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7fed-106">Atualiza as propriedades de um objeto [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="e7fed-106">Update the properties of a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7fed-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e7fed-107">Prerequisites</span></span>
<span data-ttu-id="e7fed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7fed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7fed-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7fed-110">Permission type</span></span>|<span data-ttu-id="e7fed-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e7fed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7fed-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7fed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e7fed-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7fed-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e7fed-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7fed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7fed-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7fed-115">Not supported.</span></span>|
|<span data-ttu-id="e7fed-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7fed-116">Application</span></span>|<span data-ttu-id="e7fed-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7fed-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7fed-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7fed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="e7fed-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7fed-119">Request headers</span></span>
|<span data-ttu-id="e7fed-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7fed-120">Header</span></span>|<span data-ttu-id="e7fed-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e7fed-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7fed-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7fed-122">Authorization</span></span>|<span data-ttu-id="e7fed-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7fed-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7fed-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e7fed-124">Accept</span></span>|<span data-ttu-id="e7fed-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e7fed-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7fed-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7fed-126">Request body</span></span>
<span data-ttu-id="e7fed-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="e7fed-127">In the request body, supply a JSON representation for the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

<span data-ttu-id="e7fed-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md).</span><span class="sxs-lookup"><span data-stu-id="e7fed-128">The following table shows the properties that are required when you create the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md).</span></span>

|<span data-ttu-id="e7fed-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e7fed-129">Property</span></span>|<span data-ttu-id="e7fed-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7fed-130">Type</span></span>|<span data-ttu-id="e7fed-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7fed-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7fed-132">rótulo</span><span class="sxs-lookup"><span data-stu-id="e7fed-132">label</span></span>|<span data-ttu-id="e7fed-133">String</span><span class="sxs-lookup"><span data-stu-id="e7fed-133">String</span></span>|<span data-ttu-id="e7fed-134">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="e7fed-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="e7fed-135">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="e7fed-135">The default value is empty.</span></span> <span data-ttu-id="e7fed-136">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="e7fed-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="e7fed-137">id</span><span class="sxs-lookup"><span data-stu-id="e7fed-137">id</span></span>|<span data-ttu-id="e7fed-138">String</span><span class="sxs-lookup"><span data-stu-id="e7fed-138">String</span></span>|<span data-ttu-id="e7fed-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e7fed-139">Key of the entity.</span></span> <span data-ttu-id="e7fed-140">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="e7fed-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="e7fed-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7fed-141">lastModifiedDateTime</span></span>|<span data-ttu-id="e7fed-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7fed-142">DateTimeOffset</span></span>|<span data-ttu-id="e7fed-143">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e7fed-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="e7fed-144">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="e7fed-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="e7fed-145">obrigatório</span><span class="sxs-lookup"><span data-stu-id="e7fed-145">required</span></span>|<span data-ttu-id="e7fed-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="e7fed-146">Boolean</span></span>|<span data-ttu-id="e7fed-147">Requisito para inserir um valor na caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="e7fed-147">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="e7fed-148">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="e7fed-148">Default value is false.</span></span>|
|<span data-ttu-id="e7fed-149">maxLength</span><span class="sxs-lookup"><span data-stu-id="e7fed-149">maxLength</span></span>|<span data-ttu-id="e7fed-150">Int64</span><span class="sxs-lookup"><span data-stu-id="e7fed-150">Int64</span></span>|<span data-ttu-id="e7fed-151">Um inteiro sem sinal que especifica o número máximo de caracteres de texto.</span><span class="sxs-lookup"><span data-stu-id="e7fed-151">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="e7fed-152">O valor padrão é 1023.</span><span class="sxs-lookup"><span data-stu-id="e7fed-152">Default value is 1023.</span></span>|
|<span data-ttu-id="e7fed-153">maxStrings</span><span class="sxs-lookup"><span data-stu-id="e7fed-153">maxStrings</span></span>|<span data-ttu-id="e7fed-154">Int64</span><span class="sxs-lookup"><span data-stu-id="e7fed-154">Int64</span></span>|<span data-ttu-id="e7fed-155">Um inteiro sem sinal que especifica o número máximo de cadeias de caracteres.</span><span class="sxs-lookup"><span data-stu-id="e7fed-155">An unsigned integer that specifies the maximum number of strings.</span></span> <span data-ttu-id="e7fed-156">O valor padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="e7fed-156">Default value is 0.</span></span>|



## <a name="response"></a><span data-ttu-id="e7fed-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7fed-157">Response</span></span>
<span data-ttu-id="e7fed-158">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7fed-158">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7fed-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7fed-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7fed-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7fed-160">Request</span></span>
<span data-ttu-id="e7fed-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7fed-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e7fed-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7fed-162">Response</span></span>
<span data-ttu-id="e7fed-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7fed-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





