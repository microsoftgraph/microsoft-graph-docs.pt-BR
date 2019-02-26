---
title: Atualizar groupPolicyDefinition
description: Atualiza as propriedades de um objeto groupPolicyDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3439c14463118f616847dd5e7f71970fa3d6a8c7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157250"
---
# <a name="update-grouppolicydefinition"></a><span data-ttu-id="2145e-103">Atualizar groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="2145e-103">Update groupPolicyDefinition</span></span>

> <span data-ttu-id="2145e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2145e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2145e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2145e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2145e-106">Atualiza as propriedades de um objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="2145e-106">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2145e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2145e-107">Prerequisites</span></span>
<span data-ttu-id="2145e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2145e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2145e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2145e-110">Permission type</span></span>|<span data-ttu-id="2145e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2145e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2145e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2145e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2145e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2145e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2145e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2145e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2145e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2145e-115">Not supported.</span></span>|
|<span data-ttu-id="2145e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2145e-116">Application</span></span>|<span data-ttu-id="2145e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2145e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2145e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2145e-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="2145e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2145e-119">Request headers</span></span>
|<span data-ttu-id="2145e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2145e-120">Header</span></span>|<span data-ttu-id="2145e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2145e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2145e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2145e-122">Authorization</span></span>|<span data-ttu-id="2145e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2145e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2145e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2145e-124">Accept</span></span>|<span data-ttu-id="2145e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2145e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2145e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2145e-126">Request body</span></span>
<span data-ttu-id="2145e-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="2145e-127">In the request body, supply a JSON representation for the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

<span data-ttu-id="2145e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="2145e-128">The following table shows the properties that are required when you create the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span>

|<span data-ttu-id="2145e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2145e-129">Property</span></span>|<span data-ttu-id="2145e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2145e-130">Type</span></span>|<span data-ttu-id="2145e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2145e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2145e-132">classType</span><span class="sxs-lookup"><span data-stu-id="2145e-132">classType</span></span>|[<span data-ttu-id="2145e-133">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="2145e-133">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="2145e-134">Identifica o tipo de grupo ao qual a política pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="2145e-134">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="2145e-135">Os valores possíveis são: `user`, `machine`, `both`.</span><span class="sxs-lookup"><span data-stu-id="2145e-135">Possible values are: `user`, `machine`, `both`.</span></span>|
|<span data-ttu-id="2145e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2145e-136">displayName</span></span>|<span data-ttu-id="2145e-137">String</span><span class="sxs-lookup"><span data-stu-id="2145e-137">String</span></span>|<span data-ttu-id="2145e-138">O nome da política localizada.</span><span class="sxs-lookup"><span data-stu-id="2145e-138">The localized policy name.</span></span>|
|<span data-ttu-id="2145e-139">Texto não criptografado</span><span class="sxs-lookup"><span data-stu-id="2145e-139">explainText</span></span>|<span data-ttu-id="2145e-140">String</span><span class="sxs-lookup"><span data-stu-id="2145e-140">String</span></span>|<span data-ttu-id="2145e-141">A explicação localizada ou o texto de ajuda associado à política.</span><span class="sxs-lookup"><span data-stu-id="2145e-141">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="2145e-142">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="2145e-142">The default value is empty.</span></span>|
|<span data-ttu-id="2145e-143">categoryPath</span><span class="sxs-lookup"><span data-stu-id="2145e-143">categoryPath</span></span>|<span data-ttu-id="2145e-144">String</span><span class="sxs-lookup"><span data-stu-id="2145e-144">String</span></span>|<span data-ttu-id="2145e-145">O caminho de categoria completo localizado para a política.</span><span class="sxs-lookup"><span data-stu-id="2145e-145">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="2145e-146">com suporte</span><span class="sxs-lookup"><span data-stu-id="2145e-146">supportedOn</span></span>|<span data-ttu-id="2145e-147">String</span><span class="sxs-lookup"><span data-stu-id="2145e-147">String</span></span>|<span data-ttu-id="2145e-148">Cadeia de caracteres localizada usada para especificar o sistema operacional ou a versão do aplicativo é afetada pela política.</span><span class="sxs-lookup"><span data-stu-id="2145e-148">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="2145e-149">PolicyType</span><span class="sxs-lookup"><span data-stu-id="2145e-149">policyType</span></span>|[<span data-ttu-id="2145e-150">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="2145e-150">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="2145e-151">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="2145e-151">Specifies the type of group policy.</span></span> <span data-ttu-id="2145e-152">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="2145e-152">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="2145e-153">id</span><span class="sxs-lookup"><span data-stu-id="2145e-153">id</span></span>|<span data-ttu-id="2145e-154">String</span><span class="sxs-lookup"><span data-stu-id="2145e-154">String</span></span>|<span data-ttu-id="2145e-155">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2145e-155">Key of the entity.</span></span>|
|<span data-ttu-id="2145e-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2145e-156">lastModifiedDateTime</span></span>|<span data-ttu-id="2145e-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2145e-157">DateTimeOffset</span></span>|<span data-ttu-id="2145e-158">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2145e-158">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="2145e-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="2145e-159">Response</span></span>
<span data-ttu-id="2145e-160">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2145e-160">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2145e-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2145e-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="2145e-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2145e-162">Request</span></span>
<span data-ttu-id="2145e-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2145e-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2145e-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="2145e-164">Response</span></span>
<span data-ttu-id="2145e-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2145e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




