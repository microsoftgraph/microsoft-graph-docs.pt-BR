---
title: Atualizar groupPolicyPresentationComboBox
description: Atualize as propriedades de um objeto groupPolicyPresentationComboBox.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6302d52e91e5fe1cf8a21e525d0eccef608b3b24
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429169"
---
# <a name="update-grouppolicypresentationcombobox"></a><span data-ttu-id="ccd7f-103">Atualizar groupPolicyPresentationComboBox</span><span class="sxs-lookup"><span data-stu-id="ccd7f-103">Update groupPolicyPresentationComboBox</span></span>

> <span data-ttu-id="ccd7f-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ccd7f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ccd7f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ccd7f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ccd7f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="ccd7f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccd7f-107">Atualize as propriedades de um objeto [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .</span><span class="sxs-lookup"><span data-stu-id="ccd7f-107">Update the properties of a [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ccd7f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ccd7f-108">Prerequisites</span></span>
<span data-ttu-id="ccd7f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ccd7f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ccd7f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ccd7f-111">Permission type</span></span>|<span data-ttu-id="ccd7f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ccd7f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ccd7f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ccd7f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ccd7f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccd7f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ccd7f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ccd7f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccd7f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ccd7f-116">Not supported.</span></span>|
|<span data-ttu-id="ccd7f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ccd7f-117">Application</span></span>|<span data-ttu-id="ccd7f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ccd7f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccd7f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ccd7f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="ccd7f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ccd7f-120">Request headers</span></span>
|<span data-ttu-id="ccd7f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ccd7f-121">Header</span></span>|<span data-ttu-id="ccd7f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ccd7f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ccd7f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ccd7f-123">Authorization</span></span>|<span data-ttu-id="ccd7f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ccd7f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ccd7f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ccd7f-125">Accept</span></span>|<span data-ttu-id="ccd7f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ccd7f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccd7f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ccd7f-127">Request body</span></span>
<span data-ttu-id="ccd7f-128">No corpo da solicitação, fornece uma representação JSON para o objeto [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .</span><span class="sxs-lookup"><span data-stu-id="ccd7f-128">In the request body, supply a JSON representation for the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

<span data-ttu-id="ccd7f-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md).</span><span class="sxs-lookup"><span data-stu-id="ccd7f-129">The following table shows the properties that are required when you create the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md).</span></span>

|<span data-ttu-id="ccd7f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ccd7f-130">Property</span></span>|<span data-ttu-id="ccd7f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccd7f-131">Type</span></span>|<span data-ttu-id="ccd7f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccd7f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccd7f-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="ccd7f-133">label</span></span>|<span data-ttu-id="ccd7f-134">String</span><span class="sxs-lookup"><span data-stu-id="ccd7f-134">String</span></span>|<span data-ttu-id="ccd7f-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="ccd7f-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="ccd7f-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="ccd7f-136">The default value is empty.</span></span> <span data-ttu-id="ccd7f-137">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ccd7f-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ccd7f-138">id</span><span class="sxs-lookup"><span data-stu-id="ccd7f-138">id</span></span>|<span data-ttu-id="ccd7f-139">String</span><span class="sxs-lookup"><span data-stu-id="ccd7f-139">String</span></span>|<span data-ttu-id="ccd7f-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ccd7f-140">Key of the entity.</span></span> <span data-ttu-id="ccd7f-141">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ccd7f-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ccd7f-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ccd7f-142">lastModifiedDateTime</span></span>|<span data-ttu-id="ccd7f-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccd7f-143">DateTimeOffset</span></span>|<span data-ttu-id="ccd7f-144">A data e hora que a entidade foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ccd7f-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="ccd7f-145">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ccd7f-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ccd7f-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="ccd7f-146">defaultValue</span></span>|<span data-ttu-id="ccd7f-147">String</span><span class="sxs-lookup"><span data-stu-id="ccd7f-147">String</span></span>|<span data-ttu-id="ccd7f-148">Cadeia de caracteres localizadas padrão exibida na caixa de combinação.</span><span class="sxs-lookup"><span data-stu-id="ccd7f-148">Localized default string displayed in the combo box.</span></span> <span data-ttu-id="ccd7f-149">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="ccd7f-149">The default value is empty.</span></span>|
|<span data-ttu-id="ccd7f-150">sugestões</span><span class="sxs-lookup"><span data-stu-id="ccd7f-150">suggestions</span></span>|<span data-ttu-id="ccd7f-151">String collection</span><span class="sxs-lookup"><span data-stu-id="ccd7f-151">String collection</span></span>|<span data-ttu-id="ccd7f-152">Cadeias de caracteres localizadas listadas na lista suspensa da caixa de combinação.</span><span class="sxs-lookup"><span data-stu-id="ccd7f-152">Localized strings listed in the drop-down list of the combo box.</span></span> <span data-ttu-id="ccd7f-153">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="ccd7f-153">The default value is empty.</span></span>|
|<span data-ttu-id="ccd7f-154">obrigatório</span><span class="sxs-lookup"><span data-stu-id="ccd7f-154">required</span></span>|<span data-ttu-id="ccd7f-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccd7f-155">Boolean</span></span>|<span data-ttu-id="ccd7f-156">Especifica se deve ser especificado um valor para o parâmetro.</span><span class="sxs-lookup"><span data-stu-id="ccd7f-156">Specifies whether a value must be specified for the parameter.</span></span> <span data-ttu-id="ccd7f-157">O valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="ccd7f-157">The default value is false.</span></span>|
|<span data-ttu-id="ccd7f-158">maxLength</span><span class="sxs-lookup"><span data-stu-id="ccd7f-158">maxLength</span></span>|<span data-ttu-id="ccd7f-159">Int64</span><span class="sxs-lookup"><span data-stu-id="ccd7f-159">Int64</span></span>|<span data-ttu-id="ccd7f-160">Um inteiro não assinado que especifica o número máximo de caracteres de texto para o parâmetro.</span><span class="sxs-lookup"><span data-stu-id="ccd7f-160">An unsigned integer that specifies the maximum number of text characters for the parameter.</span></span> <span data-ttu-id="ccd7f-161">O valor padrão é 1023.</span><span class="sxs-lookup"><span data-stu-id="ccd7f-161">The default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="ccd7f-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccd7f-162">Response</span></span>
<span data-ttu-id="ccd7f-163">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ccd7f-163">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccd7f-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ccd7f-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="ccd7f-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ccd7f-165">Request</span></span>
<span data-ttu-id="ccd7f-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ccd7f-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ccd7f-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccd7f-167">Response</span></span>
<span data-ttu-id="ccd7f-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ccd7f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




