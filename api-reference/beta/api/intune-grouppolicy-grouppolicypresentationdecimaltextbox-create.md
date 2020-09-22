---
title: Criar groupPolicyPresentationDecimalTextBox
description: Criar um novo objeto groupPolicyPresentationDecimalTextBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9231a4387badafe48cde53fc5ec087222aa19c0b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078714"
---
# <a name="create-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="a27a8-103">Criar groupPolicyPresentationDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="a27a8-103">Create groupPolicyPresentationDecimalTextBox</span></span>

<span data-ttu-id="a27a8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a27a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a27a8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a27a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a27a8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a27a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a27a8-107">Criar um novo objeto [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="a27a8-107">Create a new [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a27a8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a27a8-108">Prerequisites</span></span>
<span data-ttu-id="a27a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a27a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a27a8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a27a8-111">Permission type</span></span>|<span data-ttu-id="a27a8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a27a8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a27a8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a27a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a27a8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a27a8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a27a8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a27a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a27a8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a27a8-116">Not supported.</span></span>|
|<span data-ttu-id="a27a8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a27a8-117">Application</span></span>|<span data-ttu-id="a27a8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a27a8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a27a8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a27a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="a27a8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a27a8-120">Request headers</span></span>
|<span data-ttu-id="a27a8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a27a8-121">Header</span></span>|<span data-ttu-id="a27a8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a27a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a27a8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a27a8-123">Authorization</span></span>|<span data-ttu-id="a27a8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a27a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a27a8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a27a8-125">Accept</span></span>|<span data-ttu-id="a27a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a27a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a27a8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a27a8-127">Request body</span></span>
<span data-ttu-id="a27a8-128">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyPresentationDecimalTextBox.</span><span class="sxs-lookup"><span data-stu-id="a27a8-128">In the request body, supply a JSON representation for the groupPolicyPresentationDecimalTextBox object.</span></span>

<span data-ttu-id="a27a8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyPresentationDecimalTextBox.</span><span class="sxs-lookup"><span data-stu-id="a27a8-129">The following table shows the properties that are required when you create the groupPolicyPresentationDecimalTextBox.</span></span>

|<span data-ttu-id="a27a8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a27a8-130">Property</span></span>|<span data-ttu-id="a27a8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a27a8-131">Type</span></span>|<span data-ttu-id="a27a8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a27a8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a27a8-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="a27a8-133">label</span></span>|<span data-ttu-id="a27a8-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a27a8-134">String</span></span>|<span data-ttu-id="a27a8-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="a27a8-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="a27a8-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="a27a8-136">The default value is empty.</span></span> <span data-ttu-id="a27a8-137">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="a27a8-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="a27a8-138">id</span><span class="sxs-lookup"><span data-stu-id="a27a8-138">id</span></span>|<span data-ttu-id="a27a8-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a27a8-139">String</span></span>|<span data-ttu-id="a27a8-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a27a8-140">Key of the entity.</span></span> <span data-ttu-id="a27a8-141">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="a27a8-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="a27a8-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a27a8-142">lastModifiedDateTime</span></span>|<span data-ttu-id="a27a8-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a27a8-143">DateTimeOffset</span></span>|<span data-ttu-id="a27a8-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="a27a8-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="a27a8-145">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="a27a8-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="a27a8-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="a27a8-146">defaultValue</span></span>|<span data-ttu-id="a27a8-147">Int64</span><span class="sxs-lookup"><span data-stu-id="a27a8-147">Int64</span></span>|<span data-ttu-id="a27a8-148">Um inteiro sem sinal que especifica o valor inicial da caixa de texto decimal.</span><span class="sxs-lookup"><span data-stu-id="a27a8-148">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="a27a8-149">O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="a27a8-149">The default value is 1.</span></span>|
|<span data-ttu-id="a27a8-150">rotação</span><span class="sxs-lookup"><span data-stu-id="a27a8-150">spin</span></span>|<span data-ttu-id="a27a8-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="a27a8-151">Boolean</span></span>|<span data-ttu-id="a27a8-152">Se true, crie um controle de rotação; caso contrário, crie uma caixa de texto para entrada numérica.</span><span class="sxs-lookup"><span data-stu-id="a27a8-152">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="a27a8-153">O valor padrão é true.</span><span class="sxs-lookup"><span data-stu-id="a27a8-153">The default value is true.</span></span>|
|<span data-ttu-id="a27a8-154">spinStep</span><span class="sxs-lookup"><span data-stu-id="a27a8-154">spinStep</span></span>|<span data-ttu-id="a27a8-155">Int64</span><span class="sxs-lookup"><span data-stu-id="a27a8-155">Int64</span></span>|<span data-ttu-id="a27a8-156">Um inteiro sem sinal que especifica o incremento de alteração para o controle de rotação.</span><span class="sxs-lookup"><span data-stu-id="a27a8-156">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="a27a8-157">O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="a27a8-157">The default value is 1.</span></span>|
|<span data-ttu-id="a27a8-158">obrigatório</span><span class="sxs-lookup"><span data-stu-id="a27a8-158">required</span></span>|<span data-ttu-id="a27a8-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="a27a8-159">Boolean</span></span>|<span data-ttu-id="a27a8-160">Requisito para inserir um valor na caixa parâmetro.</span><span class="sxs-lookup"><span data-stu-id="a27a8-160">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="a27a8-161">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="a27a8-161">The default value is false.</span></span>|
|<span data-ttu-id="a27a8-162">MaxValue</span><span class="sxs-lookup"><span data-stu-id="a27a8-162">minValue</span></span>|<span data-ttu-id="a27a8-163">Int64</span><span class="sxs-lookup"><span data-stu-id="a27a8-163">Int64</span></span>|<span data-ttu-id="a27a8-164">Um inteiro sem sinal que especifica o valor mínimo permitido.</span><span class="sxs-lookup"><span data-stu-id="a27a8-164">An unsigned integer that specifies the minimum allowed value.</span></span> <span data-ttu-id="a27a8-165">O valor padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="a27a8-165">The default value is 0.</span></span>|
|<span data-ttu-id="a27a8-166">maxValue</span><span class="sxs-lookup"><span data-stu-id="a27a8-166">maxValue</span></span>|<span data-ttu-id="a27a8-167">Int64</span><span class="sxs-lookup"><span data-stu-id="a27a8-167">Int64</span></span>|<span data-ttu-id="a27a8-168">Um inteiro sem sinal que especifica o valor máximo permitido.</span><span class="sxs-lookup"><span data-stu-id="a27a8-168">An unsigned integer that specifies the maximum allowed value.</span></span> <span data-ttu-id="a27a8-169">O valor padrão é 9999.</span><span class="sxs-lookup"><span data-stu-id="a27a8-169">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="a27a8-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="a27a8-170">Response</span></span>
<span data-ttu-id="a27a8-171">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a27a8-171">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a27a8-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a27a8-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="a27a8-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a27a8-173">Request</span></span>
<span data-ttu-id="a27a8-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a27a8-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
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

### <a name="response"></a><span data-ttu-id="a27a8-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="a27a8-175">Response</span></span>
<span data-ttu-id="a27a8-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a27a8-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






