---
title: Atualizar groupPolicyDefinitionFile
description: Atualize as propriedades de um objeto groupPolicyDefinitionFile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be713dba2d503f19cd565fe5e53d252ed20667e0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429171"
---
# <a name="update-grouppolicydefinitionfile"></a><span data-ttu-id="c5173-103">Atualizar groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="c5173-103">Update groupPolicyDefinitionFile</span></span>

> <span data-ttu-id="c5173-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="c5173-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c5173-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c5173-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5173-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="c5173-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5173-107">Atualize as propriedades de um objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="c5173-107">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5173-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c5173-108">Prerequisites</span></span>
<span data-ttu-id="c5173-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c5173-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c5173-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5173-111">Permission type</span></span>|<span data-ttu-id="c5173-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c5173-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5173-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5173-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5173-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5173-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c5173-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5173-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5173-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5173-116">Not supported.</span></span>|
|<span data-ttu-id="c5173-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5173-117">Application</span></span>|<span data-ttu-id="c5173-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5173-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5173-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5173-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile
```

## <a name="request-headers"></a><span data-ttu-id="c5173-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5173-120">Request headers</span></span>
|<span data-ttu-id="c5173-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c5173-121">Header</span></span>|<span data-ttu-id="c5173-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c5173-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5173-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5173-123">Authorization</span></span>|<span data-ttu-id="c5173-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5173-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5173-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c5173-125">Accept</span></span>|<span data-ttu-id="c5173-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5173-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5173-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5173-127">Request body</span></span>
<span data-ttu-id="c5173-128">No corpo da solicitação, fornece uma representação JSON para o objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="c5173-128">In the request body, supply a JSON representation for the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

<span data-ttu-id="c5173-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span><span class="sxs-lookup"><span data-stu-id="c5173-129">The following table shows the properties that are required when you create the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span></span>

|<span data-ttu-id="c5173-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5173-130">Property</span></span>|<span data-ttu-id="c5173-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5173-131">Type</span></span>|<span data-ttu-id="c5173-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5173-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5173-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c5173-133">displayName</span></span>|<span data-ttu-id="c5173-134">String</span><span class="sxs-lookup"><span data-stu-id="c5173-134">String</span></span>|<span data-ttu-id="c5173-135">O nome amigável localizado do arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="c5173-135">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="c5173-136">description</span><span class="sxs-lookup"><span data-stu-id="c5173-136">description</span></span>|<span data-ttu-id="c5173-137">String</span><span class="sxs-lookup"><span data-stu-id="c5173-137">String</span></span>|<span data-ttu-id="c5173-138">A descrição localizada das configurações de política no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="c5173-138">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="c5173-139">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="c5173-139">The default value is empty.</span></span>|
|<span data-ttu-id="c5173-140">languageCodes</span><span class="sxs-lookup"><span data-stu-id="c5173-140">languageCodes</span></span>|<span data-ttu-id="c5173-141">String collection</span><span class="sxs-lookup"><span data-stu-id="c5173-141">String collection</span></span>|<span data-ttu-id="c5173-142">Os códigos de idioma com suporte para o arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="c5173-142">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="c5173-143">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="c5173-143">targetPrefix</span></span>|<span data-ttu-id="c5173-144">String</span><span class="sxs-lookup"><span data-stu-id="c5173-144">String</span></span>|<span data-ttu-id="c5173-145">Especifica o nome lógico que se refere ao namespace no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="c5173-145">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="c5173-146">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="c5173-146">targetNamespace</span></span>|<span data-ttu-id="c5173-147">String</span><span class="sxs-lookup"><span data-stu-id="c5173-147">String</span></span>|<span data-ttu-id="c5173-148">Especifica o URI usado para identificar o namespace no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="c5173-148">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="c5173-149">policyType</span><span class="sxs-lookup"><span data-stu-id="c5173-149">policyType</span></span>|[<span data-ttu-id="c5173-150">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="c5173-150">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="c5173-151">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="c5173-151">Specifies the type of group policy.</span></span> <span data-ttu-id="c5173-152">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="c5173-152">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="c5173-153">id</span><span class="sxs-lookup"><span data-stu-id="c5173-153">id</span></span>|<span data-ttu-id="c5173-154">String</span><span class="sxs-lookup"><span data-stu-id="c5173-154">String</span></span>|<span data-ttu-id="c5173-155">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c5173-155">Key of the entity.</span></span>|
|<span data-ttu-id="c5173-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5173-156">lastModifiedDateTime</span></span>|<span data-ttu-id="c5173-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5173-157">DateTimeOffset</span></span>|<span data-ttu-id="c5173-158">A data e hora que a entidade foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="c5173-158">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="c5173-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5173-159">Response</span></span>
<span data-ttu-id="c5173-160">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5173-160">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5173-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5173-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5173-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5173-162">Request</span></span>
<span data-ttu-id="c5173-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5173-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested"
}
```

### <a name="response"></a><span data-ttu-id="c5173-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5173-164">Response</span></span>
<span data-ttu-id="c5173-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5173-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 438

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested",
  "id": "940aa2a1-a2a1-940a-a1a2-0a94a1a20a94",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




