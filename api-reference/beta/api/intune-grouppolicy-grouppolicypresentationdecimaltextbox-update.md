---
title: Atualizar groupPolicyPresentationDecimalTextBox
description: Atualiza as propriedades de um objeto groupPolicyPresentationDecimalTextBox.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fedddbc3e5e6bd19f27d5023ea8c8704b6bcb000
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804258"
---
# <a name="update-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="5b067-103">Atualizar groupPolicyPresentationDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="5b067-103">Update groupPolicyPresentationDecimalTextBox</span></span>

> <span data-ttu-id="5b067-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5b067-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b067-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5b067-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b067-106">Atualiza as propriedades de um objeto [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="5b067-106">Update the properties of a [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b067-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5b067-107">Prerequisites</span></span>
<span data-ttu-id="5b067-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b067-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b067-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b067-110">Permission type</span></span>|<span data-ttu-id="5b067-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5b067-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b067-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b067-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5b067-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b067-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5b067-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b067-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b067-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b067-115">Not supported.</span></span>|
|<span data-ttu-id="5b067-116">Application</span><span class="sxs-lookup"><span data-stu-id="5b067-116">Application</span></span>|<span data-ttu-id="5b067-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b067-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b067-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b067-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="5b067-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b067-119">Request headers</span></span>
|<span data-ttu-id="5b067-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5b067-120">Header</span></span>|<span data-ttu-id="5b067-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5b067-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b067-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b067-122">Authorization</span></span>|<span data-ttu-id="5b067-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b067-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b067-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5b067-124">Accept</span></span>|<span data-ttu-id="5b067-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5b067-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b067-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b067-126">Request body</span></span>
<span data-ttu-id="5b067-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="5b067-127">In the request body, supply a JSON representation for the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

<span data-ttu-id="5b067-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md).</span><span class="sxs-lookup"><span data-stu-id="5b067-128">The following table shows the properties that are required when you create the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md).</span></span>

|<span data-ttu-id="5b067-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b067-129">Property</span></span>|<span data-ttu-id="5b067-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b067-130">Type</span></span>|<span data-ttu-id="5b067-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b067-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b067-132">rótulo</span><span class="sxs-lookup"><span data-stu-id="5b067-132">label</span></span>|<span data-ttu-id="5b067-133">String</span><span class="sxs-lookup"><span data-stu-id="5b067-133">String</span></span>|<span data-ttu-id="5b067-134">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="5b067-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="5b067-135">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="5b067-135">The default value is empty.</span></span> <span data-ttu-id="5b067-136">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="5b067-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="5b067-137">id</span><span class="sxs-lookup"><span data-stu-id="5b067-137">id</span></span>|<span data-ttu-id="5b067-138">String</span><span class="sxs-lookup"><span data-stu-id="5b067-138">String</span></span>|<span data-ttu-id="5b067-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5b067-139">Key of the entity.</span></span> <span data-ttu-id="5b067-140">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="5b067-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="5b067-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5b067-141">lastModifiedDateTime</span></span>|<span data-ttu-id="5b067-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b067-142">DateTimeOffset</span></span>|<span data-ttu-id="5b067-143">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="5b067-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="5b067-144">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="5b067-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="5b067-145">defaultValue</span><span class="sxs-lookup"><span data-stu-id="5b067-145">defaultValue</span></span>|<span data-ttu-id="5b067-146">Int64</span><span class="sxs-lookup"><span data-stu-id="5b067-146">Int64</span></span>|<span data-ttu-id="5b067-147">Um inteiro sem sinal que especifica o valor inicial da caixa de texto decimal.</span><span class="sxs-lookup"><span data-stu-id="5b067-147">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="5b067-148">O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="5b067-148">The default value is 1.</span></span>|
|<span data-ttu-id="5b067-149">rotação</span><span class="sxs-lookup"><span data-stu-id="5b067-149">spin</span></span>|<span data-ttu-id="5b067-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b067-150">Boolean</span></span>|<span data-ttu-id="5b067-151">Se true, crie um controle de rotação; caso contrário, crie uma caixa de texto para entrada numérica.</span><span class="sxs-lookup"><span data-stu-id="5b067-151">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="5b067-152">O valor padrão é true.</span><span class="sxs-lookup"><span data-stu-id="5b067-152">The default value is true.</span></span>|
|<span data-ttu-id="5b067-153">spinStep</span><span class="sxs-lookup"><span data-stu-id="5b067-153">spinStep</span></span>|<span data-ttu-id="5b067-154">Int64</span><span class="sxs-lookup"><span data-stu-id="5b067-154">Int64</span></span>|<span data-ttu-id="5b067-155">Um inteiro sem sinal que especifica o incremento de alteração para o controle de rotação.</span><span class="sxs-lookup"><span data-stu-id="5b067-155">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="5b067-156">O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="5b067-156">The default value is 1.</span></span>|
|<span data-ttu-id="5b067-157">obrigatório</span><span class="sxs-lookup"><span data-stu-id="5b067-157">required</span></span>|<span data-ttu-id="5b067-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b067-158">Boolean</span></span>|<span data-ttu-id="5b067-159">Requisito para inserir um valor na caixa parâmetro.</span><span class="sxs-lookup"><span data-stu-id="5b067-159">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="5b067-160">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="5b067-160">The default value is false.</span></span>|
|<span data-ttu-id="5b067-161">MaxValue</span><span class="sxs-lookup"><span data-stu-id="5b067-161">minValue</span></span>|<span data-ttu-id="5b067-162">Int64</span><span class="sxs-lookup"><span data-stu-id="5b067-162">Int64</span></span>|<span data-ttu-id="5b067-163">Um inteiro sem sinal que especifica o valor mínimo permitido.</span><span class="sxs-lookup"><span data-stu-id="5b067-163">An unsigned integer that specifies the minimum allowed value.</span></span> <span data-ttu-id="5b067-164">O valor padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="5b067-164">The default value is 0.</span></span>|
|<span data-ttu-id="5b067-165">maxValue</span><span class="sxs-lookup"><span data-stu-id="5b067-165">maxValue</span></span>|<span data-ttu-id="5b067-166">Int64</span><span class="sxs-lookup"><span data-stu-id="5b067-166">Int64</span></span>|<span data-ttu-id="5b067-167">Um inteiro sem sinal que especifica o valor máximo permitido.</span><span class="sxs-lookup"><span data-stu-id="5b067-167">An unsigned integer that specifies the maximum allowed value.</span></span> <span data-ttu-id="5b067-168">O valor padrão é 9999.</span><span class="sxs-lookup"><span data-stu-id="5b067-168">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="5b067-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b067-169">Response</span></span>
<span data-ttu-id="5b067-170">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b067-170">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b067-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b067-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b067-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b067-172">Request</span></span>
<span data-ttu-id="5b067-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b067-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5b067-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b067-174">Response</span></span>
<span data-ttu-id="5b067-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b067-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




