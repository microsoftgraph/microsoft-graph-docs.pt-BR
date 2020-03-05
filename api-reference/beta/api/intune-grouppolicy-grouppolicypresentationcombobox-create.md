---
title: Criar groupPolicyPresentationComboBox
description: Criar um novo objeto groupPolicyPresentationComboBox.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 95e693ff7c4861659a33f363c10a7fc6887bfe44
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42464900"
---
# <a name="create-grouppolicypresentationcombobox"></a><span data-ttu-id="cdabe-103">Criar groupPolicyPresentationComboBox</span><span class="sxs-lookup"><span data-stu-id="cdabe-103">Create groupPolicyPresentationComboBox</span></span>

<span data-ttu-id="cdabe-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cdabe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cdabe-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cdabe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdabe-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cdabe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdabe-107">Criar um novo objeto [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .</span><span class="sxs-lookup"><span data-stu-id="cdabe-107">Create a new [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cdabe-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cdabe-108">Prerequisites</span></span>
<span data-ttu-id="cdabe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdabe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdabe-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cdabe-111">Permission type</span></span>|<span data-ttu-id="cdabe-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cdabe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdabe-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cdabe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cdabe-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdabe-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cdabe-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cdabe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdabe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cdabe-116">Not supported.</span></span>|
|<span data-ttu-id="cdabe-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cdabe-117">Application</span></span>|<span data-ttu-id="cdabe-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdabe-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdabe-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cdabe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="cdabe-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cdabe-120">Request headers</span></span>
|<span data-ttu-id="cdabe-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cdabe-121">Header</span></span>|<span data-ttu-id="cdabe-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cdabe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdabe-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cdabe-123">Authorization</span></span>|<span data-ttu-id="cdabe-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cdabe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdabe-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cdabe-125">Accept</span></span>|<span data-ttu-id="cdabe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cdabe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdabe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cdabe-127">Request body</span></span>
<span data-ttu-id="cdabe-128">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyPresentationComboBox.</span><span class="sxs-lookup"><span data-stu-id="cdabe-128">In the request body, supply a JSON representation for the groupPolicyPresentationComboBox object.</span></span>

<span data-ttu-id="cdabe-129">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyPresentationComboBox.</span><span class="sxs-lookup"><span data-stu-id="cdabe-129">The following table shows the properties that are required when you create the groupPolicyPresentationComboBox.</span></span>

|<span data-ttu-id="cdabe-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cdabe-130">Property</span></span>|<span data-ttu-id="cdabe-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cdabe-131">Type</span></span>|<span data-ttu-id="cdabe-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdabe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdabe-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="cdabe-133">label</span></span>|<span data-ttu-id="cdabe-134">String</span><span class="sxs-lookup"><span data-stu-id="cdabe-134">String</span></span>|<span data-ttu-id="cdabe-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="cdabe-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="cdabe-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="cdabe-136">The default value is empty.</span></span> <span data-ttu-id="cdabe-137">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="cdabe-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="cdabe-138">id</span><span class="sxs-lookup"><span data-stu-id="cdabe-138">id</span></span>|<span data-ttu-id="cdabe-139">String</span><span class="sxs-lookup"><span data-stu-id="cdabe-139">String</span></span>|<span data-ttu-id="cdabe-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cdabe-140">Key of the entity.</span></span> <span data-ttu-id="cdabe-141">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="cdabe-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="cdabe-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cdabe-142">lastModifiedDateTime</span></span>|<span data-ttu-id="cdabe-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdabe-143">DateTimeOffset</span></span>|<span data-ttu-id="cdabe-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="cdabe-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="cdabe-145">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="cdabe-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="cdabe-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="cdabe-146">defaultValue</span></span>|<span data-ttu-id="cdabe-147">String</span><span class="sxs-lookup"><span data-stu-id="cdabe-147">String</span></span>|<span data-ttu-id="cdabe-148">Cadeia de caracteres padrão localizada exibida na caixa de combinação.</span><span class="sxs-lookup"><span data-stu-id="cdabe-148">Localized default string displayed in the combo box.</span></span> <span data-ttu-id="cdabe-149">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="cdabe-149">The default value is empty.</span></span>|
|<span data-ttu-id="cdabe-150">enviou</span><span class="sxs-lookup"><span data-stu-id="cdabe-150">suggestions</span></span>|<span data-ttu-id="cdabe-151">String collection</span><span class="sxs-lookup"><span data-stu-id="cdabe-151">String collection</span></span>|<span data-ttu-id="cdabe-152">Cadeias de caracteres localizadas listadas na lista suspensa da caixa de combinação.</span><span class="sxs-lookup"><span data-stu-id="cdabe-152">Localized strings listed in the drop-down list of the combo box.</span></span> <span data-ttu-id="cdabe-153">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="cdabe-153">The default value is empty.</span></span>|
|<span data-ttu-id="cdabe-154">obrigatório</span><span class="sxs-lookup"><span data-stu-id="cdabe-154">required</span></span>|<span data-ttu-id="cdabe-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="cdabe-155">Boolean</span></span>|<span data-ttu-id="cdabe-156">Especifica se um valor deve ser especificado para o parâmetro.</span><span class="sxs-lookup"><span data-stu-id="cdabe-156">Specifies whether a value must be specified for the parameter.</span></span> <span data-ttu-id="cdabe-157">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="cdabe-157">The default value is false.</span></span>|
|<span data-ttu-id="cdabe-158">maxLength</span><span class="sxs-lookup"><span data-stu-id="cdabe-158">maxLength</span></span>|<span data-ttu-id="cdabe-159">Int64</span><span class="sxs-lookup"><span data-stu-id="cdabe-159">Int64</span></span>|<span data-ttu-id="cdabe-160">Um inteiro sem sinal que especifica o número máximo de caracteres de texto para o parâmetro.</span><span class="sxs-lookup"><span data-stu-id="cdabe-160">An unsigned integer that specifies the maximum number of text characters for the parameter.</span></span> <span data-ttu-id="cdabe-161">O valor padrão é 1023.</span><span class="sxs-lookup"><span data-stu-id="cdabe-161">The default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="cdabe-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdabe-162">Response</span></span>
<span data-ttu-id="cdabe-163">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdabe-163">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdabe-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cdabe-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="cdabe-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cdabe-165">Request</span></span>
<span data-ttu-id="cdabe-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cdabe-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cdabe-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdabe-167">Response</span></span>
<span data-ttu-id="cdabe-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cdabe-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





