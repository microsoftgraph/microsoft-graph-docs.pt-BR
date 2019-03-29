---
title: Atualizar groupPolicyPresentationLongDecimalTextBox
description: Atualiza as propriedades de um objeto groupPolicyPresentationLongDecimalTextBox.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 02bcc2147bccee59594627e5c2ce3eaac9c64c5e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978553"
---
# <a name="update-grouppolicypresentationlongdecimaltextbox"></a><span data-ttu-id="9b8bb-103">Atualizar groupPolicyPresentationLongDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="9b8bb-103">Update groupPolicyPresentationLongDecimalTextBox</span></span>

> <span data-ttu-id="9b8bb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9b8bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b8bb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9b8bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b8bb-106">Atualiza as propriedades de um objeto [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="9b8bb-106">Update the properties of a [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b8bb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9b8bb-107">Prerequisites</span></span>
<span data-ttu-id="9b8bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b8bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b8bb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b8bb-110">Permission type</span></span>|<span data-ttu-id="9b8bb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9b8bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b8bb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b8bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9b8bb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b8bb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9b8bb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b8bb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b8bb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b8bb-115">Not supported.</span></span>|
|<span data-ttu-id="9b8bb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b8bb-116">Application</span></span>|<span data-ttu-id="9b8bb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b8bb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b8bb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b8bb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="9b8bb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b8bb-119">Request headers</span></span>
|<span data-ttu-id="9b8bb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9b8bb-120">Header</span></span>|<span data-ttu-id="9b8bb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9b8bb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b8bb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b8bb-122">Authorization</span></span>|<span data-ttu-id="9b8bb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b8bb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b8bb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9b8bb-124">Accept</span></span>|<span data-ttu-id="9b8bb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9b8bb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b8bb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b8bb-126">Request body</span></span>
<span data-ttu-id="9b8bb-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="9b8bb-127">In the request body, supply a JSON representation for the [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object.</span></span>

<span data-ttu-id="9b8bb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md).</span><span class="sxs-lookup"><span data-stu-id="9b8bb-128">The following table shows the properties that are required when you create the [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md).</span></span>

|<span data-ttu-id="9b8bb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b8bb-129">Property</span></span>|<span data-ttu-id="9b8bb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b8bb-130">Type</span></span>|<span data-ttu-id="9b8bb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b8bb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b8bb-132">rótulo</span><span class="sxs-lookup"><span data-stu-id="9b8bb-132">label</span></span>|<span data-ttu-id="9b8bb-133">String</span><span class="sxs-lookup"><span data-stu-id="9b8bb-133">String</span></span>|<span data-ttu-id="9b8bb-134">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="9b8bb-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="9b8bb-135">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="9b8bb-135">The default value is empty.</span></span> <span data-ttu-id="9b8bb-136">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="9b8bb-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="9b8bb-137">id</span><span class="sxs-lookup"><span data-stu-id="9b8bb-137">id</span></span>|<span data-ttu-id="9b8bb-138">String</span><span class="sxs-lookup"><span data-stu-id="9b8bb-138">String</span></span>|<span data-ttu-id="9b8bb-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9b8bb-139">Key of the entity.</span></span> <span data-ttu-id="9b8bb-140">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="9b8bb-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="9b8bb-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b8bb-141">lastModifiedDateTime</span></span>|<span data-ttu-id="9b8bb-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b8bb-142">DateTimeOffset</span></span>|<span data-ttu-id="9b8bb-143">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9b8bb-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="9b8bb-144">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="9b8bb-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="9b8bb-145">defaultValue</span><span class="sxs-lookup"><span data-stu-id="9b8bb-145">defaultValue</span></span>|<span data-ttu-id="9b8bb-146">Int64</span><span class="sxs-lookup"><span data-stu-id="9b8bb-146">Int64</span></span>|<span data-ttu-id="9b8bb-147">Um inteiro sem sinal que especifica o valor inicial da caixa de texto decimal.</span><span class="sxs-lookup"><span data-stu-id="9b8bb-147">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="9b8bb-148">O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="9b8bb-148">The default value is 1.</span></span>|
|<span data-ttu-id="9b8bb-149">rotação</span><span class="sxs-lookup"><span data-stu-id="9b8bb-149">spin</span></span>|<span data-ttu-id="9b8bb-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b8bb-150">Boolean</span></span>|<span data-ttu-id="9b8bb-151">Se true, crie um controle de rotação; caso contrário, crie uma caixa de texto para entrada numérica.</span><span class="sxs-lookup"><span data-stu-id="9b8bb-151">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="9b8bb-152">O valor padrão é true.</span><span class="sxs-lookup"><span data-stu-id="9b8bb-152">The default value is true.</span></span>|
|<span data-ttu-id="9b8bb-153">spinStep</span><span class="sxs-lookup"><span data-stu-id="9b8bb-153">spinStep</span></span>|<span data-ttu-id="9b8bb-154">Int64</span><span class="sxs-lookup"><span data-stu-id="9b8bb-154">Int64</span></span>|<span data-ttu-id="9b8bb-155">Um inteiro sem sinal que especifica o incremento de alteração para o controle de rotação.</span><span class="sxs-lookup"><span data-stu-id="9b8bb-155">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="9b8bb-156">O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="9b8bb-156">The default value is 1.</span></span>|
|<span data-ttu-id="9b8bb-157">obrigatório</span><span class="sxs-lookup"><span data-stu-id="9b8bb-157">required</span></span>|<span data-ttu-id="9b8bb-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b8bb-158">Boolean</span></span>|<span data-ttu-id="9b8bb-159">Requisito para inserir um valor na caixa parâmetro.</span><span class="sxs-lookup"><span data-stu-id="9b8bb-159">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="9b8bb-160">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="9b8bb-160">The default value is false.</span></span>|
|<span data-ttu-id="9b8bb-161">MaxValue</span><span class="sxs-lookup"><span data-stu-id="9b8bb-161">minValue</span></span>|<span data-ttu-id="9b8bb-162">Int64</span><span class="sxs-lookup"><span data-stu-id="9b8bb-162">Int64</span></span>|<span data-ttu-id="9b8bb-163">Um Long não assinado que especifica o valor mínimo permitido.</span><span class="sxs-lookup"><span data-stu-id="9b8bb-163">An unsigned long that specifies the minimum allowed value.</span></span> <span data-ttu-id="9b8bb-164">O valor padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="9b8bb-164">The default value is 0.</span></span>|
|<span data-ttu-id="9b8bb-165">maxValue</span><span class="sxs-lookup"><span data-stu-id="9b8bb-165">maxValue</span></span>|<span data-ttu-id="9b8bb-166">Int64</span><span class="sxs-lookup"><span data-stu-id="9b8bb-166">Int64</span></span>|<span data-ttu-id="9b8bb-167">Um Long não assinado que especifica o valor máximo permitido.</span><span class="sxs-lookup"><span data-stu-id="9b8bb-167">An unsigned long that specifies the maximum allowed value.</span></span> <span data-ttu-id="9b8bb-168">O valor padrão é 9999.</span><span class="sxs-lookup"><span data-stu-id="9b8bb-168">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="9b8bb-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b8bb-169">Response</span></span>
<span data-ttu-id="9b8bb-170">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b8bb-170">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b8bb-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b8bb-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b8bb-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b8bb-172">Request</span></span>
<span data-ttu-id="9b8bb-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b8bb-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
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

### <a name="response"></a><span data-ttu-id="9b8bb-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b8bb-174">Response</span></span>
<span data-ttu-id="9b8bb-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9b8bb-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




