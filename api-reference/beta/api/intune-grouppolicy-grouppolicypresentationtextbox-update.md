---
title: Atualizar groupPolicyPresentationTextBox
description: Atualize as propriedades de um objeto groupPolicyPresentationTextBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5ff83558c1d66505e0623d4cd9b48ef83f033f37
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157388"
---
# <a name="update-grouppolicypresentationtextbox"></a><span data-ttu-id="31cd1-103">Atualizar groupPolicyPresentationTextBox</span><span class="sxs-lookup"><span data-stu-id="31cd1-103">Update groupPolicyPresentationTextBox</span></span>

<span data-ttu-id="31cd1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31cd1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="31cd1-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="31cd1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31cd1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="31cd1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31cd1-107">Atualize as propriedades de [um objeto groupPolicyPresentationTextBox.](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)</span><span class="sxs-lookup"><span data-stu-id="31cd1-107">Update the properties of a [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31cd1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="31cd1-108">Prerequisites</span></span>
<span data-ttu-id="31cd1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31cd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31cd1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31cd1-111">Permission type</span></span>|<span data-ttu-id="31cd1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31cd1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31cd1-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31cd1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="31cd1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31cd1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="31cd1-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31cd1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31cd1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31cd1-116">Not supported.</span></span>|
|<span data-ttu-id="31cd1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31cd1-117">Application</span></span>|<span data-ttu-id="31cd1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31cd1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31cd1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31cd1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="31cd1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31cd1-120">Request headers</span></span>
|<span data-ttu-id="31cd1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="31cd1-121">Header</span></span>|<span data-ttu-id="31cd1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="31cd1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31cd1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="31cd1-123">Authorization</span></span>|<span data-ttu-id="31cd1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31cd1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31cd1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="31cd1-125">Accept</span></span>|<span data-ttu-id="31cd1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="31cd1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31cd1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31cd1-127">Request body</span></span>
<span data-ttu-id="31cd1-128">No corpo da solicitação, fornece uma representação JSON para o [objeto groupPolicyPresentationTextBox.](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)</span><span class="sxs-lookup"><span data-stu-id="31cd1-128">In the request body, supply a JSON representation for the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

<span data-ttu-id="31cd1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md).</span><span class="sxs-lookup"><span data-stu-id="31cd1-129">The following table shows the properties that are required when you create the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md).</span></span>

|<span data-ttu-id="31cd1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31cd1-130">Property</span></span>|<span data-ttu-id="31cd1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="31cd1-131">Type</span></span>|<span data-ttu-id="31cd1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="31cd1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31cd1-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="31cd1-133">label</span></span>|<span data-ttu-id="31cd1-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31cd1-134">String</span></span>|<span data-ttu-id="31cd1-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="31cd1-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="31cd1-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="31cd1-136">The default value is empty.</span></span> <span data-ttu-id="31cd1-137">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="31cd1-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="31cd1-138">id</span><span class="sxs-lookup"><span data-stu-id="31cd1-138">id</span></span>|<span data-ttu-id="31cd1-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31cd1-139">String</span></span>|<span data-ttu-id="31cd1-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="31cd1-140">Key of the entity.</span></span> <span data-ttu-id="31cd1-141">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="31cd1-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="31cd1-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="31cd1-142">lastModifiedDateTime</span></span>|<span data-ttu-id="31cd1-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31cd1-143">DateTimeOffset</span></span>|<span data-ttu-id="31cd1-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="31cd1-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="31cd1-145">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="31cd1-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="31cd1-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="31cd1-146">defaultValue</span></span>|<span data-ttu-id="31cd1-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31cd1-147">String</span></span>|<span data-ttu-id="31cd1-148">Cadeia de caracteres padrão localizada exibida na caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="31cd1-148">Localized default string displayed in the text box.</span></span> <span data-ttu-id="31cd1-149">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="31cd1-149">The default value is empty.</span></span>|
|<span data-ttu-id="31cd1-150">obrigatório</span><span class="sxs-lookup"><span data-stu-id="31cd1-150">required</span></span>|<span data-ttu-id="31cd1-151">Booleano</span><span class="sxs-lookup"><span data-stu-id="31cd1-151">Boolean</span></span>|<span data-ttu-id="31cd1-152">Requisito para inserir um valor na caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="31cd1-152">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="31cd1-153">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="31cd1-153">Default value is false.</span></span>|
|<span data-ttu-id="31cd1-154">maxLength</span><span class="sxs-lookup"><span data-stu-id="31cd1-154">maxLength</span></span>|<span data-ttu-id="31cd1-155">Int64</span><span class="sxs-lookup"><span data-stu-id="31cd1-155">Int64</span></span>|<span data-ttu-id="31cd1-156">Um inteiro não assinado que especifica o número máximo de caracteres de texto.</span><span class="sxs-lookup"><span data-stu-id="31cd1-156">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="31cd1-157">O valor padrão é 1023.</span><span class="sxs-lookup"><span data-stu-id="31cd1-157">Default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="31cd1-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="31cd1-158">Response</span></span>
<span data-ttu-id="31cd1-159">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31cd1-159">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31cd1-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31cd1-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="31cd1-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31cd1-161">Request</span></span>
<span data-ttu-id="31cd1-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="31cd1-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="31cd1-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="31cd1-163">Response</span></span>
<span data-ttu-id="31cd1-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31cd1-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




