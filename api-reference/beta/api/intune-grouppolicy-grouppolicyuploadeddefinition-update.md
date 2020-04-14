---
title: Atualizar groupPolicyUploadedDefinition
description: Atualiza as propriedades de um objeto groupPolicyUploadedDefinition.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0dfefce242ea07312bdcc93f6fa3eeb592ad9770
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448199"
---
# <a name="update-grouppolicyuploadeddefinition"></a><span data-ttu-id="e49bd-103">Atualizar groupPolicyUploadedDefinition</span><span class="sxs-lookup"><span data-stu-id="e49bd-103">Update groupPolicyUploadedDefinition</span></span>

<span data-ttu-id="e49bd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e49bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e49bd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e49bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e49bd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e49bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e49bd-107">Atualiza as propriedades de um objeto [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="e49bd-107">Update the properties of a [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e49bd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e49bd-108">Prerequisites</span></span>
<span data-ttu-id="e49bd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e49bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e49bd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e49bd-111">Permission type</span></span>|<span data-ttu-id="e49bd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e49bd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e49bd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e49bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e49bd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e49bd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e49bd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e49bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e49bd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e49bd-116">Not supported.</span></span>|
|<span data-ttu-id="e49bd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e49bd-117">Application</span></span>|<span data-ttu-id="e49bd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e49bd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e49bd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e49bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/definition
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/definitions/{groupPolicyDefinitionId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions/{groupPolicyDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="e49bd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e49bd-120">Request headers</span></span>
|<span data-ttu-id="e49bd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e49bd-121">Header</span></span>|<span data-ttu-id="e49bd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e49bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e49bd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e49bd-123">Authorization</span></span>|<span data-ttu-id="e49bd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e49bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e49bd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e49bd-125">Accept</span></span>|<span data-ttu-id="e49bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e49bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e49bd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e49bd-127">Request body</span></span>
<span data-ttu-id="e49bd-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="e49bd-128">In the request body, supply a JSON representation for the [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object.</span></span>

<span data-ttu-id="e49bd-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md).</span><span class="sxs-lookup"><span data-stu-id="e49bd-129">The following table shows the properties that are required when you create the [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md).</span></span>

|<span data-ttu-id="e49bd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e49bd-130">Property</span></span>|<span data-ttu-id="e49bd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e49bd-131">Type</span></span>|<span data-ttu-id="e49bd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e49bd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e49bd-133">classType</span><span class="sxs-lookup"><span data-stu-id="e49bd-133">classType</span></span>|[<span data-ttu-id="e49bd-134">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="e49bd-134">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="e49bd-135">Identifica o tipo de grupo ao qual a política pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="e49bd-135">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="e49bd-136">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="e49bd-136">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span> <span data-ttu-id="e49bd-137">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="e49bd-137">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="e49bd-138">displayName</span><span class="sxs-lookup"><span data-stu-id="e49bd-138">displayName</span></span>|<span data-ttu-id="e49bd-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e49bd-139">String</span></span>|<span data-ttu-id="e49bd-140">O nome da política localizada.</span><span class="sxs-lookup"><span data-stu-id="e49bd-140">The localized policy name.</span></span> <span data-ttu-id="e49bd-141">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e49bd-141">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="e49bd-142">Texto não criptografado</span><span class="sxs-lookup"><span data-stu-id="e49bd-142">explainText</span></span>|<span data-ttu-id="e49bd-143">String</span><span class="sxs-lookup"><span data-stu-id="e49bd-143">String</span></span>|<span data-ttu-id="e49bd-144">A explicação localizada ou o texto de ajuda associado à política.</span><span class="sxs-lookup"><span data-stu-id="e49bd-144">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="e49bd-145">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="e49bd-145">The default value is empty.</span></span> <span data-ttu-id="e49bd-146">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e49bd-146">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="e49bd-147">categoryPath</span><span class="sxs-lookup"><span data-stu-id="e49bd-147">categoryPath</span></span>|<span data-ttu-id="e49bd-148">String</span><span class="sxs-lookup"><span data-stu-id="e49bd-148">String</span></span>|<span data-ttu-id="e49bd-149">O caminho de categoria completo localizado para a política.</span><span class="sxs-lookup"><span data-stu-id="e49bd-149">The localized full category path for the policy.</span></span> <span data-ttu-id="e49bd-150">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e49bd-150">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="e49bd-151">com suporte</span><span class="sxs-lookup"><span data-stu-id="e49bd-151">supportedOn</span></span>|<span data-ttu-id="e49bd-152">String</span><span class="sxs-lookup"><span data-stu-id="e49bd-152">String</span></span>|<span data-ttu-id="e49bd-153">Cadeia de caracteres localizada usada para especificar o sistema operacional ou a versão do aplicativo é afetada pela política.</span><span class="sxs-lookup"><span data-stu-id="e49bd-153">Localized string used to specify what operating system or application version is affected by the policy.</span></span> <span data-ttu-id="e49bd-154">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e49bd-154">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="e49bd-155">PolicyType</span><span class="sxs-lookup"><span data-stu-id="e49bd-155">policyType</span></span>|[<span data-ttu-id="e49bd-156">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="e49bd-156">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="e49bd-157">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="e49bd-157">Specifies the type of group policy.</span></span> <span data-ttu-id="e49bd-158">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="e49bd-158">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span> <span data-ttu-id="e49bd-159">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="e49bd-159">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="e49bd-160">groupPolicyCategoryId</span><span class="sxs-lookup"><span data-stu-id="e49bd-160">groupPolicyCategoryId</span></span>|<span data-ttu-id="e49bd-161">Guid</span><span class="sxs-lookup"><span data-stu-id="e49bd-161">Guid</span></span>|<span data-ttu-id="e49bd-162">A ID de categoria da categoria pai herdada de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e49bd-162">The category id of the parent category Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="e49bd-163">id</span><span class="sxs-lookup"><span data-stu-id="e49bd-163">id</span></span>|<span data-ttu-id="e49bd-164">String</span><span class="sxs-lookup"><span data-stu-id="e49bd-164">String</span></span>|<span data-ttu-id="e49bd-165">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e49bd-165">Key of the entity.</span></span> <span data-ttu-id="e49bd-166">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e49bd-166">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="e49bd-167">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e49bd-167">lastModifiedDateTime</span></span>|<span data-ttu-id="e49bd-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e49bd-168">DateTimeOffset</span></span>|<span data-ttu-id="e49bd-169">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e49bd-169">The date and time the entity was last modified.</span></span> <span data-ttu-id="e49bd-170">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e49bd-170">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="e49bd-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="e49bd-171">Response</span></span>
<span data-ttu-id="e49bd-172">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e49bd-172">If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e49bd-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e49bd-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="e49bd-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e49bd-174">Request</span></span>
<span data-ttu-id="e49bd-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e49bd-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "groupPolicyCategoryId": "4d1e97a2-97a2-4d1e-a297-1e4da2971e4d"
}
```

### <a name="response"></a><span data-ttu-id="e49bd-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="e49bd-176">Response</span></span>
<span data-ttu-id="e49bd-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e49bd-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 474

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "groupPolicyCategoryId": "4d1e97a2-97a2-4d1e-a297-1e4da2971e4d",
  "id": "a5f83119-3119-a5f8-1931-f8a51931f8a5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```



