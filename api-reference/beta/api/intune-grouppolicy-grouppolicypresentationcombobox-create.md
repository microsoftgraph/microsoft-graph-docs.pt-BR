---
title: Criar groupPolicyPresentationComboBox
description: Criar um novo objeto groupPolicyPresentationComboBox.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 30952aa522378b3c8a881ddb6549e8a48946f493
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975965"
---
# <a name="create-grouppolicypresentationcombobox"></a><span data-ttu-id="63969-103">Criar groupPolicyPresentationComboBox</span><span class="sxs-lookup"><span data-stu-id="63969-103">Create groupPolicyPresentationComboBox</span></span>

> <span data-ttu-id="63969-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="63969-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63969-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63969-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63969-106">Criar um novo objeto [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .</span><span class="sxs-lookup"><span data-stu-id="63969-106">Create a new [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63969-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="63969-107">Prerequisites</span></span>
<span data-ttu-id="63969-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63969-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63969-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63969-110">Permission type</span></span>|<span data-ttu-id="63969-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="63969-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63969-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63969-112">Delegated (work or school account)</span></span>|<span data-ttu-id="63969-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63969-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="63969-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63969-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63969-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63969-115">Not supported.</span></span>|
|<span data-ttu-id="63969-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63969-116">Application</span></span>|<span data-ttu-id="63969-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63969-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63969-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63969-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="63969-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63969-119">Request headers</span></span>
|<span data-ttu-id="63969-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63969-120">Header</span></span>|<span data-ttu-id="63969-121">Valor</span><span class="sxs-lookup"><span data-stu-id="63969-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63969-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="63969-122">Authorization</span></span>|<span data-ttu-id="63969-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63969-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63969-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="63969-124">Accept</span></span>|<span data-ttu-id="63969-125">application/json</span><span class="sxs-lookup"><span data-stu-id="63969-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63969-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63969-126">Request body</span></span>
<span data-ttu-id="63969-127">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyPresentationComboBox.</span><span class="sxs-lookup"><span data-stu-id="63969-127">In the request body, supply a JSON representation for the groupPolicyPresentationComboBox object.</span></span>

<span data-ttu-id="63969-128">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyPresentationComboBox.</span><span class="sxs-lookup"><span data-stu-id="63969-128">The following table shows the properties that are required when you create the groupPolicyPresentationComboBox.</span></span>

|<span data-ttu-id="63969-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63969-129">Property</span></span>|<span data-ttu-id="63969-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="63969-130">Type</span></span>|<span data-ttu-id="63969-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="63969-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63969-132">rótulo</span><span class="sxs-lookup"><span data-stu-id="63969-132">label</span></span>|<span data-ttu-id="63969-133">String</span><span class="sxs-lookup"><span data-stu-id="63969-133">String</span></span>|<span data-ttu-id="63969-134">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="63969-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="63969-135">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="63969-135">The default value is empty.</span></span> <span data-ttu-id="63969-136">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="63969-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="63969-137">id</span><span class="sxs-lookup"><span data-stu-id="63969-137">id</span></span>|<span data-ttu-id="63969-138">String</span><span class="sxs-lookup"><span data-stu-id="63969-138">String</span></span>|<span data-ttu-id="63969-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="63969-139">Key of the entity.</span></span> <span data-ttu-id="63969-140">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="63969-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="63969-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="63969-141">lastModifiedDateTime</span></span>|<span data-ttu-id="63969-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63969-142">DateTimeOffset</span></span>|<span data-ttu-id="63969-143">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="63969-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="63969-144">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="63969-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="63969-145">defaultValue</span><span class="sxs-lookup"><span data-stu-id="63969-145">defaultValue</span></span>|<span data-ttu-id="63969-146">String</span><span class="sxs-lookup"><span data-stu-id="63969-146">String</span></span>|<span data-ttu-id="63969-147">Cadeia de caracteres padrão localizada exibida na caixa de combinação.</span><span class="sxs-lookup"><span data-stu-id="63969-147">Localized default string displayed in the combo box.</span></span> <span data-ttu-id="63969-148">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="63969-148">The default value is empty.</span></span>|
|<span data-ttu-id="63969-149">enviou</span><span class="sxs-lookup"><span data-stu-id="63969-149">suggestions</span></span>|<span data-ttu-id="63969-150">Coleção String</span><span class="sxs-lookup"><span data-stu-id="63969-150">String collection</span></span>|<span data-ttu-id="63969-151">Cadeias de caracteres localizadas listadas na lista suspensa da caixa de combinação.</span><span class="sxs-lookup"><span data-stu-id="63969-151">Localized strings listed in the drop-down list of the combo box.</span></span> <span data-ttu-id="63969-152">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="63969-152">The default value is empty.</span></span>|
|<span data-ttu-id="63969-153">obrigatório</span><span class="sxs-lookup"><span data-stu-id="63969-153">required</span></span>|<span data-ttu-id="63969-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="63969-154">Boolean</span></span>|<span data-ttu-id="63969-155">Especifica se um valor deve ser especificado para o parâmetro.</span><span class="sxs-lookup"><span data-stu-id="63969-155">Specifies whether a value must be specified for the parameter.</span></span> <span data-ttu-id="63969-156">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="63969-156">The default value is false.</span></span>|
|<span data-ttu-id="63969-157">maxLength</span><span class="sxs-lookup"><span data-stu-id="63969-157">maxLength</span></span>|<span data-ttu-id="63969-158">Int64</span><span class="sxs-lookup"><span data-stu-id="63969-158">Int64</span></span>|<span data-ttu-id="63969-159">Um inteiro sem sinal que especifica o número máximo de caracteres de texto para o parâmetro.</span><span class="sxs-lookup"><span data-stu-id="63969-159">An unsigned integer that specifies the maximum number of text characters for the parameter.</span></span> <span data-ttu-id="63969-160">O valor padrão é 1023.</span><span class="sxs-lookup"><span data-stu-id="63969-160">The default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="63969-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="63969-161">Response</span></span>
<span data-ttu-id="63969-162">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63969-162">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63969-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63969-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="63969-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63969-164">Request</span></span>
<span data-ttu-id="63969-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63969-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
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

### <a name="response"></a><span data-ttu-id="63969-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="63969-166">Response</span></span>
<span data-ttu-id="63969-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63969-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




