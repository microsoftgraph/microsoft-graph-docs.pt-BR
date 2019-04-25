---
title: Atualizar groupPolicyPresentationComboBox
description: Atualiza as propriedades de um objeto groupPolicyPresentationComboBox.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4df510c4dab590c97a5399a1ab453afa2099bc1f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32531247"
---
# <a name="update-grouppolicypresentationcombobox"></a><span data-ttu-id="86a98-103">Atualizar groupPolicyPresentationComboBox</span><span class="sxs-lookup"><span data-stu-id="86a98-103">Update groupPolicyPresentationComboBox</span></span>

> <span data-ttu-id="86a98-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="86a98-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86a98-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="86a98-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86a98-106">Atualiza as propriedades de um objeto [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .</span><span class="sxs-lookup"><span data-stu-id="86a98-106">Update the properties of a [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86a98-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="86a98-107">Prerequisites</span></span>
<span data-ttu-id="86a98-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86a98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86a98-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86a98-110">Permission type</span></span>|<span data-ttu-id="86a98-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="86a98-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86a98-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86a98-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86a98-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86a98-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="86a98-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86a98-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86a98-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86a98-115">Not supported.</span></span>|
|<span data-ttu-id="86a98-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86a98-116">Application</span></span>|<span data-ttu-id="86a98-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86a98-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86a98-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86a98-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="86a98-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86a98-119">Request headers</span></span>
|<span data-ttu-id="86a98-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86a98-120">Header</span></span>|<span data-ttu-id="86a98-121">Valor</span><span class="sxs-lookup"><span data-stu-id="86a98-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86a98-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="86a98-122">Authorization</span></span>|<span data-ttu-id="86a98-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86a98-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86a98-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="86a98-124">Accept</span></span>|<span data-ttu-id="86a98-125">application/json</span><span class="sxs-lookup"><span data-stu-id="86a98-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86a98-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86a98-126">Request body</span></span>
<span data-ttu-id="86a98-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .</span><span class="sxs-lookup"><span data-stu-id="86a98-127">In the request body, supply a JSON representation for the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

<span data-ttu-id="86a98-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md).</span><span class="sxs-lookup"><span data-stu-id="86a98-128">The following table shows the properties that are required when you create the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md).</span></span>

|<span data-ttu-id="86a98-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86a98-129">Property</span></span>|<span data-ttu-id="86a98-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="86a98-130">Type</span></span>|<span data-ttu-id="86a98-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="86a98-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86a98-132">rótulo</span><span class="sxs-lookup"><span data-stu-id="86a98-132">label</span></span>|<span data-ttu-id="86a98-133">String</span><span class="sxs-lookup"><span data-stu-id="86a98-133">String</span></span>|<span data-ttu-id="86a98-134">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="86a98-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="86a98-135">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="86a98-135">The default value is empty.</span></span> <span data-ttu-id="86a98-136">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="86a98-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="86a98-137">id</span><span class="sxs-lookup"><span data-stu-id="86a98-137">id</span></span>|<span data-ttu-id="86a98-138">String</span><span class="sxs-lookup"><span data-stu-id="86a98-138">String</span></span>|<span data-ttu-id="86a98-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="86a98-139">Key of the entity.</span></span> <span data-ttu-id="86a98-140">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="86a98-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="86a98-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86a98-141">lastModifiedDateTime</span></span>|<span data-ttu-id="86a98-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86a98-142">DateTimeOffset</span></span>|<span data-ttu-id="86a98-143">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="86a98-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="86a98-144">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="86a98-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="86a98-145">defaultValue</span><span class="sxs-lookup"><span data-stu-id="86a98-145">defaultValue</span></span>|<span data-ttu-id="86a98-146">String</span><span class="sxs-lookup"><span data-stu-id="86a98-146">String</span></span>|<span data-ttu-id="86a98-147">Cadeia de caracteres padrão localizada exibida na caixa de combinação.</span><span class="sxs-lookup"><span data-stu-id="86a98-147">Localized default string displayed in the combo box.</span></span> <span data-ttu-id="86a98-148">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="86a98-148">The default value is empty.</span></span>|
|<span data-ttu-id="86a98-149">enviou</span><span class="sxs-lookup"><span data-stu-id="86a98-149">suggestions</span></span>|<span data-ttu-id="86a98-150">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="86a98-150">String collection</span></span>|<span data-ttu-id="86a98-151">Cadeias de caracteres localizadas listadas na lista suspensa da caixa de combinação.</span><span class="sxs-lookup"><span data-stu-id="86a98-151">Localized strings listed in the drop-down list of the combo box.</span></span> <span data-ttu-id="86a98-152">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="86a98-152">The default value is empty.</span></span>|
|<span data-ttu-id="86a98-153">obrigatório</span><span class="sxs-lookup"><span data-stu-id="86a98-153">required</span></span>|<span data-ttu-id="86a98-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="86a98-154">Boolean</span></span>|<span data-ttu-id="86a98-155">Especifica se um valor deve ser especificado para o parâmetro.</span><span class="sxs-lookup"><span data-stu-id="86a98-155">Specifies whether a value must be specified for the parameter.</span></span> <span data-ttu-id="86a98-156">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="86a98-156">The default value is false.</span></span>|
|<span data-ttu-id="86a98-157">maxLength</span><span class="sxs-lookup"><span data-stu-id="86a98-157">maxLength</span></span>|<span data-ttu-id="86a98-158">Int64</span><span class="sxs-lookup"><span data-stu-id="86a98-158">Int64</span></span>|<span data-ttu-id="86a98-159">Um inteiro sem sinal que especifica o número máximo de caracteres de texto para o parâmetro.</span><span class="sxs-lookup"><span data-stu-id="86a98-159">An unsigned integer that specifies the maximum number of text characters for the parameter.</span></span> <span data-ttu-id="86a98-160">O valor padrão é 1023.</span><span class="sxs-lookup"><span data-stu-id="86a98-160">The default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="86a98-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="86a98-161">Response</span></span>
<span data-ttu-id="86a98-162">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86a98-162">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86a98-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86a98-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="86a98-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86a98-164">Request</span></span>
<span data-ttu-id="86a98-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86a98-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="86a98-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="86a98-166">Response</span></span>
<span data-ttu-id="86a98-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86a98-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





