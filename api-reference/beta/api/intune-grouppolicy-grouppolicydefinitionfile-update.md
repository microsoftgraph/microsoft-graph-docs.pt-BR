---
title: Atualizar groupPolicyDefinitionFile
description: Atualiza as propriedades de um objeto groupPolicyDefinitionFile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dbcaaa6cd8689f039d9daeb7b4ad7f83f2276783
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33905095"
---
# <a name="update-grouppolicydefinitionfile"></a><span data-ttu-id="2f564-103">Atualizar groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="2f564-103">Update groupPolicyDefinitionFile</span></span>

> <span data-ttu-id="2f564-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2f564-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f564-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f564-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f564-106">Atualiza as propriedades de um objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="2f564-106">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f564-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f564-107">Prerequisites</span></span>
<span data-ttu-id="2f564-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f564-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f564-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f564-110">Permission type</span></span>|<span data-ttu-id="2f564-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f564-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f564-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f564-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f564-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f564-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2f564-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f564-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f564-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f564-115">Not supported.</span></span>|
|<span data-ttu-id="2f564-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f564-116">Application</span></span>|<span data-ttu-id="2f564-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f564-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f564-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f564-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile
```

## <a name="request-headers"></a><span data-ttu-id="2f564-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f564-119">Request headers</span></span>
|<span data-ttu-id="2f564-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f564-120">Header</span></span>|<span data-ttu-id="2f564-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2f564-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f564-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f564-122">Authorization</span></span>|<span data-ttu-id="2f564-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f564-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f564-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f564-124">Accept</span></span>|<span data-ttu-id="2f564-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f564-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f564-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f564-126">Request body</span></span>
<span data-ttu-id="2f564-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="2f564-127">In the request body, supply a JSON representation for the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

<span data-ttu-id="2f564-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span><span class="sxs-lookup"><span data-stu-id="2f564-128">The following table shows the properties that are required when you create the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span></span>

|<span data-ttu-id="2f564-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f564-129">Property</span></span>|<span data-ttu-id="2f564-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f564-130">Type</span></span>|<span data-ttu-id="2f564-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f564-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f564-132">displayName</span><span class="sxs-lookup"><span data-stu-id="2f564-132">displayName</span></span>|<span data-ttu-id="2f564-133">String</span><span class="sxs-lookup"><span data-stu-id="2f564-133">String</span></span>|<span data-ttu-id="2f564-134">O nome amigável localizado do arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="2f564-134">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="2f564-135">description</span><span class="sxs-lookup"><span data-stu-id="2f564-135">description</span></span>|<span data-ttu-id="2f564-136">String</span><span class="sxs-lookup"><span data-stu-id="2f564-136">String</span></span>|<span data-ttu-id="2f564-137">A descrição localizada das configurações de política no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="2f564-137">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="2f564-138">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="2f564-138">The default value is empty.</span></span>|
|<span data-ttu-id="2f564-139">languageCodes</span><span class="sxs-lookup"><span data-stu-id="2f564-139">languageCodes</span></span>|<span data-ttu-id="2f564-140">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f564-140">String collection</span></span>|<span data-ttu-id="2f564-141">Os códigos de idioma suportados para o arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="2f564-141">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="2f564-142">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="2f564-142">targetPrefix</span></span>|<span data-ttu-id="2f564-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f564-143">String</span></span>|<span data-ttu-id="2f564-144">Especifica o nome lógico que se refere ao namespace dentro do arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="2f564-144">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="2f564-145">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="2f564-145">targetNamespace</span></span>|<span data-ttu-id="2f564-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f564-146">String</span></span>|<span data-ttu-id="2f564-147">Especifica o URI usado para identificar o namespace no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="2f564-147">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="2f564-148">PolicyType</span><span class="sxs-lookup"><span data-stu-id="2f564-148">policyType</span></span>|[<span data-ttu-id="2f564-149">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="2f564-149">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="2f564-150">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="2f564-150">Specifies the type of group policy.</span></span> <span data-ttu-id="2f564-151">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="2f564-151">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="2f564-152">id</span><span class="sxs-lookup"><span data-stu-id="2f564-152">id</span></span>|<span data-ttu-id="2f564-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f564-153">String</span></span>|<span data-ttu-id="2f564-154">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2f564-154">Key of the entity.</span></span>|
|<span data-ttu-id="2f564-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f564-155">lastModifiedDateTime</span></span>|<span data-ttu-id="2f564-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f564-156">DateTimeOffset</span></span>|<span data-ttu-id="2f564-157">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2f564-157">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="2f564-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f564-158">Response</span></span>
<span data-ttu-id="2f564-159">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f564-159">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f564-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f564-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f564-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f564-161">Request</span></span>
<span data-ttu-id="2f564-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f564-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2f564-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f564-163">Response</span></span>
<span data-ttu-id="2f564-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f564-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




