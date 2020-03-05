---
title: Criar groupPolicyUploadedDefinition
description: Criar um novo objeto groupPolicyUploadedDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c4f40f61d61050d3311f11bd8f8ded8381027a05
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42463865"
---
# <a name="create-grouppolicyuploadeddefinition"></a><span data-ttu-id="9be74-103">Criar groupPolicyUploadedDefinition</span><span class="sxs-lookup"><span data-stu-id="9be74-103">Create groupPolicyUploadedDefinition</span></span>

<span data-ttu-id="9be74-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9be74-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9be74-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9be74-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9be74-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9be74-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9be74-107">Criar um novo objeto [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="9be74-107">Create a new [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9be74-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9be74-108">Prerequisites</span></span>
<span data-ttu-id="9be74-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9be74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9be74-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9be74-111">Permission type</span></span>|<span data-ttu-id="9be74-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9be74-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9be74-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9be74-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9be74-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9be74-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9be74-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9be74-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9be74-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9be74-116">Not supported.</span></span>|
|<span data-ttu-id="9be74-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9be74-117">Application</span></span>|<span data-ttu-id="9be74-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9be74-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9be74-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9be74-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyDefinitions
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions
```

## <a name="request-headers"></a><span data-ttu-id="9be74-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9be74-120">Request headers</span></span>
|<span data-ttu-id="9be74-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9be74-121">Header</span></span>|<span data-ttu-id="9be74-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9be74-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9be74-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9be74-123">Authorization</span></span>|<span data-ttu-id="9be74-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9be74-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9be74-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9be74-125">Accept</span></span>|<span data-ttu-id="9be74-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9be74-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9be74-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9be74-127">Request body</span></span>
<span data-ttu-id="9be74-128">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyUploadedDefinition.</span><span class="sxs-lookup"><span data-stu-id="9be74-128">In the request body, supply a JSON representation for the groupPolicyUploadedDefinition object.</span></span>

<span data-ttu-id="9be74-129">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyUploadedDefinition.</span><span class="sxs-lookup"><span data-stu-id="9be74-129">The following table shows the properties that are required when you create the groupPolicyUploadedDefinition.</span></span>

|<span data-ttu-id="9be74-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9be74-130">Property</span></span>|<span data-ttu-id="9be74-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9be74-131">Type</span></span>|<span data-ttu-id="9be74-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9be74-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9be74-133">classType</span><span class="sxs-lookup"><span data-stu-id="9be74-133">classType</span></span>|[<span data-ttu-id="9be74-134">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="9be74-134">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="9be74-135">Identifica o tipo de grupo ao qual a política pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="9be74-135">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="9be74-136">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9be74-136">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span> <span data-ttu-id="9be74-137">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="9be74-137">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="9be74-138">displayName</span><span class="sxs-lookup"><span data-stu-id="9be74-138">displayName</span></span>|<span data-ttu-id="9be74-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9be74-139">String</span></span>|<span data-ttu-id="9be74-140">O nome da política localizada.</span><span class="sxs-lookup"><span data-stu-id="9be74-140">The localized policy name.</span></span> <span data-ttu-id="9be74-141">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9be74-141">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="9be74-142">Texto não criptografado</span><span class="sxs-lookup"><span data-stu-id="9be74-142">explainText</span></span>|<span data-ttu-id="9be74-143">String</span><span class="sxs-lookup"><span data-stu-id="9be74-143">String</span></span>|<span data-ttu-id="9be74-144">A explicação localizada ou o texto de ajuda associado à política.</span><span class="sxs-lookup"><span data-stu-id="9be74-144">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="9be74-145">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="9be74-145">The default value is empty.</span></span> <span data-ttu-id="9be74-146">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9be74-146">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="9be74-147">categoryPath</span><span class="sxs-lookup"><span data-stu-id="9be74-147">categoryPath</span></span>|<span data-ttu-id="9be74-148">String</span><span class="sxs-lookup"><span data-stu-id="9be74-148">String</span></span>|<span data-ttu-id="9be74-149">O caminho de categoria completo localizado para a política.</span><span class="sxs-lookup"><span data-stu-id="9be74-149">The localized full category path for the policy.</span></span> <span data-ttu-id="9be74-150">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9be74-150">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="9be74-151">com suporte</span><span class="sxs-lookup"><span data-stu-id="9be74-151">supportedOn</span></span>|<span data-ttu-id="9be74-152">String</span><span class="sxs-lookup"><span data-stu-id="9be74-152">String</span></span>|<span data-ttu-id="9be74-153">Cadeia de caracteres localizada usada para especificar o sistema operacional ou a versão do aplicativo é afetada pela política.</span><span class="sxs-lookup"><span data-stu-id="9be74-153">Localized string used to specify what operating system or application version is affected by the policy.</span></span> <span data-ttu-id="9be74-154">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9be74-154">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="9be74-155">PolicyType</span><span class="sxs-lookup"><span data-stu-id="9be74-155">policyType</span></span>|[<span data-ttu-id="9be74-156">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="9be74-156">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="9be74-157">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="9be74-157">Specifies the type of group policy.</span></span> <span data-ttu-id="9be74-158">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9be74-158">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span> <span data-ttu-id="9be74-159">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="9be74-159">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="9be74-160">id</span><span class="sxs-lookup"><span data-stu-id="9be74-160">id</span></span>|<span data-ttu-id="9be74-161">String</span><span class="sxs-lookup"><span data-stu-id="9be74-161">String</span></span>|<span data-ttu-id="9be74-162">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9be74-162">Key of the entity.</span></span> <span data-ttu-id="9be74-163">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9be74-163">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="9be74-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9be74-164">lastModifiedDateTime</span></span>|<span data-ttu-id="9be74-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9be74-165">DateTimeOffset</span></span>|<span data-ttu-id="9be74-166">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9be74-166">The date and time the entity was last modified.</span></span> <span data-ttu-id="9be74-167">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9be74-167">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="9be74-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="9be74-168">Response</span></span>
<span data-ttu-id="9be74-169">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9be74-169">If successful, this method returns a `201 Created` response code and a [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9be74-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9be74-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="9be74-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9be74-171">Request</span></span>
<span data-ttu-id="9be74-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9be74-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions
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

### <a name="response"></a><span data-ttu-id="9be74-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="9be74-173">Response</span></span>
<span data-ttu-id="9be74-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9be74-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





