---
title: Atualizar groupPolicyDefinition
description: Atualize as propriedades de um objeto groupPolicyDefinition.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: eeb3e32f1870eac8491989426081df2ae41e4d42
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429019"
---
# <a name="update-grouppolicydefinition"></a><span data-ttu-id="6c83b-103">Atualizar groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="6c83b-103">Update groupPolicyDefinition</span></span>

> <span data-ttu-id="6c83b-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="6c83b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6c83b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6c83b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6c83b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="6c83b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c83b-107">Atualize as propriedades de um objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="6c83b-107">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c83b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6c83b-108">Prerequisites</span></span>
<span data-ttu-id="6c83b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6c83b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6c83b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c83b-111">Permission type</span></span>|<span data-ttu-id="6c83b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6c83b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c83b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c83b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6c83b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c83b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6c83b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c83b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c83b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c83b-116">Not supported.</span></span>|
|<span data-ttu-id="6c83b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c83b-117">Application</span></span>|<span data-ttu-id="6c83b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c83b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c83b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c83b-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="6c83b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c83b-120">Request headers</span></span>
|<span data-ttu-id="6c83b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6c83b-121">Header</span></span>|<span data-ttu-id="6c83b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6c83b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c83b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c83b-123">Authorization</span></span>|<span data-ttu-id="6c83b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c83b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c83b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6c83b-125">Accept</span></span>|<span data-ttu-id="6c83b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6c83b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c83b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c83b-127">Request body</span></span>
<span data-ttu-id="6c83b-128">No corpo da solicitação, fornece uma representação JSON para o objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="6c83b-128">In the request body, supply a JSON representation for the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

<span data-ttu-id="6c83b-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="6c83b-129">The following table shows the properties that are required when you create the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span>

|<span data-ttu-id="6c83b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c83b-130">Property</span></span>|<span data-ttu-id="6c83b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c83b-131">Type</span></span>|<span data-ttu-id="6c83b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c83b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c83b-133">classType</span><span class="sxs-lookup"><span data-stu-id="6c83b-133">classType</span></span>|[<span data-ttu-id="6c83b-134">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="6c83b-134">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="6c83b-135">Identifica o tipo dos grupos a que a diretiva pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="6c83b-135">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="6c83b-136">Os valores possíveis são: `user`, `machine`, `both`.</span><span class="sxs-lookup"><span data-stu-id="6c83b-136">Possible values are: `user`, `machine`, `both`.</span></span>|
|<span data-ttu-id="6c83b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="6c83b-137">displayName</span></span>|<span data-ttu-id="6c83b-138">String</span><span class="sxs-lookup"><span data-stu-id="6c83b-138">String</span></span>|<span data-ttu-id="6c83b-139">O nome da política localizado.</span><span class="sxs-lookup"><span data-stu-id="6c83b-139">The localized policy name.</span></span>|
|<span data-ttu-id="6c83b-140">explainText</span><span class="sxs-lookup"><span data-stu-id="6c83b-140">explainText</span></span>|<span data-ttu-id="6c83b-141">String</span><span class="sxs-lookup"><span data-stu-id="6c83b-141">String</span></span>|<span data-ttu-id="6c83b-142">A explicação ou ajuda texto localizado associado à política.</span><span class="sxs-lookup"><span data-stu-id="6c83b-142">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="6c83b-143">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="6c83b-143">The default value is empty.</span></span>|
|<span data-ttu-id="6c83b-144">categoryPath</span><span class="sxs-lookup"><span data-stu-id="6c83b-144">categoryPath</span></span>|<span data-ttu-id="6c83b-145">String</span><span class="sxs-lookup"><span data-stu-id="6c83b-145">String</span></span>|<span data-ttu-id="6c83b-146">O caminho de categoria completo localizado para a política.</span><span class="sxs-lookup"><span data-stu-id="6c83b-146">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="6c83b-147">supportedOn</span><span class="sxs-lookup"><span data-stu-id="6c83b-147">supportedOn</span></span>|<span data-ttu-id="6c83b-148">String</span><span class="sxs-lookup"><span data-stu-id="6c83b-148">String</span></span>|<span data-ttu-id="6c83b-149">A cadeia de caracteres localizada é usada para especificar qual sistema operacional ou a versão do aplicativo é afetada pela diretiva.</span><span class="sxs-lookup"><span data-stu-id="6c83b-149">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="6c83b-150">policyType</span><span class="sxs-lookup"><span data-stu-id="6c83b-150">policyType</span></span>|[<span data-ttu-id="6c83b-151">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="6c83b-151">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="6c83b-152">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="6c83b-152">Specifies the type of group policy.</span></span> <span data-ttu-id="6c83b-153">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="6c83b-153">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="6c83b-154">id</span><span class="sxs-lookup"><span data-stu-id="6c83b-154">id</span></span>|<span data-ttu-id="6c83b-155">String</span><span class="sxs-lookup"><span data-stu-id="6c83b-155">String</span></span>|<span data-ttu-id="6c83b-156">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6c83b-156">Key of the entity.</span></span>|
|<span data-ttu-id="6c83b-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c83b-157">lastModifiedDateTime</span></span>|<span data-ttu-id="6c83b-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c83b-158">DateTimeOffset</span></span>|<span data-ttu-id="6c83b-159">A data e hora que a entidade foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6c83b-159">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="6c83b-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c83b-160">Response</span></span>
<span data-ttu-id="6c83b-161">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c83b-161">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c83b-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c83b-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c83b-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c83b-163">Request</span></span>
<span data-ttu-id="6c83b-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c83b-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6c83b-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c83b-165">Response</span></span>
<span data-ttu-id="6c83b-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c83b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




