---
title: Criar groupPolicyPresentationLongDecimalTextBox
description: Crie um novo objeto de groupPolicyPresentationLongDecimalTextBox.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d1fd47d422358dd0cd4a23ff35137654787498bf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429048"
---
# <a name="create-grouppolicypresentationlongdecimaltextbox"></a><span data-ttu-id="7919b-103">Criar groupPolicyPresentationLongDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="7919b-103">Create groupPolicyPresentationLongDecimalTextBox</span></span>

> <span data-ttu-id="7919b-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="7919b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7919b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7919b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7919b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="7919b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7919b-107">Crie um novo objeto de [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="7919b-107">Create a new [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7919b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7919b-108">Prerequisites</span></span>
<span data-ttu-id="7919b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7919b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7919b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7919b-111">Permission type</span></span>|<span data-ttu-id="7919b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7919b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7919b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7919b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7919b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7919b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7919b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7919b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7919b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7919b-116">Not supported.</span></span>|
|<span data-ttu-id="7919b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7919b-117">Application</span></span>|<span data-ttu-id="7919b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7919b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7919b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7919b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="7919b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7919b-120">Request headers</span></span>
|<span data-ttu-id="7919b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7919b-121">Header</span></span>|<span data-ttu-id="7919b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7919b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7919b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7919b-123">Authorization</span></span>|<span data-ttu-id="7919b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7919b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7919b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7919b-125">Accept</span></span>|<span data-ttu-id="7919b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7919b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7919b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7919b-127">Request body</span></span>
<span data-ttu-id="7919b-128">No corpo da solicitação, fornece uma representação JSON para o objeto groupPolicyPresentationLongDecimalTextBox.</span><span class="sxs-lookup"><span data-stu-id="7919b-128">In the request body, supply a JSON representation for the groupPolicyPresentationLongDecimalTextBox object.</span></span>

<span data-ttu-id="7919b-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o groupPolicyPresentationLongDecimalTextBox.</span><span class="sxs-lookup"><span data-stu-id="7919b-129">The following table shows the properties that are required when you create the groupPolicyPresentationLongDecimalTextBox.</span></span>

|<span data-ttu-id="7919b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7919b-130">Property</span></span>|<span data-ttu-id="7919b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7919b-131">Type</span></span>|<span data-ttu-id="7919b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7919b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7919b-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="7919b-133">label</span></span>|<span data-ttu-id="7919b-134">String</span><span class="sxs-lookup"><span data-stu-id="7919b-134">String</span></span>|<span data-ttu-id="7919b-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="7919b-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="7919b-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="7919b-136">The default value is empty.</span></span> <span data-ttu-id="7919b-137">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="7919b-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="7919b-138">id</span><span class="sxs-lookup"><span data-stu-id="7919b-138">id</span></span>|<span data-ttu-id="7919b-139">String</span><span class="sxs-lookup"><span data-stu-id="7919b-139">String</span></span>|<span data-ttu-id="7919b-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7919b-140">Key of the entity.</span></span> <span data-ttu-id="7919b-141">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="7919b-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="7919b-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7919b-142">lastModifiedDateTime</span></span>|<span data-ttu-id="7919b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7919b-143">DateTimeOffset</span></span>|<span data-ttu-id="7919b-144">A data e hora que a entidade foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="7919b-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="7919b-145">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="7919b-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="7919b-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="7919b-146">defaultValue</span></span>|<span data-ttu-id="7919b-147">Int64</span><span class="sxs-lookup"><span data-stu-id="7919b-147">Int64</span></span>|<span data-ttu-id="7919b-148">Um inteiro não assinado que especifica o valor inicial da caixa de texto decimal.</span><span class="sxs-lookup"><span data-stu-id="7919b-148">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="7919b-149">O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="7919b-149">The default value is 1.</span></span>|
|<span data-ttu-id="7919b-150">rotação</span><span class="sxs-lookup"><span data-stu-id="7919b-150">spin</span></span>|<span data-ttu-id="7919b-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="7919b-151">Boolean</span></span>|<span data-ttu-id="7919b-152">Se for true, crie um controle de rotação; Caso contrário, crie uma caixa de texto para entrada numérica.</span><span class="sxs-lookup"><span data-stu-id="7919b-152">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="7919b-153">O valor padrão é true.</span><span class="sxs-lookup"><span data-stu-id="7919b-153">The default value is true.</span></span>|
|<span data-ttu-id="7919b-154">spinStep</span><span class="sxs-lookup"><span data-stu-id="7919b-154">spinStep</span></span>|<span data-ttu-id="7919b-155">Int64</span><span class="sxs-lookup"><span data-stu-id="7919b-155">Int64</span></span>|<span data-ttu-id="7919b-156">Um inteiro não assinado que especifica o incremento de alteração para o controle de rotação.</span><span class="sxs-lookup"><span data-stu-id="7919b-156">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="7919b-157">O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="7919b-157">The default value is 1.</span></span>|
|<span data-ttu-id="7919b-158">obrigatório</span><span class="sxs-lookup"><span data-stu-id="7919b-158">required</span></span>|<span data-ttu-id="7919b-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="7919b-159">Boolean</span></span>|<span data-ttu-id="7919b-160">Requisito para inserir um valor na caixa de parâmetro.</span><span class="sxs-lookup"><span data-stu-id="7919b-160">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="7919b-161">O valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="7919b-161">The default value is false.</span></span>|
|<span data-ttu-id="7919b-162">minValue</span><span class="sxs-lookup"><span data-stu-id="7919b-162">minValue</span></span>|<span data-ttu-id="7919b-163">Int64</span><span class="sxs-lookup"><span data-stu-id="7919b-163">Int64</span></span>|<span data-ttu-id="7919b-164">Um não assinados long que especifica o valor mínimo permitido.</span><span class="sxs-lookup"><span data-stu-id="7919b-164">An unsigned long that specifies the minimum allowed value.</span></span> <span data-ttu-id="7919b-165">O valor padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="7919b-165">The default value is 0.</span></span>|
|<span data-ttu-id="7919b-166">maxValue</span><span class="sxs-lookup"><span data-stu-id="7919b-166">maxValue</span></span>|<span data-ttu-id="7919b-167">Int64</span><span class="sxs-lookup"><span data-stu-id="7919b-167">Int64</span></span>|<span data-ttu-id="7919b-168">Um não assinados long que especifica o valor máximo permitido.</span><span class="sxs-lookup"><span data-stu-id="7919b-168">An unsigned long that specifies the maximum allowed value.</span></span> <span data-ttu-id="7919b-169">O valor padrão é 9999.</span><span class="sxs-lookup"><span data-stu-id="7919b-169">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="7919b-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="7919b-170">Response</span></span>
<span data-ttu-id="7919b-171">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7919b-171">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7919b-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7919b-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="7919b-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7919b-173">Request</span></span>
<span data-ttu-id="7919b-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7919b-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 225

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationLongDecimalTextBox",
  "label": "Label value",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```

### <a name="response"></a><span data-ttu-id="7919b-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="7919b-175">Response</span></span>
<span data-ttu-id="7919b-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7919b-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 338

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationLongDecimalTextBox",
  "label": "Label value",
  "id": "754d8495-8495-754d-9584-4d7595844d75",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```




