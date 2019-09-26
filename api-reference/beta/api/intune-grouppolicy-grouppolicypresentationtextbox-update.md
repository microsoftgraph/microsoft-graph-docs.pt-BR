---
title: Atualizar groupPolicyPresentationTextBox
description: Atualiza as propriedades de um objeto groupPolicyPresentationTextBox.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0cc3170e813ea48cce12a42b50e06bc680e45e44
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37193932"
---
# <a name="update-grouppolicypresentationtextbox"></a><span data-ttu-id="24473-103">Atualizar groupPolicyPresentationTextBox</span><span class="sxs-lookup"><span data-stu-id="24473-103">Update groupPolicyPresentationTextBox</span></span>

> <span data-ttu-id="24473-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="24473-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24473-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="24473-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24473-106">Atualiza as propriedades de um objeto [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="24473-106">Update the properties of a [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24473-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="24473-107">Prerequisites</span></span>
<span data-ttu-id="24473-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24473-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24473-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24473-110">Permission type</span></span>|<span data-ttu-id="24473-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="24473-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24473-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24473-112">Delegated (work or school account)</span></span>|<span data-ttu-id="24473-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24473-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="24473-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24473-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24473-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24473-115">Not supported.</span></span>|
|<span data-ttu-id="24473-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24473-116">Application</span></span>|<span data-ttu-id="24473-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24473-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24473-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24473-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="24473-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24473-119">Request headers</span></span>
|<span data-ttu-id="24473-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="24473-120">Header</span></span>|<span data-ttu-id="24473-121">Valor</span><span class="sxs-lookup"><span data-stu-id="24473-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24473-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="24473-122">Authorization</span></span>|<span data-ttu-id="24473-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24473-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24473-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="24473-124">Accept</span></span>|<span data-ttu-id="24473-125">application/json</span><span class="sxs-lookup"><span data-stu-id="24473-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24473-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24473-126">Request body</span></span>
<span data-ttu-id="24473-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="24473-127">In the request body, supply a JSON representation for the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

<span data-ttu-id="24473-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md).</span><span class="sxs-lookup"><span data-stu-id="24473-128">The following table shows the properties that are required when you create the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md).</span></span>

|<span data-ttu-id="24473-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="24473-129">Property</span></span>|<span data-ttu-id="24473-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="24473-130">Type</span></span>|<span data-ttu-id="24473-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="24473-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24473-132">rótulo</span><span class="sxs-lookup"><span data-stu-id="24473-132">label</span></span>|<span data-ttu-id="24473-133">String</span><span class="sxs-lookup"><span data-stu-id="24473-133">String</span></span>|<span data-ttu-id="24473-134">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="24473-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="24473-135">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="24473-135">The default value is empty.</span></span> <span data-ttu-id="24473-136">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="24473-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="24473-137">id</span><span class="sxs-lookup"><span data-stu-id="24473-137">id</span></span>|<span data-ttu-id="24473-138">String</span><span class="sxs-lookup"><span data-stu-id="24473-138">String</span></span>|<span data-ttu-id="24473-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="24473-139">Key of the entity.</span></span> <span data-ttu-id="24473-140">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="24473-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="24473-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="24473-141">lastModifiedDateTime</span></span>|<span data-ttu-id="24473-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24473-142">DateTimeOffset</span></span>|<span data-ttu-id="24473-143">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="24473-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="24473-144">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="24473-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="24473-145">defaultValue</span><span class="sxs-lookup"><span data-stu-id="24473-145">defaultValue</span></span>|<span data-ttu-id="24473-146">String</span><span class="sxs-lookup"><span data-stu-id="24473-146">String</span></span>|<span data-ttu-id="24473-147">Cadeia de caracteres padrão localizada exibida na caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="24473-147">Localized default string displayed in the text box.</span></span> <span data-ttu-id="24473-148">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="24473-148">The default value is empty.</span></span>|
|<span data-ttu-id="24473-149">obrigatório</span><span class="sxs-lookup"><span data-stu-id="24473-149">required</span></span>|<span data-ttu-id="24473-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="24473-150">Boolean</span></span>|<span data-ttu-id="24473-151">Requisito para inserir um valor na caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="24473-151">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="24473-152">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="24473-152">Default value is false.</span></span>|
|<span data-ttu-id="24473-153">maxLength</span><span class="sxs-lookup"><span data-stu-id="24473-153">maxLength</span></span>|<span data-ttu-id="24473-154">Int64</span><span class="sxs-lookup"><span data-stu-id="24473-154">Int64</span></span>|<span data-ttu-id="24473-155">Um inteiro sem sinal que especifica o número máximo de caracteres de texto.</span><span class="sxs-lookup"><span data-stu-id="24473-155">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="24473-156">O valor padrão é 1023.</span><span class="sxs-lookup"><span data-stu-id="24473-156">Default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="24473-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="24473-157">Response</span></span>
<span data-ttu-id="24473-158">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24473-158">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24473-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24473-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="24473-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24473-160">Request</span></span>
<span data-ttu-id="24473-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="24473-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "Label value",
  "defaultValue": "Default Value value",
  "required": true,
  "maxLength": 9
}
```

### <a name="response"></a><span data-ttu-id="24473-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="24473-162">Response</span></span>
<span data-ttu-id="24473-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24473-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 294

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "Label value",
  "id": "ec80633e-633e-ec80-3e63-80ec3e6380ec",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": "Default Value value",
  "required": true,
  "maxLength": 9
}
```




