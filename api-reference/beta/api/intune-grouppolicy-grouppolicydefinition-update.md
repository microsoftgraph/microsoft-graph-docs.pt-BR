---
title: Atualizar groupPolicyDefinition
description: Atualiza as propriedades de um objeto groupPolicyDefinition.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 02010b63320f295dad8ec5d5c579d5aa19d0a062
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804426"
---
# <a name="update-grouppolicydefinition"></a><span data-ttu-id="d7de0-103">Atualizar groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="d7de0-103">Update groupPolicyDefinition</span></span>

> <span data-ttu-id="d7de0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d7de0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7de0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d7de0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7de0-106">Atualiza as propriedades de um objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="d7de0-106">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7de0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d7de0-107">Prerequisites</span></span>
<span data-ttu-id="d7de0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7de0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7de0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7de0-110">Permission type</span></span>|<span data-ttu-id="d7de0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d7de0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7de0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7de0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d7de0-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7de0-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d7de0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7de0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7de0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7de0-115">Not supported.</span></span>|
|<span data-ttu-id="d7de0-116">Application</span><span class="sxs-lookup"><span data-stu-id="d7de0-116">Application</span></span>|<span data-ttu-id="d7de0-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7de0-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7de0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7de0-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="d7de0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7de0-119">Request headers</span></span>
|<span data-ttu-id="d7de0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d7de0-120">Header</span></span>|<span data-ttu-id="d7de0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d7de0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7de0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7de0-122">Authorization</span></span>|<span data-ttu-id="d7de0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7de0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7de0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d7de0-124">Accept</span></span>|<span data-ttu-id="d7de0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d7de0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7de0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7de0-126">Request body</span></span>
<span data-ttu-id="d7de0-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="d7de0-127">In the request body, supply a JSON representation for the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

<span data-ttu-id="d7de0-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="d7de0-128">The following table shows the properties that are required when you create the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span>

|<span data-ttu-id="d7de0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7de0-129">Property</span></span>|<span data-ttu-id="d7de0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7de0-130">Type</span></span>|<span data-ttu-id="d7de0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7de0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7de0-132">classType</span><span class="sxs-lookup"><span data-stu-id="d7de0-132">classType</span></span>|[<span data-ttu-id="d7de0-133">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="d7de0-133">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="d7de0-134">Identifica o tipo de grupo ao qual a política pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="d7de0-134">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="d7de0-135">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="d7de0-135">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="d7de0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d7de0-136">displayName</span></span>|<span data-ttu-id="d7de0-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7de0-137">String</span></span>|<span data-ttu-id="d7de0-138">O nome da política localizada.</span><span class="sxs-lookup"><span data-stu-id="d7de0-138">The localized policy name.</span></span>|
|<span data-ttu-id="d7de0-139">Texto não criptografado</span><span class="sxs-lookup"><span data-stu-id="d7de0-139">explainText</span></span>|<span data-ttu-id="d7de0-140">String</span><span class="sxs-lookup"><span data-stu-id="d7de0-140">String</span></span>|<span data-ttu-id="d7de0-141">A explicação localizada ou o texto de ajuda associado à política.</span><span class="sxs-lookup"><span data-stu-id="d7de0-141">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="d7de0-142">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="d7de0-142">The default value is empty.</span></span>|
|<span data-ttu-id="d7de0-143">categoryPath</span><span class="sxs-lookup"><span data-stu-id="d7de0-143">categoryPath</span></span>|<span data-ttu-id="d7de0-144">String</span><span class="sxs-lookup"><span data-stu-id="d7de0-144">String</span></span>|<span data-ttu-id="d7de0-145">O caminho de categoria completo localizado para a política.</span><span class="sxs-lookup"><span data-stu-id="d7de0-145">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="d7de0-146">com suporte</span><span class="sxs-lookup"><span data-stu-id="d7de0-146">supportedOn</span></span>|<span data-ttu-id="d7de0-147">String</span><span class="sxs-lookup"><span data-stu-id="d7de0-147">String</span></span>|<span data-ttu-id="d7de0-148">Cadeia de caracteres localizada usada para especificar o sistema operacional ou a versão do aplicativo é afetada pela política.</span><span class="sxs-lookup"><span data-stu-id="d7de0-148">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="d7de0-149">PolicyType</span><span class="sxs-lookup"><span data-stu-id="d7de0-149">policyType</span></span>|[<span data-ttu-id="d7de0-150">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="d7de0-150">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="d7de0-151">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="d7de0-151">Specifies the type of group policy.</span></span> <span data-ttu-id="d7de0-152">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="d7de0-152">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="d7de0-153">groupPolicyCategoryId</span><span class="sxs-lookup"><span data-stu-id="d7de0-153">groupPolicyCategoryId</span></span>|<span data-ttu-id="d7de0-154">Guid</span><span class="sxs-lookup"><span data-stu-id="d7de0-154">Guid</span></span>|<span data-ttu-id="d7de0-155">A ID de categoria da categoria pai</span><span class="sxs-lookup"><span data-stu-id="d7de0-155">The category id of the parent category</span></span>|
|<span data-ttu-id="d7de0-156">id</span><span class="sxs-lookup"><span data-stu-id="d7de0-156">id</span></span>|<span data-ttu-id="d7de0-157">String</span><span class="sxs-lookup"><span data-stu-id="d7de0-157">String</span></span>|<span data-ttu-id="d7de0-158">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d7de0-158">Key of the entity.</span></span>|
|<span data-ttu-id="d7de0-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7de0-159">lastModifiedDateTime</span></span>|<span data-ttu-id="d7de0-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7de0-160">DateTimeOffset</span></span>|<span data-ttu-id="d7de0-161">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d7de0-161">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="d7de0-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7de0-162">Response</span></span>
<span data-ttu-id="d7de0-163">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7de0-163">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7de0-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7de0-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7de0-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7de0-165">Request</span></span>
<span data-ttu-id="d7de0-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7de0-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d7de0-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7de0-167">Response</span></span>
<span data-ttu-id="d7de0-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7de0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




