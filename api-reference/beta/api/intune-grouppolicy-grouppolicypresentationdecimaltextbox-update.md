---
title: Atualizar groupPolicyPresentationDecimalTextBox
description: Atualiza as propriedades de um objeto groupPolicyPresentationDecimalTextBox.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 622d75e58a131d2875d40894bfae00c5df9db75f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785619"
---
# <a name="update-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="1294f-103">Atualizar groupPolicyPresentationDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="1294f-103">Update groupPolicyPresentationDecimalTextBox</span></span>

> <span data-ttu-id="1294f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1294f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1294f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1294f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1294f-106">Atualiza as propriedades de um objeto [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="1294f-106">Update the properties of a [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1294f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1294f-107">Prerequisites</span></span>
<span data-ttu-id="1294f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1294f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1294f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1294f-110">Permission type</span></span>|<span data-ttu-id="1294f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1294f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1294f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1294f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1294f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1294f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1294f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1294f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1294f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1294f-115">Not supported.</span></span>|
|<span data-ttu-id="1294f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1294f-116">Application</span></span>|<span data-ttu-id="1294f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1294f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1294f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1294f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="1294f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1294f-119">Request headers</span></span>
|<span data-ttu-id="1294f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1294f-120">Header</span></span>|<span data-ttu-id="1294f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1294f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1294f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1294f-122">Authorization</span></span>|<span data-ttu-id="1294f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1294f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1294f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1294f-124">Accept</span></span>|<span data-ttu-id="1294f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1294f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1294f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1294f-126">Request body</span></span>
<span data-ttu-id="1294f-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="1294f-127">In the request body, supply a JSON representation for the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

<span data-ttu-id="1294f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md).</span><span class="sxs-lookup"><span data-stu-id="1294f-128">The following table shows the properties that are required when you create the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md).</span></span>

|<span data-ttu-id="1294f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1294f-129">Property</span></span>|<span data-ttu-id="1294f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1294f-130">Type</span></span>|<span data-ttu-id="1294f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1294f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1294f-132">rótulo</span><span class="sxs-lookup"><span data-stu-id="1294f-132">label</span></span>|<span data-ttu-id="1294f-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1294f-133">String</span></span>|<span data-ttu-id="1294f-134">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="1294f-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="1294f-135">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="1294f-135">The default value is empty.</span></span> <span data-ttu-id="1294f-136">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="1294f-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="1294f-137">id</span><span class="sxs-lookup"><span data-stu-id="1294f-137">id</span></span>|<span data-ttu-id="1294f-138">String</span><span class="sxs-lookup"><span data-stu-id="1294f-138">String</span></span>|<span data-ttu-id="1294f-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1294f-139">Key of the entity.</span></span> <span data-ttu-id="1294f-140">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="1294f-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="1294f-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1294f-141">lastModifiedDateTime</span></span>|<span data-ttu-id="1294f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1294f-142">DateTimeOffset</span></span>|<span data-ttu-id="1294f-143">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="1294f-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="1294f-144">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="1294f-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="1294f-145">defaultValue</span><span class="sxs-lookup"><span data-stu-id="1294f-145">defaultValue</span></span>|<span data-ttu-id="1294f-146">Int64</span><span class="sxs-lookup"><span data-stu-id="1294f-146">Int64</span></span>|<span data-ttu-id="1294f-147">Um inteiro sem sinal que especifica o valor inicial da caixa de texto decimal.</span><span class="sxs-lookup"><span data-stu-id="1294f-147">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="1294f-148">O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="1294f-148">The default value is 1.</span></span>|
|<span data-ttu-id="1294f-149">rotação</span><span class="sxs-lookup"><span data-stu-id="1294f-149">spin</span></span>|<span data-ttu-id="1294f-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="1294f-150">Boolean</span></span>|<span data-ttu-id="1294f-151">Se true, crie um controle de rotação; caso contrário, crie uma caixa de texto para entrada numérica.</span><span class="sxs-lookup"><span data-stu-id="1294f-151">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="1294f-152">O valor padrão é true.</span><span class="sxs-lookup"><span data-stu-id="1294f-152">The default value is true.</span></span>|
|<span data-ttu-id="1294f-153">spinStep</span><span class="sxs-lookup"><span data-stu-id="1294f-153">spinStep</span></span>|<span data-ttu-id="1294f-154">Int64</span><span class="sxs-lookup"><span data-stu-id="1294f-154">Int64</span></span>|<span data-ttu-id="1294f-155">Um inteiro sem sinal que especifica o incremento de alteração para o controle de rotação.</span><span class="sxs-lookup"><span data-stu-id="1294f-155">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="1294f-156">O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="1294f-156">The default value is 1.</span></span>|
|<span data-ttu-id="1294f-157">obrigatório</span><span class="sxs-lookup"><span data-stu-id="1294f-157">required</span></span>|<span data-ttu-id="1294f-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="1294f-158">Boolean</span></span>|<span data-ttu-id="1294f-159">Requisito para inserir um valor na caixa parâmetro.</span><span class="sxs-lookup"><span data-stu-id="1294f-159">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="1294f-160">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="1294f-160">The default value is false.</span></span>|
|<span data-ttu-id="1294f-161">MaxValue</span><span class="sxs-lookup"><span data-stu-id="1294f-161">minValue</span></span>|<span data-ttu-id="1294f-162">Int64</span><span class="sxs-lookup"><span data-stu-id="1294f-162">Int64</span></span>|<span data-ttu-id="1294f-163">Um inteiro sem sinal que especifica o valor mínimo permitido.</span><span class="sxs-lookup"><span data-stu-id="1294f-163">An unsigned integer that specifies the minimum allowed value.</span></span> <span data-ttu-id="1294f-164">O valor padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="1294f-164">The default value is 0.</span></span>|
|<span data-ttu-id="1294f-165">maxValue</span><span class="sxs-lookup"><span data-stu-id="1294f-165">maxValue</span></span>|<span data-ttu-id="1294f-166">Int64</span><span class="sxs-lookup"><span data-stu-id="1294f-166">Int64</span></span>|<span data-ttu-id="1294f-167">Um inteiro sem sinal que especifica o valor máximo permitido.</span><span class="sxs-lookup"><span data-stu-id="1294f-167">An unsigned integer that specifies the maximum allowed value.</span></span> <span data-ttu-id="1294f-168">O valor padrão é 9999.</span><span class="sxs-lookup"><span data-stu-id="1294f-168">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="1294f-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="1294f-169">Response</span></span>
<span data-ttu-id="1294f-170">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1294f-170">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1294f-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1294f-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="1294f-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1294f-172">Request</span></span>
<span data-ttu-id="1294f-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1294f-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1294f-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="1294f-174">Response</span></span>
<span data-ttu-id="1294f-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1294f-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





