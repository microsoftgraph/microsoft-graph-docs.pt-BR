---
title: Atualizar groupPolicyPresentationLongDecimalTextBox
description: Atualize as propriedades de um objeto groupPolicyPresentationLongDecimalTextBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5c1dfaa1d7c1cdb2bf7bd0fc0ced89ffca078a44
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153248"
---
# <a name="update-grouppolicypresentationlongdecimaltextbox"></a><span data-ttu-id="b67c2-103">Atualizar groupPolicyPresentationLongDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="b67c2-103">Update groupPolicyPresentationLongDecimalTextBox</span></span>

<span data-ttu-id="b67c2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b67c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b67c2-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b67c2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b67c2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b67c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b67c2-107">Atualize as propriedades de [um objeto groupPolicyPresentationLongDecimalTextBox.](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)</span><span class="sxs-lookup"><span data-stu-id="b67c2-107">Update the properties of a [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b67c2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b67c2-108">Prerequisites</span></span>
<span data-ttu-id="b67c2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b67c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b67c2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b67c2-111">Permission type</span></span>|<span data-ttu-id="b67c2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b67c2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b67c2-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b67c2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b67c2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b67c2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b67c2-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b67c2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b67c2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b67c2-116">Not supported.</span></span>|
|<span data-ttu-id="b67c2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b67c2-117">Application</span></span>|<span data-ttu-id="b67c2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b67c2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b67c2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b67c2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="b67c2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b67c2-120">Request headers</span></span>
|<span data-ttu-id="b67c2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b67c2-121">Header</span></span>|<span data-ttu-id="b67c2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b67c2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b67c2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b67c2-123">Authorization</span></span>|<span data-ttu-id="b67c2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b67c2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b67c2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b67c2-125">Accept</span></span>|<span data-ttu-id="b67c2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b67c2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b67c2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b67c2-127">Request body</span></span>
<span data-ttu-id="b67c2-128">No corpo da solicitação, fornece uma representação JSON para [o objeto groupPolicyPresentationLongDecimalTextBox.](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)</span><span class="sxs-lookup"><span data-stu-id="b67c2-128">In the request body, supply a JSON representation for the [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object.</span></span>

<span data-ttu-id="b67c2-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md).</span><span class="sxs-lookup"><span data-stu-id="b67c2-129">The following table shows the properties that are required when you create the [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md).</span></span>

|<span data-ttu-id="b67c2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b67c2-130">Property</span></span>|<span data-ttu-id="b67c2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b67c2-131">Type</span></span>|<span data-ttu-id="b67c2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b67c2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b67c2-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="b67c2-133">label</span></span>|<span data-ttu-id="b67c2-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b67c2-134">String</span></span>|<span data-ttu-id="b67c2-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="b67c2-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="b67c2-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="b67c2-136">The default value is empty.</span></span> <span data-ttu-id="b67c2-137">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="b67c2-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="b67c2-138">id</span><span class="sxs-lookup"><span data-stu-id="b67c2-138">id</span></span>|<span data-ttu-id="b67c2-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b67c2-139">String</span></span>|<span data-ttu-id="b67c2-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b67c2-140">Key of the entity.</span></span> <span data-ttu-id="b67c2-141">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="b67c2-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="b67c2-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b67c2-142">lastModifiedDateTime</span></span>|<span data-ttu-id="b67c2-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b67c2-143">DateTimeOffset</span></span>|<span data-ttu-id="b67c2-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b67c2-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="b67c2-145">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="b67c2-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="b67c2-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="b67c2-146">defaultValue</span></span>|<span data-ttu-id="b67c2-147">Int64</span><span class="sxs-lookup"><span data-stu-id="b67c2-147">Int64</span></span>|<span data-ttu-id="b67c2-148">Um inteiro não assinado que especifica o valor inicial da caixa de texto decimal.</span><span class="sxs-lookup"><span data-stu-id="b67c2-148">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="b67c2-149">O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="b67c2-149">The default value is 1.</span></span>|
|<span data-ttu-id="b67c2-150">spin</span><span class="sxs-lookup"><span data-stu-id="b67c2-150">spin</span></span>|<span data-ttu-id="b67c2-151">Booleano</span><span class="sxs-lookup"><span data-stu-id="b67c2-151">Boolean</span></span>|<span data-ttu-id="b67c2-152">Se for true, crie um controle de rotação; caso contrário, crie uma caixa de texto para entrada numérica.</span><span class="sxs-lookup"><span data-stu-id="b67c2-152">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="b67c2-153">O valor padrão é true.</span><span class="sxs-lookup"><span data-stu-id="b67c2-153">The default value is true.</span></span>|
|<span data-ttu-id="b67c2-154">spinStep</span><span class="sxs-lookup"><span data-stu-id="b67c2-154">spinStep</span></span>|<span data-ttu-id="b67c2-155">Int64</span><span class="sxs-lookup"><span data-stu-id="b67c2-155">Int64</span></span>|<span data-ttu-id="b67c2-156">Um inteiro não assinado que especifica o incremento de alteração para o controle de rotação.</span><span class="sxs-lookup"><span data-stu-id="b67c2-156">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="b67c2-157">O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="b67c2-157">The default value is 1.</span></span>|
|<span data-ttu-id="b67c2-158">obrigatório</span><span class="sxs-lookup"><span data-stu-id="b67c2-158">required</span></span>|<span data-ttu-id="b67c2-159">Booleano</span><span class="sxs-lookup"><span data-stu-id="b67c2-159">Boolean</span></span>|<span data-ttu-id="b67c2-160">Requisito para inserir um valor na caixa de parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b67c2-160">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="b67c2-161">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="b67c2-161">The default value is false.</span></span>|
|<span data-ttu-id="b67c2-162">minValue</span><span class="sxs-lookup"><span data-stu-id="b67c2-162">minValue</span></span>|<span data-ttu-id="b67c2-163">Int64</span><span class="sxs-lookup"><span data-stu-id="b67c2-163">Int64</span></span>|<span data-ttu-id="b67c2-164">Um long não assinado que especifica o valor mínimo permitido.</span><span class="sxs-lookup"><span data-stu-id="b67c2-164">An unsigned long that specifies the minimum allowed value.</span></span> <span data-ttu-id="b67c2-165">O valor padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="b67c2-165">The default value is 0.</span></span>|
|<span data-ttu-id="b67c2-166">maxValue</span><span class="sxs-lookup"><span data-stu-id="b67c2-166">maxValue</span></span>|<span data-ttu-id="b67c2-167">Int64</span><span class="sxs-lookup"><span data-stu-id="b67c2-167">Int64</span></span>|<span data-ttu-id="b67c2-168">Um long não assinado que especifica o valor máximo permitido.</span><span class="sxs-lookup"><span data-stu-id="b67c2-168">An unsigned long that specifies the maximum allowed value.</span></span> <span data-ttu-id="b67c2-169">O valor padrão é 9999.</span><span class="sxs-lookup"><span data-stu-id="b67c2-169">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="b67c2-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="b67c2-170">Response</span></span>
<span data-ttu-id="b67c2-171">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b67c2-171">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b67c2-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b67c2-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="b67c2-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b67c2-173">Request</span></span>
<span data-ttu-id="b67c2-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b67c2-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b67c2-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="b67c2-175">Response</span></span>
<span data-ttu-id="b67c2-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b67c2-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




