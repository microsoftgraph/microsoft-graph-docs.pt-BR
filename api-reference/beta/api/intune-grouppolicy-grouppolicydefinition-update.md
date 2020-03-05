---
title: Atualizar groupPolicyDefinition
description: Atualiza as propriedades de um objeto groupPolicyDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c9470b2affadb3ea0cdd38f1dbbb8dd9d44fa966
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465160"
---
# <a name="update-grouppolicydefinition"></a><span data-ttu-id="e7044-103">Atualizar groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="e7044-103">Update groupPolicyDefinition</span></span>

<span data-ttu-id="e7044-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e7044-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7044-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e7044-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7044-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e7044-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7044-107">Atualiza as propriedades de um objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="e7044-107">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7044-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e7044-108">Prerequisites</span></span>
<span data-ttu-id="e7044-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7044-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7044-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7044-111">Permission type</span></span>|<span data-ttu-id="e7044-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e7044-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7044-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7044-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e7044-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7044-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e7044-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7044-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7044-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7044-116">Not supported.</span></span>|
|<span data-ttu-id="e7044-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7044-117">Application</span></span>|<span data-ttu-id="e7044-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7044-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7044-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7044-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="e7044-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7044-120">Request headers</span></span>
|<span data-ttu-id="e7044-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7044-121">Header</span></span>|<span data-ttu-id="e7044-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e7044-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7044-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7044-123">Authorization</span></span>|<span data-ttu-id="e7044-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7044-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7044-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e7044-125">Accept</span></span>|<span data-ttu-id="e7044-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e7044-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7044-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7044-127">Request body</span></span>
<span data-ttu-id="e7044-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="e7044-128">In the request body, supply a JSON representation for the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

<span data-ttu-id="e7044-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="e7044-129">The following table shows the properties that are required when you create the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span>

|<span data-ttu-id="e7044-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e7044-130">Property</span></span>|<span data-ttu-id="e7044-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7044-131">Type</span></span>|<span data-ttu-id="e7044-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7044-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7044-133">classType</span><span class="sxs-lookup"><span data-stu-id="e7044-133">classType</span></span>|[<span data-ttu-id="e7044-134">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="e7044-134">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="e7044-135">Identifica o tipo de grupo ao qual a política pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="e7044-135">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="e7044-136">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="e7044-136">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="e7044-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e7044-137">displayName</span></span>|<span data-ttu-id="e7044-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7044-138">String</span></span>|<span data-ttu-id="e7044-139">O nome da política localizada.</span><span class="sxs-lookup"><span data-stu-id="e7044-139">The localized policy name.</span></span>|
|<span data-ttu-id="e7044-140">Texto não criptografado</span><span class="sxs-lookup"><span data-stu-id="e7044-140">explainText</span></span>|<span data-ttu-id="e7044-141">String</span><span class="sxs-lookup"><span data-stu-id="e7044-141">String</span></span>|<span data-ttu-id="e7044-142">A explicação localizada ou o texto de ajuda associado à política.</span><span class="sxs-lookup"><span data-stu-id="e7044-142">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="e7044-143">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="e7044-143">The default value is empty.</span></span>|
|<span data-ttu-id="e7044-144">categoryPath</span><span class="sxs-lookup"><span data-stu-id="e7044-144">categoryPath</span></span>|<span data-ttu-id="e7044-145">String</span><span class="sxs-lookup"><span data-stu-id="e7044-145">String</span></span>|<span data-ttu-id="e7044-146">O caminho de categoria completo localizado para a política.</span><span class="sxs-lookup"><span data-stu-id="e7044-146">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="e7044-147">com suporte</span><span class="sxs-lookup"><span data-stu-id="e7044-147">supportedOn</span></span>|<span data-ttu-id="e7044-148">String</span><span class="sxs-lookup"><span data-stu-id="e7044-148">String</span></span>|<span data-ttu-id="e7044-149">Cadeia de caracteres localizada usada para especificar o sistema operacional ou a versão do aplicativo é afetada pela política.</span><span class="sxs-lookup"><span data-stu-id="e7044-149">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="e7044-150">PolicyType</span><span class="sxs-lookup"><span data-stu-id="e7044-150">policyType</span></span>|[<span data-ttu-id="e7044-151">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="e7044-151">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="e7044-152">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="e7044-152">Specifies the type of group policy.</span></span> <span data-ttu-id="e7044-153">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="e7044-153">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="e7044-154">id</span><span class="sxs-lookup"><span data-stu-id="e7044-154">id</span></span>|<span data-ttu-id="e7044-155">String</span><span class="sxs-lookup"><span data-stu-id="e7044-155">String</span></span>|<span data-ttu-id="e7044-156">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e7044-156">Key of the entity.</span></span>|
|<span data-ttu-id="e7044-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7044-157">lastModifiedDateTime</span></span>|<span data-ttu-id="e7044-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7044-158">DateTimeOffset</span></span>|<span data-ttu-id="e7044-159">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e7044-159">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="e7044-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7044-160">Response</span></span>
<span data-ttu-id="e7044-161">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7044-161">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7044-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7044-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7044-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7044-163">Request</span></span>
<span data-ttu-id="e7044-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7044-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
Content-type: application/json
Content-length: 285

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested"
}
```

### <a name="response"></a><span data-ttu-id="e7044-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7044-165">Response</span></span>
<span data-ttu-id="e7044-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7044-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 398

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "id": "f9607947-7947-f960-4779-60f9477960f9",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





