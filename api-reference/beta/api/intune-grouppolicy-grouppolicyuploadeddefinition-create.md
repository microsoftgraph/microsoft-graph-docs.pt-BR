---
title: Criar groupPolicyUploadedDefinition
description: Criar um novo objeto groupPolicyUploadedDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 18254611d04bb408aa798b2df892d30a9ac14994
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42160821"
---
# <a name="create-grouppolicyuploadeddefinition"></a><span data-ttu-id="be099-103">Criar groupPolicyUploadedDefinition</span><span class="sxs-lookup"><span data-stu-id="be099-103">Create groupPolicyUploadedDefinition</span></span>

> <span data-ttu-id="be099-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="be099-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be099-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="be099-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be099-106">Criar um novo objeto [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="be099-106">Create a new [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be099-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="be099-107">Prerequisites</span></span>
<span data-ttu-id="be099-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be099-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be099-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be099-110">Permission type</span></span>|<span data-ttu-id="be099-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="be099-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be099-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be099-112">Delegated (work or school account)</span></span>|<span data-ttu-id="be099-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be099-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="be099-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be099-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be099-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be099-115">Not supported.</span></span>|
|<span data-ttu-id="be099-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be099-116">Application</span></span>|<span data-ttu-id="be099-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be099-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="be099-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be099-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyDefinitions
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions
```

## <a name="request-headers"></a><span data-ttu-id="be099-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be099-119">Request headers</span></span>
|<span data-ttu-id="be099-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="be099-120">Header</span></span>|<span data-ttu-id="be099-121">Valor</span><span class="sxs-lookup"><span data-stu-id="be099-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be099-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="be099-122">Authorization</span></span>|<span data-ttu-id="be099-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be099-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be099-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="be099-124">Accept</span></span>|<span data-ttu-id="be099-125">application/json</span><span class="sxs-lookup"><span data-stu-id="be099-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be099-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be099-126">Request body</span></span>
<span data-ttu-id="be099-127">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyUploadedDefinition.</span><span class="sxs-lookup"><span data-stu-id="be099-127">In the request body, supply a JSON representation for the groupPolicyUploadedDefinition object.</span></span>

<span data-ttu-id="be099-128">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyUploadedDefinition.</span><span class="sxs-lookup"><span data-stu-id="be099-128">The following table shows the properties that are required when you create the groupPolicyUploadedDefinition.</span></span>

|<span data-ttu-id="be099-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be099-129">Property</span></span>|<span data-ttu-id="be099-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="be099-130">Type</span></span>|<span data-ttu-id="be099-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="be099-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be099-132">classType</span><span class="sxs-lookup"><span data-stu-id="be099-132">classType</span></span>|[<span data-ttu-id="be099-133">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="be099-133">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="be099-134">Identifica o tipo de grupo ao qual a política pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="be099-134">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="be099-135">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="be099-135">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span> <span data-ttu-id="be099-136">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="be099-136">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="be099-137">displayName</span><span class="sxs-lookup"><span data-stu-id="be099-137">displayName</span></span>|<span data-ttu-id="be099-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be099-138">String</span></span>|<span data-ttu-id="be099-139">O nome da política localizada.</span><span class="sxs-lookup"><span data-stu-id="be099-139">The localized policy name.</span></span> <span data-ttu-id="be099-140">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="be099-140">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="be099-141">Texto não criptografado</span><span class="sxs-lookup"><span data-stu-id="be099-141">explainText</span></span>|<span data-ttu-id="be099-142">String</span><span class="sxs-lookup"><span data-stu-id="be099-142">String</span></span>|<span data-ttu-id="be099-143">A explicação localizada ou o texto de ajuda associado à política.</span><span class="sxs-lookup"><span data-stu-id="be099-143">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="be099-144">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="be099-144">The default value is empty.</span></span> <span data-ttu-id="be099-145">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="be099-145">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="be099-146">categoryPath</span><span class="sxs-lookup"><span data-stu-id="be099-146">categoryPath</span></span>|<span data-ttu-id="be099-147">String</span><span class="sxs-lookup"><span data-stu-id="be099-147">String</span></span>|<span data-ttu-id="be099-148">O caminho de categoria completo localizado para a política.</span><span class="sxs-lookup"><span data-stu-id="be099-148">The localized full category path for the policy.</span></span> <span data-ttu-id="be099-149">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="be099-149">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="be099-150">com suporte</span><span class="sxs-lookup"><span data-stu-id="be099-150">supportedOn</span></span>|<span data-ttu-id="be099-151">String</span><span class="sxs-lookup"><span data-stu-id="be099-151">String</span></span>|<span data-ttu-id="be099-152">Cadeia de caracteres localizada usada para especificar o sistema operacional ou a versão do aplicativo é afetada pela política.</span><span class="sxs-lookup"><span data-stu-id="be099-152">Localized string used to specify what operating system or application version is affected by the policy.</span></span> <span data-ttu-id="be099-153">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="be099-153">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="be099-154">PolicyType</span><span class="sxs-lookup"><span data-stu-id="be099-154">policyType</span></span>|[<span data-ttu-id="be099-155">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="be099-155">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="be099-156">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="be099-156">Specifies the type of group policy.</span></span> <span data-ttu-id="be099-157">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="be099-157">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span> <span data-ttu-id="be099-158">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="be099-158">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="be099-159">id</span><span class="sxs-lookup"><span data-stu-id="be099-159">id</span></span>|<span data-ttu-id="be099-160">String</span><span class="sxs-lookup"><span data-stu-id="be099-160">String</span></span>|<span data-ttu-id="be099-161">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="be099-161">Key of the entity.</span></span> <span data-ttu-id="be099-162">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="be099-162">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="be099-163">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be099-163">lastModifiedDateTime</span></span>|<span data-ttu-id="be099-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be099-164">DateTimeOffset</span></span>|<span data-ttu-id="be099-165">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="be099-165">The date and time the entity was last modified.</span></span> <span data-ttu-id="be099-166">Herdado de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="be099-166">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="be099-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="be099-167">Response</span></span>
<span data-ttu-id="be099-168">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be099-168">If successful, this method returns a `201 Created` response code and a [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be099-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="be099-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="be099-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be099-170">Request</span></span>
<span data-ttu-id="be099-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="be099-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="be099-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="be099-172">Response</span></span>
<span data-ttu-id="be099-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="be099-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





