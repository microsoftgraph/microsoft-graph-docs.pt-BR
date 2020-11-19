---
title: Atualizar groupPolicyDefinition
description: Atualiza as propriedades de um objeto groupPolicyDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ff7a0a56f01dcc3e2cc627548a3f7f77c97895ef
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49286000"
---
# <a name="update-grouppolicydefinition"></a><span data-ttu-id="c5d3a-103">Atualizar groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="c5d3a-103">Update groupPolicyDefinition</span></span>

<span data-ttu-id="c5d3a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5d3a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5d3a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c5d3a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5d3a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c5d3a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5d3a-107">Atualiza as propriedades de um objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="c5d3a-107">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5d3a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c5d3a-108">Prerequisites</span></span>
<span data-ttu-id="c5d3a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5d3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5d3a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5d3a-111">Permission type</span></span>|<span data-ttu-id="c5d3a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c5d3a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5d3a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5d3a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5d3a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5d3a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c5d3a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5d3a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5d3a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5d3a-116">Not supported.</span></span>|
|<span data-ttu-id="c5d3a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5d3a-117">Application</span></span>|<span data-ttu-id="c5d3a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5d3a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5d3a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5d3a-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="c5d3a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5d3a-120">Request headers</span></span>
|<span data-ttu-id="c5d3a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c5d3a-121">Header</span></span>|<span data-ttu-id="c5d3a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c5d3a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5d3a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5d3a-123">Authorization</span></span>|<span data-ttu-id="c5d3a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5d3a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5d3a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c5d3a-125">Accept</span></span>|<span data-ttu-id="c5d3a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5d3a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5d3a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5d3a-127">Request body</span></span>
<span data-ttu-id="c5d3a-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="c5d3a-128">In the request body, supply a JSON representation for the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

<span data-ttu-id="c5d3a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c5d3a-129">The following table shows the properties that are required when you create the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span>

|<span data-ttu-id="c5d3a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5d3a-130">Property</span></span>|<span data-ttu-id="c5d3a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5d3a-131">Type</span></span>|<span data-ttu-id="c5d3a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5d3a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5d3a-133">classType</span><span class="sxs-lookup"><span data-stu-id="c5d3a-133">classType</span></span>|[<span data-ttu-id="c5d3a-134">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="c5d3a-134">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="c5d3a-135">Identifica o tipo de grupo ao qual a política pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="c5d3a-135">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="c5d3a-136">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="c5d3a-136">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="c5d3a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c5d3a-137">displayName</span></span>|<span data-ttu-id="c5d3a-138">String</span><span class="sxs-lookup"><span data-stu-id="c5d3a-138">String</span></span>|<span data-ttu-id="c5d3a-139">O nome da política localizada.</span><span class="sxs-lookup"><span data-stu-id="c5d3a-139">The localized policy name.</span></span>|
|<span data-ttu-id="c5d3a-140">Texto não criptografado</span><span class="sxs-lookup"><span data-stu-id="c5d3a-140">explainText</span></span>|<span data-ttu-id="c5d3a-141">String</span><span class="sxs-lookup"><span data-stu-id="c5d3a-141">String</span></span>|<span data-ttu-id="c5d3a-142">A explicação localizada ou o texto de ajuda associado à política.</span><span class="sxs-lookup"><span data-stu-id="c5d3a-142">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="c5d3a-143">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="c5d3a-143">The default value is empty.</span></span>|
|<span data-ttu-id="c5d3a-144">categoryPath</span><span class="sxs-lookup"><span data-stu-id="c5d3a-144">categoryPath</span></span>|<span data-ttu-id="c5d3a-145">String</span><span class="sxs-lookup"><span data-stu-id="c5d3a-145">String</span></span>|<span data-ttu-id="c5d3a-146">O caminho de categoria completo localizado para a política.</span><span class="sxs-lookup"><span data-stu-id="c5d3a-146">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="c5d3a-147">com suporte</span><span class="sxs-lookup"><span data-stu-id="c5d3a-147">supportedOn</span></span>|<span data-ttu-id="c5d3a-148">String</span><span class="sxs-lookup"><span data-stu-id="c5d3a-148">String</span></span>|<span data-ttu-id="c5d3a-149">Cadeia de caracteres localizada usada para especificar o sistema operacional ou a versão do aplicativo é afetada pela política.</span><span class="sxs-lookup"><span data-stu-id="c5d3a-149">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="c5d3a-150">PolicyType</span><span class="sxs-lookup"><span data-stu-id="c5d3a-150">policyType</span></span>|[<span data-ttu-id="c5d3a-151">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="c5d3a-151">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="c5d3a-152">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="c5d3a-152">Specifies the type of group policy.</span></span> <span data-ttu-id="c5d3a-153">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="c5d3a-153">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="c5d3a-154">groupPolicyCategoryId</span><span class="sxs-lookup"><span data-stu-id="c5d3a-154">groupPolicyCategoryId</span></span>|<span data-ttu-id="c5d3a-155">Guid</span><span class="sxs-lookup"><span data-stu-id="c5d3a-155">Guid</span></span>|<span data-ttu-id="c5d3a-156">A ID de categoria da categoria pai</span><span class="sxs-lookup"><span data-stu-id="c5d3a-156">The category id of the parent category</span></span>|
|<span data-ttu-id="c5d3a-157">id</span><span class="sxs-lookup"><span data-stu-id="c5d3a-157">id</span></span>|<span data-ttu-id="c5d3a-158">String</span><span class="sxs-lookup"><span data-stu-id="c5d3a-158">String</span></span>|<span data-ttu-id="c5d3a-159">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c5d3a-159">Key of the entity.</span></span>|
|<span data-ttu-id="c5d3a-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5d3a-160">lastModifiedDateTime</span></span>|<span data-ttu-id="c5d3a-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5d3a-161">DateTimeOffset</span></span>|<span data-ttu-id="c5d3a-162">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="c5d3a-162">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="c5d3a-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5d3a-163">Response</span></span>
<span data-ttu-id="c5d3a-164">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5d3a-164">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5d3a-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5d3a-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5d3a-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5d3a-166">Request</span></span>
<span data-ttu-id="c5d3a-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5d3a-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
Content-type: application/json
Content-length: 353

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "groupPolicyCategoryId": "4d1e97a2-97a2-4d1e-a297-1e4da2971e4d"
}
```

### <a name="response"></a><span data-ttu-id="c5d3a-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5d3a-168">Response</span></span>
<span data-ttu-id="c5d3a-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5d3a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 466

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "groupPolicyCategoryId": "4d1e97a2-97a2-4d1e-a297-1e4da2971e4d",
  "id": "f9607947-7947-f960-4779-60f9477960f9",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




