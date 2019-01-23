---
title: Atualizar groupPolicyPresentationDecimalTextBox
description: Atualize as propriedades de um objeto groupPolicyPresentationDecimalTextBox.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c4f91abc80fe37fe3f3677afc7d06b547df9bee4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429022"
---
# <a name="update-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="90498-103">Atualizar groupPolicyPresentationDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="90498-103">Update groupPolicyPresentationDecimalTextBox</span></span>

> <span data-ttu-id="90498-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="90498-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="90498-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="90498-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="90498-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="90498-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90498-107">Atualize as propriedades de um objeto [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="90498-107">Update the properties of a [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90498-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="90498-108">Prerequisites</span></span>
<span data-ttu-id="90498-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="90498-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="90498-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90498-111">Permission type</span></span>|<span data-ttu-id="90498-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="90498-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90498-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90498-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90498-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90498-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="90498-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90498-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90498-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90498-116">Not supported.</span></span>|
|<span data-ttu-id="90498-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90498-117">Application</span></span>|<span data-ttu-id="90498-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90498-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90498-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90498-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="90498-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90498-120">Request headers</span></span>
|<span data-ttu-id="90498-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="90498-121">Header</span></span>|<span data-ttu-id="90498-122">Valor</span><span class="sxs-lookup"><span data-stu-id="90498-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90498-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="90498-123">Authorization</span></span>|<span data-ttu-id="90498-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90498-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90498-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="90498-125">Accept</span></span>|<span data-ttu-id="90498-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90498-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90498-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90498-127">Request body</span></span>
<span data-ttu-id="90498-128">No corpo da solicitação, fornece uma representação JSON para o objeto [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="90498-128">In the request body, supply a JSON representation for the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

<span data-ttu-id="90498-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md).</span><span class="sxs-lookup"><span data-stu-id="90498-129">The following table shows the properties that are required when you create the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md).</span></span>

|<span data-ttu-id="90498-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90498-130">Property</span></span>|<span data-ttu-id="90498-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="90498-131">Type</span></span>|<span data-ttu-id="90498-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="90498-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90498-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="90498-133">label</span></span>|<span data-ttu-id="90498-134">String</span><span class="sxs-lookup"><span data-stu-id="90498-134">String</span></span>|<span data-ttu-id="90498-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="90498-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="90498-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="90498-136">The default value is empty.</span></span> <span data-ttu-id="90498-137">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="90498-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="90498-138">id</span><span class="sxs-lookup"><span data-stu-id="90498-138">id</span></span>|<span data-ttu-id="90498-139">String</span><span class="sxs-lookup"><span data-stu-id="90498-139">String</span></span>|<span data-ttu-id="90498-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="90498-140">Key of the entity.</span></span> <span data-ttu-id="90498-141">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="90498-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="90498-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="90498-142">lastModifiedDateTime</span></span>|<span data-ttu-id="90498-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90498-143">DateTimeOffset</span></span>|<span data-ttu-id="90498-144">A data e hora que a entidade foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="90498-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="90498-145">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="90498-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="90498-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="90498-146">defaultValue</span></span>|<span data-ttu-id="90498-147">Int64</span><span class="sxs-lookup"><span data-stu-id="90498-147">Int64</span></span>|<span data-ttu-id="90498-148">Um inteiro não assinado que especifica o valor inicial da caixa de texto decimal.</span><span class="sxs-lookup"><span data-stu-id="90498-148">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="90498-149">O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="90498-149">The default value is 1.</span></span>|
|<span data-ttu-id="90498-150">rotação</span><span class="sxs-lookup"><span data-stu-id="90498-150">spin</span></span>|<span data-ttu-id="90498-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="90498-151">Boolean</span></span>|<span data-ttu-id="90498-152">Se for true, crie um controle de rotação; Caso contrário, crie uma caixa de texto para entrada numérica.</span><span class="sxs-lookup"><span data-stu-id="90498-152">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="90498-153">O valor padrão é true.</span><span class="sxs-lookup"><span data-stu-id="90498-153">The default value is true.</span></span>|
|<span data-ttu-id="90498-154">spinStep</span><span class="sxs-lookup"><span data-stu-id="90498-154">spinStep</span></span>|<span data-ttu-id="90498-155">Int64</span><span class="sxs-lookup"><span data-stu-id="90498-155">Int64</span></span>|<span data-ttu-id="90498-156">Um inteiro não assinado que especifica o incremento de alteração para o controle de rotação.</span><span class="sxs-lookup"><span data-stu-id="90498-156">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="90498-157">O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="90498-157">The default value is 1.</span></span>|
|<span data-ttu-id="90498-158">obrigatório</span><span class="sxs-lookup"><span data-stu-id="90498-158">required</span></span>|<span data-ttu-id="90498-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="90498-159">Boolean</span></span>|<span data-ttu-id="90498-160">Requisito para inserir um valor na caixa de parâmetro.</span><span class="sxs-lookup"><span data-stu-id="90498-160">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="90498-161">O valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="90498-161">The default value is false.</span></span>|
|<span data-ttu-id="90498-162">minValue</span><span class="sxs-lookup"><span data-stu-id="90498-162">minValue</span></span>|<span data-ttu-id="90498-163">Int64</span><span class="sxs-lookup"><span data-stu-id="90498-163">Int64</span></span>|<span data-ttu-id="90498-164">Um inteiro não assinado que especifica o valor mínimo permitido.</span><span class="sxs-lookup"><span data-stu-id="90498-164">An unsigned integer that specifies the minimum allowed value.</span></span> <span data-ttu-id="90498-165">O valor padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="90498-165">The default value is 0.</span></span>|
|<span data-ttu-id="90498-166">maxValue</span><span class="sxs-lookup"><span data-stu-id="90498-166">maxValue</span></span>|<span data-ttu-id="90498-167">Int64</span><span class="sxs-lookup"><span data-stu-id="90498-167">Int64</span></span>|<span data-ttu-id="90498-168">Um inteiro não assinado que especifica o valor máximo permitido.</span><span class="sxs-lookup"><span data-stu-id="90498-168">An unsigned integer that specifies the maximum allowed value.</span></span> <span data-ttu-id="90498-169">O valor padrão é 9999.</span><span class="sxs-lookup"><span data-stu-id="90498-169">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="90498-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="90498-170">Response</span></span>
<span data-ttu-id="90498-171">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90498-171">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90498-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90498-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="90498-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90498-173">Request</span></span>
<span data-ttu-id="90498-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90498-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="90498-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="90498-175">Response</span></span>
<span data-ttu-id="90498-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90498-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




