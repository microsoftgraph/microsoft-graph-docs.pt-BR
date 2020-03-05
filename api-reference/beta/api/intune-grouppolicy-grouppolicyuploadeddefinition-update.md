---
title: Atualizar groupPolicyUploadedDefinition
description: Atualiza as propriedades de um objeto groupPolicyUploadedDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9d0f31fdb28089c2792d453b00524314128bfb42
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42463851"
---
# <a name="update-grouppolicyuploadeddefinition"></a><span data-ttu-id="2295c-103">Atualizar groupPolicyUploadedDefinition</span><span class="sxs-lookup"><span data-stu-id="2295c-103">Update groupPolicyUploadedDefinition</span></span>

<span data-ttu-id="2295c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2295c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2295c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2295c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2295c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2295c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2295c-107">Atualiza as propriedades de um objeto [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="2295c-107">Update the properties of a [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2295c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2295c-108">Prerequisites</span></span>
<span data-ttu-id="2295c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2295c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2295c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2295c-111">Permission type</span></span>|<span data-ttu-id="2295c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2295c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2295c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2295c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2295c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2295c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2295c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2295c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2295c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2295c-116">Not supported.</span></span>|
|<span data-ttu-id="2295c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2295c-117">Application</span></span>|<span data-ttu-id="2295c-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2295c-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2295c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2295c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/definition
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions/{groupPolicyDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="2295c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2295c-120">Request headers</span></span>
|<span data-ttu-id="2295c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2295c-121">Header</span></span>|<span data-ttu-id="2295c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2295c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2295c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2295c-123">Authorization</span></span>|<span data-ttu-id="2295c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2295c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2295c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2295c-125">Accept</span></span>|<span data-ttu-id="2295c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2295c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2295c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2295c-127">Request body</span></span>
<span data-ttu-id="2295c-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="2295c-128">In the request body, supply a JSON representation for the [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object.</span></span>

<span data-ttu-id="2295c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md).</span><span class="sxs-lookup"><span data-stu-id="2295c-129">The following table shows the properties that are required when you create the [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md).</span></span>

|<span data-ttu-id="2295c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2295c-130">Property</span></span>|<span data-ttu-id="2295c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2295c-131">Type</span></span>|<span data-ttu-id="2295c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2295c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2295c-133">classType</span><span class="sxs-lookup"><span data-stu-id="2295c-133">classType</span></span>|[<span data-ttu-id="2295c-134">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="2295c-134">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="2295c-135">Identifica o tipo de grupo ao qual a política pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="2295c-135">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="2295c-136">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="2295c-136">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span> <span data-ttu-id="2295c-137">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="2295c-137">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="2295c-138">displayName</span><span class="sxs-lookup"><span data-stu-id="2295c-138">displayName</span></span>|<span data-ttu-id="2295c-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2295c-139">String</span></span>|<span data-ttu-id="2295c-140">O nome da política localizada.</span><span class="sxs-lookup"><span data-stu-id="2295c-140">The localized policy name.</span></span> <span data-ttu-id="2295c-141">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2295c-141">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="2295c-142">Texto não criptografado</span><span class="sxs-lookup"><span data-stu-id="2295c-142">explainText</span></span>|<span data-ttu-id="2295c-143">String</span><span class="sxs-lookup"><span data-stu-id="2295c-143">String</span></span>|<span data-ttu-id="2295c-144">A explicação localizada ou o texto de ajuda associado à política.</span><span class="sxs-lookup"><span data-stu-id="2295c-144">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="2295c-145">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="2295c-145">The default value is empty.</span></span> <span data-ttu-id="2295c-146">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2295c-146">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="2295c-147">categoryPath</span><span class="sxs-lookup"><span data-stu-id="2295c-147">categoryPath</span></span>|<span data-ttu-id="2295c-148">String</span><span class="sxs-lookup"><span data-stu-id="2295c-148">String</span></span>|<span data-ttu-id="2295c-149">O caminho de categoria completo localizado para a política.</span><span class="sxs-lookup"><span data-stu-id="2295c-149">The localized full category path for the policy.</span></span> <span data-ttu-id="2295c-150">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2295c-150">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="2295c-151">com suporte</span><span class="sxs-lookup"><span data-stu-id="2295c-151">supportedOn</span></span>|<span data-ttu-id="2295c-152">String</span><span class="sxs-lookup"><span data-stu-id="2295c-152">String</span></span>|<span data-ttu-id="2295c-153">Cadeia de caracteres localizada usada para especificar o sistema operacional ou a versão do aplicativo é afetada pela política.</span><span class="sxs-lookup"><span data-stu-id="2295c-153">Localized string used to specify what operating system or application version is affected by the policy.</span></span> <span data-ttu-id="2295c-154">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2295c-154">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="2295c-155">PolicyType</span><span class="sxs-lookup"><span data-stu-id="2295c-155">policyType</span></span>|[<span data-ttu-id="2295c-156">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="2295c-156">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="2295c-157">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="2295c-157">Specifies the type of group policy.</span></span> <span data-ttu-id="2295c-158">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="2295c-158">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span> <span data-ttu-id="2295c-159">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="2295c-159">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="2295c-160">id</span><span class="sxs-lookup"><span data-stu-id="2295c-160">id</span></span>|<span data-ttu-id="2295c-161">String</span><span class="sxs-lookup"><span data-stu-id="2295c-161">String</span></span>|<span data-ttu-id="2295c-162">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2295c-162">Key of the entity.</span></span> <span data-ttu-id="2295c-163">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2295c-163">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="2295c-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2295c-164">lastModifiedDateTime</span></span>|<span data-ttu-id="2295c-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2295c-165">DateTimeOffset</span></span>|<span data-ttu-id="2295c-166">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2295c-166">The date and time the entity was last modified.</span></span> <span data-ttu-id="2295c-167">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2295c-167">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="2295c-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="2295c-168">Response</span></span>
<span data-ttu-id="2295c-169">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2295c-169">If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2295c-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2295c-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="2295c-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2295c-171">Request</span></span>
<span data-ttu-id="2295c-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2295c-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
Content-type: application/json
Content-length: 293

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested"
}
```

### <a name="response"></a><span data-ttu-id="2295c-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="2295c-173">Response</span></span>
<span data-ttu-id="2295c-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2295c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 406

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "id": "a5f83119-3119-a5f8-1931-f8a51931f8a5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





