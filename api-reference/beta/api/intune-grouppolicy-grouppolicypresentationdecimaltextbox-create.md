---
title: Criar groupPolicyPresentationDecimalTextBox
description: Crie um novo objeto groupPolicyPresentationDecimalTextBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0e2d9a32c3a2c9d17efa0d6a5550dbdf7042a743
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149692"
---
# <a name="create-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="6f2b8-103">Criar groupPolicyPresentationDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="6f2b8-103">Create groupPolicyPresentationDecimalTextBox</span></span>

<span data-ttu-id="6f2b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f2b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f2b8-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6f2b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f2b8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6f2b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f2b8-107">Crie um novo [objeto groupPolicyPresentationDecimalTextBox.](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)</span><span class="sxs-lookup"><span data-stu-id="6f2b8-107">Create a new [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f2b8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6f2b8-108">Prerequisites</span></span>
<span data-ttu-id="6f2b8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f2b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f2b8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f2b8-111">Permission type</span></span>|<span data-ttu-id="6f2b8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6f2b8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f2b8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f2b8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f2b8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f2b8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6f2b8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f2b8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f2b8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f2b8-116">Not supported.</span></span>|
|<span data-ttu-id="6f2b8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f2b8-117">Application</span></span>|<span data-ttu-id="6f2b8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f2b8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f2b8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f2b8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="6f2b8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f2b8-120">Request headers</span></span>
|<span data-ttu-id="6f2b8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6f2b8-121">Header</span></span>|<span data-ttu-id="6f2b8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6f2b8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f2b8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f2b8-123">Authorization</span></span>|<span data-ttu-id="6f2b8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f2b8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f2b8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6f2b8-125">Accept</span></span>|<span data-ttu-id="6f2b8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f2b8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f2b8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f2b8-127">Request body</span></span>
<span data-ttu-id="6f2b8-128">No corpo da solicitação, fornece uma representação JSON para o objeto groupPolicyPresentationDecimalTextBox.</span><span class="sxs-lookup"><span data-stu-id="6f2b8-128">In the request body, supply a JSON representation for the groupPolicyPresentationDecimalTextBox object.</span></span>

<span data-ttu-id="6f2b8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o groupPolicyPresentationDecimalTextBox.</span><span class="sxs-lookup"><span data-stu-id="6f2b8-129">The following table shows the properties that are required when you create the groupPolicyPresentationDecimalTextBox.</span></span>

|<span data-ttu-id="6f2b8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f2b8-130">Property</span></span>|<span data-ttu-id="6f2b8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f2b8-131">Type</span></span>|<span data-ttu-id="6f2b8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f2b8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f2b8-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="6f2b8-133">label</span></span>|<span data-ttu-id="6f2b8-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f2b8-134">String</span></span>|<span data-ttu-id="6f2b8-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="6f2b8-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="6f2b8-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="6f2b8-136">The default value is empty.</span></span> <span data-ttu-id="6f2b8-137">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="6f2b8-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="6f2b8-138">id</span><span class="sxs-lookup"><span data-stu-id="6f2b8-138">id</span></span>|<span data-ttu-id="6f2b8-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f2b8-139">String</span></span>|<span data-ttu-id="6f2b8-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6f2b8-140">Key of the entity.</span></span> <span data-ttu-id="6f2b8-141">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="6f2b8-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="6f2b8-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f2b8-142">lastModifiedDateTime</span></span>|<span data-ttu-id="6f2b8-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f2b8-143">DateTimeOffset</span></span>|<span data-ttu-id="6f2b8-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6f2b8-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="6f2b8-145">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="6f2b8-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="6f2b8-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="6f2b8-146">defaultValue</span></span>|<span data-ttu-id="6f2b8-147">Int64</span><span class="sxs-lookup"><span data-stu-id="6f2b8-147">Int64</span></span>|<span data-ttu-id="6f2b8-148">Um inteiro não assinado que especifica o valor inicial da caixa de texto decimal.</span><span class="sxs-lookup"><span data-stu-id="6f2b8-148">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="6f2b8-149">O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="6f2b8-149">The default value is 1.</span></span>|
|<span data-ttu-id="6f2b8-150">spin</span><span class="sxs-lookup"><span data-stu-id="6f2b8-150">spin</span></span>|<span data-ttu-id="6f2b8-151">Booleano</span><span class="sxs-lookup"><span data-stu-id="6f2b8-151">Boolean</span></span>|<span data-ttu-id="6f2b8-152">Se for true, crie um controle de rotação; caso contrário, crie uma caixa de texto para entrada numérica.</span><span class="sxs-lookup"><span data-stu-id="6f2b8-152">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="6f2b8-153">O valor padrão é true.</span><span class="sxs-lookup"><span data-stu-id="6f2b8-153">The default value is true.</span></span>|
|<span data-ttu-id="6f2b8-154">spinStep</span><span class="sxs-lookup"><span data-stu-id="6f2b8-154">spinStep</span></span>|<span data-ttu-id="6f2b8-155">Int64</span><span class="sxs-lookup"><span data-stu-id="6f2b8-155">Int64</span></span>|<span data-ttu-id="6f2b8-156">Um inteiro não assinado que especifica o incremento de alteração para o controle de rotação.</span><span class="sxs-lookup"><span data-stu-id="6f2b8-156">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="6f2b8-157">O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="6f2b8-157">The default value is 1.</span></span>|
|<span data-ttu-id="6f2b8-158">obrigatório</span><span class="sxs-lookup"><span data-stu-id="6f2b8-158">required</span></span>|<span data-ttu-id="6f2b8-159">Booleano</span><span class="sxs-lookup"><span data-stu-id="6f2b8-159">Boolean</span></span>|<span data-ttu-id="6f2b8-160">Requisito para inserir um valor na caixa de parâmetros.</span><span class="sxs-lookup"><span data-stu-id="6f2b8-160">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="6f2b8-161">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="6f2b8-161">The default value is false.</span></span>|
|<span data-ttu-id="6f2b8-162">minValue</span><span class="sxs-lookup"><span data-stu-id="6f2b8-162">minValue</span></span>|<span data-ttu-id="6f2b8-163">Int64</span><span class="sxs-lookup"><span data-stu-id="6f2b8-163">Int64</span></span>|<span data-ttu-id="6f2b8-164">Um inteiro não assinado que especifica o valor mínimo permitido.</span><span class="sxs-lookup"><span data-stu-id="6f2b8-164">An unsigned integer that specifies the minimum allowed value.</span></span> <span data-ttu-id="6f2b8-165">O valor padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="6f2b8-165">The default value is 0.</span></span>|
|<span data-ttu-id="6f2b8-166">maxValue</span><span class="sxs-lookup"><span data-stu-id="6f2b8-166">maxValue</span></span>|<span data-ttu-id="6f2b8-167">Int64</span><span class="sxs-lookup"><span data-stu-id="6f2b8-167">Int64</span></span>|<span data-ttu-id="6f2b8-168">Um inteiro não assinado que especifica o valor máximo permitido.</span><span class="sxs-lookup"><span data-stu-id="6f2b8-168">An unsigned integer that specifies the maximum allowed value.</span></span> <span data-ttu-id="6f2b8-169">O valor padrão é 9999.</span><span class="sxs-lookup"><span data-stu-id="6f2b8-169">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="6f2b8-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f2b8-170">Response</span></span>
<span data-ttu-id="6f2b8-171">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f2b8-171">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f2b8-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f2b8-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f2b8-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f2b8-173">Request</span></span>
<span data-ttu-id="6f2b8-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f2b8-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6f2b8-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f2b8-175">Response</span></span>
<span data-ttu-id="6f2b8-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6f2b8-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




