---
title: Atualizar groupPolicyPresentationLongDecimalTextBox
description: Atualize as propriedades de um objeto groupPolicyPresentationLongDecimalTextBox.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b0b206a557ebd4715aede7e8becbeae672c8bea4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29428839"
---
# <a name="update-grouppolicypresentationlongdecimaltextbox"></a><span data-ttu-id="bee52-103">Atualizar groupPolicyPresentationLongDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="bee52-103">Update groupPolicyPresentationLongDecimalTextBox</span></span>

> <span data-ttu-id="bee52-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="bee52-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bee52-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bee52-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bee52-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="bee52-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bee52-107">Atualize as propriedades de um objeto [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="bee52-107">Update the properties of a [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bee52-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bee52-108">Prerequisites</span></span>
<span data-ttu-id="bee52-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bee52-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bee52-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bee52-111">Permission type</span></span>|<span data-ttu-id="bee52-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bee52-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bee52-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bee52-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bee52-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bee52-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bee52-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bee52-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bee52-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bee52-116">Not supported.</span></span>|
|<span data-ttu-id="bee52-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bee52-117">Application</span></span>|<span data-ttu-id="bee52-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bee52-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bee52-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bee52-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="bee52-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bee52-120">Request headers</span></span>
|<span data-ttu-id="bee52-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bee52-121">Header</span></span>|<span data-ttu-id="bee52-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bee52-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bee52-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bee52-123">Authorization</span></span>|<span data-ttu-id="bee52-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bee52-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bee52-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bee52-125">Accept</span></span>|<span data-ttu-id="bee52-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bee52-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bee52-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bee52-127">Request body</span></span>
<span data-ttu-id="bee52-128">No corpo da solicitação, fornece uma representação JSON para o objeto [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="bee52-128">In the request body, supply a JSON representation for the [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object.</span></span>

<span data-ttu-id="bee52-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md).</span><span class="sxs-lookup"><span data-stu-id="bee52-129">The following table shows the properties that are required when you create the [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md).</span></span>

|<span data-ttu-id="bee52-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bee52-130">Property</span></span>|<span data-ttu-id="bee52-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bee52-131">Type</span></span>|<span data-ttu-id="bee52-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bee52-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bee52-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="bee52-133">label</span></span>|<span data-ttu-id="bee52-134">String</span><span class="sxs-lookup"><span data-stu-id="bee52-134">String</span></span>|<span data-ttu-id="bee52-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="bee52-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="bee52-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="bee52-136">The default value is empty.</span></span> <span data-ttu-id="bee52-137">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="bee52-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="bee52-138">id</span><span class="sxs-lookup"><span data-stu-id="bee52-138">id</span></span>|<span data-ttu-id="bee52-139">String</span><span class="sxs-lookup"><span data-stu-id="bee52-139">String</span></span>|<span data-ttu-id="bee52-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bee52-140">Key of the entity.</span></span> <span data-ttu-id="bee52-141">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="bee52-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="bee52-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bee52-142">lastModifiedDateTime</span></span>|<span data-ttu-id="bee52-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bee52-143">DateTimeOffset</span></span>|<span data-ttu-id="bee52-144">A data e hora que a entidade foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="bee52-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="bee52-145">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="bee52-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="bee52-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="bee52-146">defaultValue</span></span>|<span data-ttu-id="bee52-147">Int64</span><span class="sxs-lookup"><span data-stu-id="bee52-147">Int64</span></span>|<span data-ttu-id="bee52-148">Um inteiro não assinado que especifica o valor inicial da caixa de texto decimal.</span><span class="sxs-lookup"><span data-stu-id="bee52-148">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="bee52-149">O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="bee52-149">The default value is 1.</span></span>|
|<span data-ttu-id="bee52-150">rotação</span><span class="sxs-lookup"><span data-stu-id="bee52-150">spin</span></span>|<span data-ttu-id="bee52-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="bee52-151">Boolean</span></span>|<span data-ttu-id="bee52-152">Se for true, crie um controle de rotação; Caso contrário, crie uma caixa de texto para entrada numérica.</span><span class="sxs-lookup"><span data-stu-id="bee52-152">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="bee52-153">O valor padrão é true.</span><span class="sxs-lookup"><span data-stu-id="bee52-153">The default value is true.</span></span>|
|<span data-ttu-id="bee52-154">spinStep</span><span class="sxs-lookup"><span data-stu-id="bee52-154">spinStep</span></span>|<span data-ttu-id="bee52-155">Int64</span><span class="sxs-lookup"><span data-stu-id="bee52-155">Int64</span></span>|<span data-ttu-id="bee52-156">Um inteiro não assinado que especifica o incremento de alteração para o controle de rotação.</span><span class="sxs-lookup"><span data-stu-id="bee52-156">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="bee52-157">O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="bee52-157">The default value is 1.</span></span>|
|<span data-ttu-id="bee52-158">obrigatório</span><span class="sxs-lookup"><span data-stu-id="bee52-158">required</span></span>|<span data-ttu-id="bee52-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="bee52-159">Boolean</span></span>|<span data-ttu-id="bee52-160">Requisito para inserir um valor na caixa de parâmetro.</span><span class="sxs-lookup"><span data-stu-id="bee52-160">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="bee52-161">O valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="bee52-161">The default value is false.</span></span>|
|<span data-ttu-id="bee52-162">minValue</span><span class="sxs-lookup"><span data-stu-id="bee52-162">minValue</span></span>|<span data-ttu-id="bee52-163">Int64</span><span class="sxs-lookup"><span data-stu-id="bee52-163">Int64</span></span>|<span data-ttu-id="bee52-164">Um não assinados long que especifica o valor mínimo permitido.</span><span class="sxs-lookup"><span data-stu-id="bee52-164">An unsigned long that specifies the minimum allowed value.</span></span> <span data-ttu-id="bee52-165">O valor padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="bee52-165">The default value is 0.</span></span>|
|<span data-ttu-id="bee52-166">maxValue</span><span class="sxs-lookup"><span data-stu-id="bee52-166">maxValue</span></span>|<span data-ttu-id="bee52-167">Int64</span><span class="sxs-lookup"><span data-stu-id="bee52-167">Int64</span></span>|<span data-ttu-id="bee52-168">Um não assinados long que especifica o valor máximo permitido.</span><span class="sxs-lookup"><span data-stu-id="bee52-168">An unsigned long that specifies the maximum allowed value.</span></span> <span data-ttu-id="bee52-169">O valor padrão é 9999.</span><span class="sxs-lookup"><span data-stu-id="bee52-169">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="bee52-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="bee52-170">Response</span></span>
<span data-ttu-id="bee52-171">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bee52-171">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bee52-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bee52-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="bee52-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bee52-173">Request</span></span>
<span data-ttu-id="bee52-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bee52-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bee52-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="bee52-175">Response</span></span>
<span data-ttu-id="bee52-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bee52-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




