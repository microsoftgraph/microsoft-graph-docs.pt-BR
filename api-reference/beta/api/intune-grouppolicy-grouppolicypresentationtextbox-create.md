---
title: Criar groupPolicyPresentationTextBox
description: Criar um novo objeto groupPolicyPresentationTextBox.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4639efd9a3c152e336ac3dd8f5297cba85cc6ab0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33904661"
---
# <a name="create-grouppolicypresentationtextbox"></a><span data-ttu-id="25f5a-103">Criar groupPolicyPresentationTextBox</span><span class="sxs-lookup"><span data-stu-id="25f5a-103">Create groupPolicyPresentationTextBox</span></span>

> <span data-ttu-id="25f5a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="25f5a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25f5a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="25f5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25f5a-106">Criar um novo objeto [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="25f5a-106">Create a new [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25f5a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="25f5a-107">Prerequisites</span></span>
<span data-ttu-id="25f5a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25f5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25f5a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25f5a-110">Permission type</span></span>|<span data-ttu-id="25f5a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="25f5a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25f5a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25f5a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="25f5a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25f5a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="25f5a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25f5a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25f5a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25f5a-115">Not supported.</span></span>|
|<span data-ttu-id="25f5a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25f5a-116">Application</span></span>|<span data-ttu-id="25f5a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25f5a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25f5a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25f5a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="25f5a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25f5a-119">Request headers</span></span>
|<span data-ttu-id="25f5a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="25f5a-120">Header</span></span>|<span data-ttu-id="25f5a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="25f5a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25f5a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="25f5a-122">Authorization</span></span>|<span data-ttu-id="25f5a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25f5a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25f5a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="25f5a-124">Accept</span></span>|<span data-ttu-id="25f5a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="25f5a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25f5a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25f5a-126">Request body</span></span>
<span data-ttu-id="25f5a-127">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyPresentationTextBox.</span><span class="sxs-lookup"><span data-stu-id="25f5a-127">In the request body, supply a JSON representation for the groupPolicyPresentationTextBox object.</span></span>

<span data-ttu-id="25f5a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyPresentationTextBox.</span><span class="sxs-lookup"><span data-stu-id="25f5a-128">The following table shows the properties that are required when you create the groupPolicyPresentationTextBox.</span></span>

|<span data-ttu-id="25f5a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25f5a-129">Property</span></span>|<span data-ttu-id="25f5a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="25f5a-130">Type</span></span>|<span data-ttu-id="25f5a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="25f5a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25f5a-132">rótulo</span><span class="sxs-lookup"><span data-stu-id="25f5a-132">label</span></span>|<span data-ttu-id="25f5a-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25f5a-133">String</span></span>|<span data-ttu-id="25f5a-134">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="25f5a-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="25f5a-135">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="25f5a-135">The default value is empty.</span></span> <span data-ttu-id="25f5a-136">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="25f5a-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="25f5a-137">id</span><span class="sxs-lookup"><span data-stu-id="25f5a-137">id</span></span>|<span data-ttu-id="25f5a-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25f5a-138">String</span></span>|<span data-ttu-id="25f5a-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="25f5a-139">Key of the entity.</span></span> <span data-ttu-id="25f5a-140">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="25f5a-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="25f5a-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="25f5a-141">lastModifiedDateTime</span></span>|<span data-ttu-id="25f5a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25f5a-142">DateTimeOffset</span></span>|<span data-ttu-id="25f5a-143">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="25f5a-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="25f5a-144">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="25f5a-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="25f5a-145">defaultValue</span><span class="sxs-lookup"><span data-stu-id="25f5a-145">defaultValue</span></span>|<span data-ttu-id="25f5a-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25f5a-146">String</span></span>|<span data-ttu-id="25f5a-147">Cadeia de caracteres padrão localizada exibida na caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="25f5a-147">Localized default string displayed in the text box.</span></span> <span data-ttu-id="25f5a-148">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="25f5a-148">The default value is empty.</span></span>|
|<span data-ttu-id="25f5a-149">obrigatório</span><span class="sxs-lookup"><span data-stu-id="25f5a-149">required</span></span>|<span data-ttu-id="25f5a-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="25f5a-150">Boolean</span></span>|<span data-ttu-id="25f5a-151">Requisito para inserir um valor na caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="25f5a-151">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="25f5a-152">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="25f5a-152">Default value is false.</span></span>|
|<span data-ttu-id="25f5a-153">maxLength</span><span class="sxs-lookup"><span data-stu-id="25f5a-153">maxLength</span></span>|<span data-ttu-id="25f5a-154">Int64</span><span class="sxs-lookup"><span data-stu-id="25f5a-154">Int64</span></span>|<span data-ttu-id="25f5a-155">Um inteiro sem sinal que especifica o número máximo de caracteres de texto.</span><span class="sxs-lookup"><span data-stu-id="25f5a-155">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="25f5a-156">O valor padrão é 1023.</span><span class="sxs-lookup"><span data-stu-id="25f5a-156">Default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="25f5a-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="25f5a-157">Response</span></span>
<span data-ttu-id="25f5a-158">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25f5a-158">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25f5a-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25f5a-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="25f5a-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25f5a-160">Request</span></span>
<span data-ttu-id="25f5a-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="25f5a-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
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

### <a name="response"></a><span data-ttu-id="25f5a-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="25f5a-162">Response</span></span>
<span data-ttu-id="25f5a-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="25f5a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




