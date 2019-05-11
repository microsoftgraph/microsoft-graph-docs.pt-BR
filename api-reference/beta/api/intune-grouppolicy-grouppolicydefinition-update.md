---
title: Atualizar groupPolicyDefinition
description: Atualiza as propriedades de um objeto groupPolicyDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cf706f941ef7535bbd0a89d3d126790e44d95853
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33905116"
---
# <a name="update-grouppolicydefinition"></a><span data-ttu-id="3e388-103">Atualizar groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="3e388-103">Update groupPolicyDefinition</span></span>

> <span data-ttu-id="3e388-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3e388-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e388-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3e388-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e388-106">Atualiza as propriedades de um objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="3e388-106">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e388-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3e388-107">Prerequisites</span></span>
<span data-ttu-id="3e388-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e388-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e388-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e388-110">Permission type</span></span>|<span data-ttu-id="3e388-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3e388-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e388-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e388-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3e388-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e388-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3e388-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e388-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e388-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e388-115">Not supported.</span></span>|
|<span data-ttu-id="3e388-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e388-116">Application</span></span>|<span data-ttu-id="3e388-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e388-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e388-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e388-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="3e388-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e388-119">Request headers</span></span>
|<span data-ttu-id="3e388-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3e388-120">Header</span></span>|<span data-ttu-id="3e388-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3e388-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e388-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e388-122">Authorization</span></span>|<span data-ttu-id="3e388-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e388-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e388-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3e388-124">Accept</span></span>|<span data-ttu-id="3e388-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3e388-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e388-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e388-126">Request body</span></span>
<span data-ttu-id="3e388-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="3e388-127">In the request body, supply a JSON representation for the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

<span data-ttu-id="3e388-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3e388-128">The following table shows the properties that are required when you create the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span>

|<span data-ttu-id="3e388-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e388-129">Property</span></span>|<span data-ttu-id="3e388-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e388-130">Type</span></span>|<span data-ttu-id="3e388-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e388-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e388-132">classType</span><span class="sxs-lookup"><span data-stu-id="3e388-132">classType</span></span>|[<span data-ttu-id="3e388-133">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="3e388-133">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="3e388-134">Identifica o tipo de grupo ao qual a política pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="3e388-134">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="3e388-135">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="3e388-135">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="3e388-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3e388-136">displayName</span></span>|<span data-ttu-id="3e388-137">String</span><span class="sxs-lookup"><span data-stu-id="3e388-137">String</span></span>|<span data-ttu-id="3e388-138">O nome da política localizada.</span><span class="sxs-lookup"><span data-stu-id="3e388-138">The localized policy name.</span></span>|
|<span data-ttu-id="3e388-139">Texto não criptografado</span><span class="sxs-lookup"><span data-stu-id="3e388-139">explainText</span></span>|<span data-ttu-id="3e388-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e388-140">String</span></span>|<span data-ttu-id="3e388-141">A explicação localizada ou o texto de ajuda associado à política.</span><span class="sxs-lookup"><span data-stu-id="3e388-141">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="3e388-142">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="3e388-142">The default value is empty.</span></span>|
|<span data-ttu-id="3e388-143">categoryPath</span><span class="sxs-lookup"><span data-stu-id="3e388-143">categoryPath</span></span>|<span data-ttu-id="3e388-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e388-144">String</span></span>|<span data-ttu-id="3e388-145">O caminho de categoria completo localizado para a política.</span><span class="sxs-lookup"><span data-stu-id="3e388-145">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="3e388-146">com suporte</span><span class="sxs-lookup"><span data-stu-id="3e388-146">supportedOn</span></span>|<span data-ttu-id="3e388-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e388-147">String</span></span>|<span data-ttu-id="3e388-148">Cadeia de caracteres localizada usada para especificar o sistema operacional ou a versão do aplicativo é afetada pela política.</span><span class="sxs-lookup"><span data-stu-id="3e388-148">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="3e388-149">PolicyType</span><span class="sxs-lookup"><span data-stu-id="3e388-149">policyType</span></span>|[<span data-ttu-id="3e388-150">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="3e388-150">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="3e388-151">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="3e388-151">Specifies the type of group policy.</span></span> <span data-ttu-id="3e388-152">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="3e388-152">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="3e388-153">id</span><span class="sxs-lookup"><span data-stu-id="3e388-153">id</span></span>|<span data-ttu-id="3e388-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e388-154">String</span></span>|<span data-ttu-id="3e388-155">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3e388-155">Key of the entity.</span></span>|
|<span data-ttu-id="3e388-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e388-156">lastModifiedDateTime</span></span>|<span data-ttu-id="3e388-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e388-157">DateTimeOffset</span></span>|<span data-ttu-id="3e388-158">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3e388-158">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="3e388-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e388-159">Response</span></span>
<span data-ttu-id="3e388-160">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e388-160">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e388-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e388-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e388-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e388-162">Request</span></span>
<span data-ttu-id="3e388-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e388-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3e388-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e388-164">Response</span></span>
<span data-ttu-id="3e388-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e388-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




