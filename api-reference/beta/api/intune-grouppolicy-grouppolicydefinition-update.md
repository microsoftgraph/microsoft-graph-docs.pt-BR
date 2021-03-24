---
title: Atualizar groupPolicyDefinition
description: Atualize as propriedades de um objeto groupPolicyDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 40012449a86324874251588dad27021e3e38fcec
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145744"
---
# <a name="update-grouppolicydefinition"></a><span data-ttu-id="91dad-103">Atualizar groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="91dad-103">Update groupPolicyDefinition</span></span>

<span data-ttu-id="91dad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91dad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91dad-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="91dad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91dad-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="91dad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91dad-107">Atualize as propriedades de [um objeto groupPolicyDefinition.](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="91dad-107">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91dad-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="91dad-108">Prerequisites</span></span>
<span data-ttu-id="91dad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91dad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91dad-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91dad-111">Permission type</span></span>|<span data-ttu-id="91dad-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91dad-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91dad-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91dad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="91dad-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91dad-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="91dad-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91dad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91dad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91dad-116">Not supported.</span></span>|
|<span data-ttu-id="91dad-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91dad-117">Application</span></span>|<span data-ttu-id="91dad-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91dad-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="91dad-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91dad-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="91dad-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91dad-120">Request headers</span></span>
|<span data-ttu-id="91dad-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="91dad-121">Header</span></span>|<span data-ttu-id="91dad-122">Valor</span><span class="sxs-lookup"><span data-stu-id="91dad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91dad-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="91dad-123">Authorization</span></span>|<span data-ttu-id="91dad-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91dad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91dad-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="91dad-125">Accept</span></span>|<span data-ttu-id="91dad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="91dad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91dad-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91dad-127">Request body</span></span>
<span data-ttu-id="91dad-128">No corpo da solicitação, fornece uma representação JSON para o [objeto groupPolicyDefinition.](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="91dad-128">In the request body, supply a JSON representation for the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

<span data-ttu-id="91dad-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="91dad-129">The following table shows the properties that are required when you create the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span>

|<span data-ttu-id="91dad-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91dad-130">Property</span></span>|<span data-ttu-id="91dad-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="91dad-131">Type</span></span>|<span data-ttu-id="91dad-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="91dad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91dad-133">classType</span><span class="sxs-lookup"><span data-stu-id="91dad-133">classType</span></span>|[<span data-ttu-id="91dad-134">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="91dad-134">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="91dad-135">Identifica o tipo de grupos aos qual a política pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="91dad-135">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="91dad-136">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="91dad-136">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="91dad-137">displayName</span><span class="sxs-lookup"><span data-stu-id="91dad-137">displayName</span></span>|<span data-ttu-id="91dad-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91dad-138">String</span></span>|<span data-ttu-id="91dad-139">O nome da política localizada.</span><span class="sxs-lookup"><span data-stu-id="91dad-139">The localized policy name.</span></span>|
|<span data-ttu-id="91dad-140">explainText</span><span class="sxs-lookup"><span data-stu-id="91dad-140">explainText</span></span>|<span data-ttu-id="91dad-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91dad-141">String</span></span>|<span data-ttu-id="91dad-142">A explicação localizada ou o texto de ajuda associado à política.</span><span class="sxs-lookup"><span data-stu-id="91dad-142">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="91dad-143">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="91dad-143">The default value is empty.</span></span>|
|<span data-ttu-id="91dad-144">categoryPath</span><span class="sxs-lookup"><span data-stu-id="91dad-144">categoryPath</span></span>|<span data-ttu-id="91dad-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91dad-145">String</span></span>|<span data-ttu-id="91dad-146">O caminho de categoria completa localizado para a política.</span><span class="sxs-lookup"><span data-stu-id="91dad-146">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="91dad-147">supportedOn</span><span class="sxs-lookup"><span data-stu-id="91dad-147">supportedOn</span></span>|<span data-ttu-id="91dad-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91dad-148">String</span></span>|<span data-ttu-id="91dad-149">Cadeia de caracteres localizada usada para especificar qual versão do sistema operacional ou aplicativo é afetada pela política.</span><span class="sxs-lookup"><span data-stu-id="91dad-149">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="91dad-150">policyType</span><span class="sxs-lookup"><span data-stu-id="91dad-150">policyType</span></span>|[<span data-ttu-id="91dad-151">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="91dad-151">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="91dad-152">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="91dad-152">Specifies the type of group policy.</span></span> <span data-ttu-id="91dad-153">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="91dad-153">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="91dad-154">groupPolicyCategoryId</span><span class="sxs-lookup"><span data-stu-id="91dad-154">groupPolicyCategoryId</span></span>|<span data-ttu-id="91dad-155">Guid</span><span class="sxs-lookup"><span data-stu-id="91dad-155">Guid</span></span>|<span data-ttu-id="91dad-156">A id de categoria da categoria pai</span><span class="sxs-lookup"><span data-stu-id="91dad-156">The category id of the parent category</span></span>|
|<span data-ttu-id="91dad-157">id</span><span class="sxs-lookup"><span data-stu-id="91dad-157">id</span></span>|<span data-ttu-id="91dad-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91dad-158">String</span></span>|<span data-ttu-id="91dad-159">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="91dad-159">Key of the entity.</span></span>|
|<span data-ttu-id="91dad-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="91dad-160">lastModifiedDateTime</span></span>|<span data-ttu-id="91dad-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91dad-161">DateTimeOffset</span></span>|<span data-ttu-id="91dad-162">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="91dad-162">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="91dad-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="91dad-163">Response</span></span>
<span data-ttu-id="91dad-164">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91dad-164">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91dad-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91dad-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="91dad-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91dad-166">Request</span></span>
<span data-ttu-id="91dad-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91dad-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="91dad-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="91dad-168">Response</span></span>
<span data-ttu-id="91dad-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91dad-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




