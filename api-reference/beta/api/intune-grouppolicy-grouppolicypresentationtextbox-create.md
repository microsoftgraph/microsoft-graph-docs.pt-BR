---
title: Criar groupPolicyPresentationTextBox
description: Crie um novo objeto groupPolicyPresentationTextBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7e5d23f310744c55522e54a74a77d21dc50d405d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149426"
---
# <a name="create-grouppolicypresentationtextbox"></a><span data-ttu-id="ded15-103">Criar groupPolicyPresentationTextBox</span><span class="sxs-lookup"><span data-stu-id="ded15-103">Create groupPolicyPresentationTextBox</span></span>

<span data-ttu-id="ded15-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ded15-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ded15-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ded15-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ded15-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ded15-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ded15-107">Crie um novo [objeto groupPolicyPresentationTextBox.](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)</span><span class="sxs-lookup"><span data-stu-id="ded15-107">Create a new [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ded15-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ded15-108">Prerequisites</span></span>
<span data-ttu-id="ded15-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ded15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ded15-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ded15-111">Permission type</span></span>|<span data-ttu-id="ded15-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ded15-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ded15-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ded15-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ded15-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ded15-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ded15-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ded15-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ded15-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ded15-116">Not supported.</span></span>|
|<span data-ttu-id="ded15-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ded15-117">Application</span></span>|<span data-ttu-id="ded15-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ded15-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ded15-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ded15-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="ded15-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ded15-120">Request headers</span></span>
|<span data-ttu-id="ded15-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ded15-121">Header</span></span>|<span data-ttu-id="ded15-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ded15-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ded15-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ded15-123">Authorization</span></span>|<span data-ttu-id="ded15-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ded15-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ded15-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ded15-125">Accept</span></span>|<span data-ttu-id="ded15-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ded15-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ded15-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ded15-127">Request body</span></span>
<span data-ttu-id="ded15-128">No corpo da solicitação, fornece uma representação JSON para o objeto groupPolicyPresentationTextBox.</span><span class="sxs-lookup"><span data-stu-id="ded15-128">In the request body, supply a JSON representation for the groupPolicyPresentationTextBox object.</span></span>

<span data-ttu-id="ded15-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o groupPolicyPresentationTextBox.</span><span class="sxs-lookup"><span data-stu-id="ded15-129">The following table shows the properties that are required when you create the groupPolicyPresentationTextBox.</span></span>

|<span data-ttu-id="ded15-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ded15-130">Property</span></span>|<span data-ttu-id="ded15-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ded15-131">Type</span></span>|<span data-ttu-id="ded15-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ded15-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ded15-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="ded15-133">label</span></span>|<span data-ttu-id="ded15-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ded15-134">String</span></span>|<span data-ttu-id="ded15-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="ded15-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="ded15-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="ded15-136">The default value is empty.</span></span> <span data-ttu-id="ded15-137">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ded15-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ded15-138">id</span><span class="sxs-lookup"><span data-stu-id="ded15-138">id</span></span>|<span data-ttu-id="ded15-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ded15-139">String</span></span>|<span data-ttu-id="ded15-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ded15-140">Key of the entity.</span></span> <span data-ttu-id="ded15-141">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ded15-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ded15-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ded15-142">lastModifiedDateTime</span></span>|<span data-ttu-id="ded15-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ded15-143">DateTimeOffset</span></span>|<span data-ttu-id="ded15-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ded15-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="ded15-145">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ded15-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ded15-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="ded15-146">defaultValue</span></span>|<span data-ttu-id="ded15-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ded15-147">String</span></span>|<span data-ttu-id="ded15-148">Cadeia de caracteres padrão localizada exibida na caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="ded15-148">Localized default string displayed in the text box.</span></span> <span data-ttu-id="ded15-149">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="ded15-149">The default value is empty.</span></span>|
|<span data-ttu-id="ded15-150">obrigatório</span><span class="sxs-lookup"><span data-stu-id="ded15-150">required</span></span>|<span data-ttu-id="ded15-151">Booleano</span><span class="sxs-lookup"><span data-stu-id="ded15-151">Boolean</span></span>|<span data-ttu-id="ded15-152">Requisito para inserir um valor na caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="ded15-152">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="ded15-153">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="ded15-153">Default value is false.</span></span>|
|<span data-ttu-id="ded15-154">maxLength</span><span class="sxs-lookup"><span data-stu-id="ded15-154">maxLength</span></span>|<span data-ttu-id="ded15-155">Int64</span><span class="sxs-lookup"><span data-stu-id="ded15-155">Int64</span></span>|<span data-ttu-id="ded15-156">Um inteiro não assinado que especifica o número máximo de caracteres de texto.</span><span class="sxs-lookup"><span data-stu-id="ded15-156">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="ded15-157">O valor padrão é 1023.</span><span class="sxs-lookup"><span data-stu-id="ded15-157">Default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="ded15-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="ded15-158">Response</span></span>
<span data-ttu-id="ded15-159">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ded15-159">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ded15-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ded15-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="ded15-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ded15-161">Request</span></span>
<span data-ttu-id="ded15-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ded15-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ded15-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="ded15-163">Response</span></span>
<span data-ttu-id="ded15-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ded15-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




