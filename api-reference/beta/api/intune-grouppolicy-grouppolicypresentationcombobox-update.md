---
title: Atualizar groupPolicyPresentationComboBox
description: Atualize as propriedades de um objeto groupPolicyPresentationComboBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a3fa1ef56577fe13a21367e4844be41870538df
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149699"
---
# <a name="update-grouppolicypresentationcombobox"></a><span data-ttu-id="430c7-103">Atualizar groupPolicyPresentationComboBox</span><span class="sxs-lookup"><span data-stu-id="430c7-103">Update groupPolicyPresentationComboBox</span></span>

<span data-ttu-id="430c7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="430c7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="430c7-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="430c7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="430c7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="430c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="430c7-107">Atualize as propriedades de [um objeto groupPolicyPresentationComboBox.](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)</span><span class="sxs-lookup"><span data-stu-id="430c7-107">Update the properties of a [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="430c7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="430c7-108">Prerequisites</span></span>
<span data-ttu-id="430c7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="430c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="430c7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="430c7-111">Permission type</span></span>|<span data-ttu-id="430c7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="430c7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="430c7-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="430c7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="430c7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="430c7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="430c7-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="430c7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="430c7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="430c7-116">Not supported.</span></span>|
|<span data-ttu-id="430c7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="430c7-117">Application</span></span>|<span data-ttu-id="430c7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="430c7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="430c7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="430c7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="430c7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="430c7-120">Request headers</span></span>
|<span data-ttu-id="430c7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="430c7-121">Header</span></span>|<span data-ttu-id="430c7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="430c7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="430c7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="430c7-123">Authorization</span></span>|<span data-ttu-id="430c7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="430c7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="430c7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="430c7-125">Accept</span></span>|<span data-ttu-id="430c7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="430c7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="430c7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="430c7-127">Request body</span></span>
<span data-ttu-id="430c7-128">No corpo da solicitação, fornece uma representação JSON para o [objeto groupPolicyPresentationComboBox.](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)</span><span class="sxs-lookup"><span data-stu-id="430c7-128">In the request body, supply a JSON representation for the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

<span data-ttu-id="430c7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md).</span><span class="sxs-lookup"><span data-stu-id="430c7-129">The following table shows the properties that are required when you create the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md).</span></span>

|<span data-ttu-id="430c7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="430c7-130">Property</span></span>|<span data-ttu-id="430c7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="430c7-131">Type</span></span>|<span data-ttu-id="430c7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="430c7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="430c7-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="430c7-133">label</span></span>|<span data-ttu-id="430c7-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="430c7-134">String</span></span>|<span data-ttu-id="430c7-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="430c7-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="430c7-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="430c7-136">The default value is empty.</span></span> <span data-ttu-id="430c7-137">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="430c7-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="430c7-138">id</span><span class="sxs-lookup"><span data-stu-id="430c7-138">id</span></span>|<span data-ttu-id="430c7-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="430c7-139">String</span></span>|<span data-ttu-id="430c7-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="430c7-140">Key of the entity.</span></span> <span data-ttu-id="430c7-141">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="430c7-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="430c7-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="430c7-142">lastModifiedDateTime</span></span>|<span data-ttu-id="430c7-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="430c7-143">DateTimeOffset</span></span>|<span data-ttu-id="430c7-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="430c7-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="430c7-145">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="430c7-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="430c7-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="430c7-146">defaultValue</span></span>|<span data-ttu-id="430c7-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="430c7-147">String</span></span>|<span data-ttu-id="430c7-148">Cadeia de caracteres padrão localizada exibida na caixa de combinação.</span><span class="sxs-lookup"><span data-stu-id="430c7-148">Localized default string displayed in the combo box.</span></span> <span data-ttu-id="430c7-149">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="430c7-149">The default value is empty.</span></span>|
|<span data-ttu-id="430c7-150">sugestões</span><span class="sxs-lookup"><span data-stu-id="430c7-150">suggestions</span></span>|<span data-ttu-id="430c7-151">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="430c7-151">String collection</span></span>|<span data-ttu-id="430c7-152">Cadeias de caracteres localizadas listadas na listada da caixa de combinação.</span><span class="sxs-lookup"><span data-stu-id="430c7-152">Localized strings listed in the drop-down list of the combo box.</span></span> <span data-ttu-id="430c7-153">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="430c7-153">The default value is empty.</span></span>|
|<span data-ttu-id="430c7-154">obrigatório</span><span class="sxs-lookup"><span data-stu-id="430c7-154">required</span></span>|<span data-ttu-id="430c7-155">Booleano</span><span class="sxs-lookup"><span data-stu-id="430c7-155">Boolean</span></span>|<span data-ttu-id="430c7-156">Especifica se um valor deve ser especificado para o parâmetro.</span><span class="sxs-lookup"><span data-stu-id="430c7-156">Specifies whether a value must be specified for the parameter.</span></span> <span data-ttu-id="430c7-157">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="430c7-157">The default value is false.</span></span>|
|<span data-ttu-id="430c7-158">maxLength</span><span class="sxs-lookup"><span data-stu-id="430c7-158">maxLength</span></span>|<span data-ttu-id="430c7-159">Int64</span><span class="sxs-lookup"><span data-stu-id="430c7-159">Int64</span></span>|<span data-ttu-id="430c7-160">Um inteiro não assinado que especifica o número máximo de caracteres de texto para o parâmetro.</span><span class="sxs-lookup"><span data-stu-id="430c7-160">An unsigned integer that specifies the maximum number of text characters for the parameter.</span></span> <span data-ttu-id="430c7-161">O valor padrão é 1023.</span><span class="sxs-lookup"><span data-stu-id="430c7-161">The default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="430c7-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="430c7-162">Response</span></span>
<span data-ttu-id="430c7-163">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="430c7-163">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="430c7-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="430c7-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="430c7-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="430c7-165">Request</span></span>
<span data-ttu-id="430c7-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="430c7-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 233

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
  "label": "Label value",
  "defaultValue": "Default Value value",
  "suggestions": [
    "Suggestions value"
  ],
  "required": true,
  "maxLength": 9
}
```

### <a name="response"></a><span data-ttu-id="430c7-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="430c7-167">Response</span></span>
<span data-ttu-id="430c7-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="430c7-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
  "label": "Label value",
  "id": "44332a1d-2a1d-4433-1d2a-33441d2a3344",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": "Default Value value",
  "suggestions": [
    "Suggestions value"
  ],
  "required": true,
  "maxLength": 9
}
```




