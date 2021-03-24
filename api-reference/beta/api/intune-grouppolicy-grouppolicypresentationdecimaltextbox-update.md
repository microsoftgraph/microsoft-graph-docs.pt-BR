---
title: Atualizar groupPolicyPresentationDecimalTextBox
description: Atualize as propriedades de um objeto groupPolicyPresentationDecimalTextBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0bc44a9a058951e2525b2f9b6c43f3fe990d2694
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149643"
---
# <a name="update-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="f8f7f-103">Atualizar groupPolicyPresentationDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="f8f7f-103">Update groupPolicyPresentationDecimalTextBox</span></span>

<span data-ttu-id="f8f7f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8f7f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8f7f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f8f7f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8f7f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f8f7f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8f7f-107">Atualize as propriedades de [um objeto groupPolicyPresentationDecimalTextBox.](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)</span><span class="sxs-lookup"><span data-stu-id="f8f7f-107">Update the properties of a [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8f7f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f8f7f-108">Prerequisites</span></span>
<span data-ttu-id="f8f7f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8f7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8f7f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8f7f-111">Permission type</span></span>|<span data-ttu-id="f8f7f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f8f7f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8f7f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8f7f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8f7f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8f7f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f8f7f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8f7f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8f7f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8f7f-116">Not supported.</span></span>|
|<span data-ttu-id="f8f7f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8f7f-117">Application</span></span>|<span data-ttu-id="f8f7f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8f7f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8f7f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8f7f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="f8f7f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8f7f-120">Request headers</span></span>
|<span data-ttu-id="f8f7f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f8f7f-121">Header</span></span>|<span data-ttu-id="f8f7f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f8f7f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8f7f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8f7f-123">Authorization</span></span>|<span data-ttu-id="f8f7f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8f7f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8f7f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f8f7f-125">Accept</span></span>|<span data-ttu-id="f8f7f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8f7f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8f7f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8f7f-127">Request body</span></span>
<span data-ttu-id="f8f7f-128">No corpo da solicitação, fornece uma representação JSON para o [objeto groupPolicyPresentationDecimalTextBox.](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)</span><span class="sxs-lookup"><span data-stu-id="f8f7f-128">In the request body, supply a JSON representation for the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

<span data-ttu-id="f8f7f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md).</span><span class="sxs-lookup"><span data-stu-id="f8f7f-129">The following table shows the properties that are required when you create the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md).</span></span>

|<span data-ttu-id="f8f7f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8f7f-130">Property</span></span>|<span data-ttu-id="f8f7f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8f7f-131">Type</span></span>|<span data-ttu-id="f8f7f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8f7f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8f7f-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="f8f7f-133">label</span></span>|<span data-ttu-id="f8f7f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8f7f-134">String</span></span>|<span data-ttu-id="f8f7f-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="f8f7f-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="f8f7f-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="f8f7f-136">The default value is empty.</span></span> <span data-ttu-id="f8f7f-137">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="f8f7f-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="f8f7f-138">id</span><span class="sxs-lookup"><span data-stu-id="f8f7f-138">id</span></span>|<span data-ttu-id="f8f7f-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8f7f-139">String</span></span>|<span data-ttu-id="f8f7f-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f8f7f-140">Key of the entity.</span></span> <span data-ttu-id="f8f7f-141">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="f8f7f-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="f8f7f-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f8f7f-142">lastModifiedDateTime</span></span>|<span data-ttu-id="f8f7f-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8f7f-143">DateTimeOffset</span></span>|<span data-ttu-id="f8f7f-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f8f7f-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="f8f7f-145">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="f8f7f-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="f8f7f-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="f8f7f-146">defaultValue</span></span>|<span data-ttu-id="f8f7f-147">Int64</span><span class="sxs-lookup"><span data-stu-id="f8f7f-147">Int64</span></span>|<span data-ttu-id="f8f7f-148">Um inteiro não assinado que especifica o valor inicial da caixa de texto decimal.</span><span class="sxs-lookup"><span data-stu-id="f8f7f-148">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="f8f7f-149">O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="f8f7f-149">The default value is 1.</span></span>|
|<span data-ttu-id="f8f7f-150">spin</span><span class="sxs-lookup"><span data-stu-id="f8f7f-150">spin</span></span>|<span data-ttu-id="f8f7f-151">Booleano</span><span class="sxs-lookup"><span data-stu-id="f8f7f-151">Boolean</span></span>|<span data-ttu-id="f8f7f-152">Se for true, crie um controle de rotação; caso contrário, crie uma caixa de texto para entrada numérica.</span><span class="sxs-lookup"><span data-stu-id="f8f7f-152">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="f8f7f-153">O valor padrão é true.</span><span class="sxs-lookup"><span data-stu-id="f8f7f-153">The default value is true.</span></span>|
|<span data-ttu-id="f8f7f-154">spinStep</span><span class="sxs-lookup"><span data-stu-id="f8f7f-154">spinStep</span></span>|<span data-ttu-id="f8f7f-155">Int64</span><span class="sxs-lookup"><span data-stu-id="f8f7f-155">Int64</span></span>|<span data-ttu-id="f8f7f-156">Um inteiro não assinado que especifica o incremento de alteração para o controle de rotação.</span><span class="sxs-lookup"><span data-stu-id="f8f7f-156">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="f8f7f-157">O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="f8f7f-157">The default value is 1.</span></span>|
|<span data-ttu-id="f8f7f-158">obrigatório</span><span class="sxs-lookup"><span data-stu-id="f8f7f-158">required</span></span>|<span data-ttu-id="f8f7f-159">Booleano</span><span class="sxs-lookup"><span data-stu-id="f8f7f-159">Boolean</span></span>|<span data-ttu-id="f8f7f-160">Requisito para inserir um valor na caixa de parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f8f7f-160">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="f8f7f-161">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="f8f7f-161">The default value is false.</span></span>|
|<span data-ttu-id="f8f7f-162">minValue</span><span class="sxs-lookup"><span data-stu-id="f8f7f-162">minValue</span></span>|<span data-ttu-id="f8f7f-163">Int64</span><span class="sxs-lookup"><span data-stu-id="f8f7f-163">Int64</span></span>|<span data-ttu-id="f8f7f-164">Um inteiro não assinado que especifica o valor mínimo permitido.</span><span class="sxs-lookup"><span data-stu-id="f8f7f-164">An unsigned integer that specifies the minimum allowed value.</span></span> <span data-ttu-id="f8f7f-165">O valor padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="f8f7f-165">The default value is 0.</span></span>|
|<span data-ttu-id="f8f7f-166">maxValue</span><span class="sxs-lookup"><span data-stu-id="f8f7f-166">maxValue</span></span>|<span data-ttu-id="f8f7f-167">Int64</span><span class="sxs-lookup"><span data-stu-id="f8f7f-167">Int64</span></span>|<span data-ttu-id="f8f7f-168">Um inteiro não assinado que especifica o valor máximo permitido.</span><span class="sxs-lookup"><span data-stu-id="f8f7f-168">An unsigned integer that specifies the maximum allowed value.</span></span> <span data-ttu-id="f8f7f-169">O valor padrão é 9999.</span><span class="sxs-lookup"><span data-stu-id="f8f7f-169">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="f8f7f-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8f7f-170">Response</span></span>
<span data-ttu-id="f8f7f-171">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8f7f-171">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8f7f-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8f7f-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8f7f-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8f7f-173">Request</span></span>
<span data-ttu-id="f8f7f-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8f7f-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 221

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
  "label": "Label value",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```

### <a name="response"></a><span data-ttu-id="f8f7f-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8f7f-175">Response</span></span>
<span data-ttu-id="f8f7f-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8f7f-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 334

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
  "label": "Label value",
  "id": "988daea7-aea7-988d-a7ae-8d98a7ae8d98",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```




