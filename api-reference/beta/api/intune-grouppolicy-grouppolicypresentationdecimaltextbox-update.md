---
title: Atualizar groupPolicyPresentationDecimalTextBox
description: Atualiza as propriedades de um objeto groupPolicyPresentationDecimalTextBox.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dc68b15443bbc59ee0d3b5f2d55024988425dfd4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43424414"
---
# <a name="update-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="b5cdc-103">Atualizar groupPolicyPresentationDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="b5cdc-103">Update groupPolicyPresentationDecimalTextBox</span></span>

<span data-ttu-id="b5cdc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5cdc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5cdc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b5cdc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5cdc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b5cdc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5cdc-107">Atualiza as propriedades de um objeto [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="b5cdc-107">Update the properties of a [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5cdc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b5cdc-108">Prerequisites</span></span>
<span data-ttu-id="b5cdc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5cdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5cdc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5cdc-111">Permission type</span></span>|<span data-ttu-id="b5cdc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b5cdc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5cdc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5cdc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b5cdc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5cdc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b5cdc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5cdc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5cdc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5cdc-116">Not supported.</span></span>|
|<span data-ttu-id="b5cdc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5cdc-117">Application</span></span>|<span data-ttu-id="b5cdc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5cdc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5cdc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5cdc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="b5cdc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5cdc-120">Request headers</span></span>
|<span data-ttu-id="b5cdc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b5cdc-121">Header</span></span>|<span data-ttu-id="b5cdc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b5cdc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5cdc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5cdc-123">Authorization</span></span>|<span data-ttu-id="b5cdc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5cdc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5cdc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b5cdc-125">Accept</span></span>|<span data-ttu-id="b5cdc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b5cdc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5cdc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5cdc-127">Request body</span></span>
<span data-ttu-id="b5cdc-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="b5cdc-128">In the request body, supply a JSON representation for the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

<span data-ttu-id="b5cdc-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md).</span><span class="sxs-lookup"><span data-stu-id="b5cdc-129">The following table shows the properties that are required when you create the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md).</span></span>

|<span data-ttu-id="b5cdc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5cdc-130">Property</span></span>|<span data-ttu-id="b5cdc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5cdc-131">Type</span></span>|<span data-ttu-id="b5cdc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5cdc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5cdc-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="b5cdc-133">label</span></span>|<span data-ttu-id="b5cdc-134">String</span><span class="sxs-lookup"><span data-stu-id="b5cdc-134">String</span></span>|<span data-ttu-id="b5cdc-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="b5cdc-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="b5cdc-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="b5cdc-136">The default value is empty.</span></span> <span data-ttu-id="b5cdc-137">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="b5cdc-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="b5cdc-138">id</span><span class="sxs-lookup"><span data-stu-id="b5cdc-138">id</span></span>|<span data-ttu-id="b5cdc-139">String</span><span class="sxs-lookup"><span data-stu-id="b5cdc-139">String</span></span>|<span data-ttu-id="b5cdc-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b5cdc-140">Key of the entity.</span></span> <span data-ttu-id="b5cdc-141">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="b5cdc-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="b5cdc-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5cdc-142">lastModifiedDateTime</span></span>|<span data-ttu-id="b5cdc-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5cdc-143">DateTimeOffset</span></span>|<span data-ttu-id="b5cdc-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b5cdc-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="b5cdc-145">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="b5cdc-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="b5cdc-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="b5cdc-146">defaultValue</span></span>|<span data-ttu-id="b5cdc-147">Int64</span><span class="sxs-lookup"><span data-stu-id="b5cdc-147">Int64</span></span>|<span data-ttu-id="b5cdc-148">Um inteiro sem sinal que especifica o valor inicial da caixa de texto decimal.</span><span class="sxs-lookup"><span data-stu-id="b5cdc-148">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="b5cdc-149">O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="b5cdc-149">The default value is 1.</span></span>|
|<span data-ttu-id="b5cdc-150">rotação</span><span class="sxs-lookup"><span data-stu-id="b5cdc-150">spin</span></span>|<span data-ttu-id="b5cdc-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5cdc-151">Boolean</span></span>|<span data-ttu-id="b5cdc-152">Se true, crie um controle de rotação; caso contrário, crie uma caixa de texto para entrada numérica.</span><span class="sxs-lookup"><span data-stu-id="b5cdc-152">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="b5cdc-153">O valor padrão é true.</span><span class="sxs-lookup"><span data-stu-id="b5cdc-153">The default value is true.</span></span>|
|<span data-ttu-id="b5cdc-154">spinStep</span><span class="sxs-lookup"><span data-stu-id="b5cdc-154">spinStep</span></span>|<span data-ttu-id="b5cdc-155">Int64</span><span class="sxs-lookup"><span data-stu-id="b5cdc-155">Int64</span></span>|<span data-ttu-id="b5cdc-156">Um inteiro sem sinal que especifica o incremento de alteração para o controle de rotação.</span><span class="sxs-lookup"><span data-stu-id="b5cdc-156">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="b5cdc-157">O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="b5cdc-157">The default value is 1.</span></span>|
|<span data-ttu-id="b5cdc-158">obrigatório</span><span class="sxs-lookup"><span data-stu-id="b5cdc-158">required</span></span>|<span data-ttu-id="b5cdc-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5cdc-159">Boolean</span></span>|<span data-ttu-id="b5cdc-160">Requisito para inserir um valor na caixa parâmetro.</span><span class="sxs-lookup"><span data-stu-id="b5cdc-160">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="b5cdc-161">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="b5cdc-161">The default value is false.</span></span>|
|<span data-ttu-id="b5cdc-162">MaxValue</span><span class="sxs-lookup"><span data-stu-id="b5cdc-162">minValue</span></span>|<span data-ttu-id="b5cdc-163">Int64</span><span class="sxs-lookup"><span data-stu-id="b5cdc-163">Int64</span></span>|<span data-ttu-id="b5cdc-164">Um inteiro sem sinal que especifica o valor mínimo permitido.</span><span class="sxs-lookup"><span data-stu-id="b5cdc-164">An unsigned integer that specifies the minimum allowed value.</span></span> <span data-ttu-id="b5cdc-165">O valor padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="b5cdc-165">The default value is 0.</span></span>|
|<span data-ttu-id="b5cdc-166">maxValue</span><span class="sxs-lookup"><span data-stu-id="b5cdc-166">maxValue</span></span>|<span data-ttu-id="b5cdc-167">Int64</span><span class="sxs-lookup"><span data-stu-id="b5cdc-167">Int64</span></span>|<span data-ttu-id="b5cdc-168">Um inteiro sem sinal que especifica o valor máximo permitido.</span><span class="sxs-lookup"><span data-stu-id="b5cdc-168">An unsigned integer that specifies the maximum allowed value.</span></span> <span data-ttu-id="b5cdc-169">O valor padrão é 9999.</span><span class="sxs-lookup"><span data-stu-id="b5cdc-169">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="b5cdc-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5cdc-170">Response</span></span>
<span data-ttu-id="b5cdc-171">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5cdc-171">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5cdc-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5cdc-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5cdc-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5cdc-173">Request</span></span>
<span data-ttu-id="b5cdc-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5cdc-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b5cdc-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5cdc-175">Response</span></span>
<span data-ttu-id="b5cdc-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b5cdc-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



