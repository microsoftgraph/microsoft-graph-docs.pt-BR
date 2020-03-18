---
title: Atualizar groupPolicyDefinitionFile
description: Atualiza as propriedades de um objeto groupPolicyDefinitionFile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ba9ce04ba17290d6240b52e780a4728f9f12ca8d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804412"
---
# <a name="update-grouppolicydefinitionfile"></a><span data-ttu-id="2f9ca-103">Atualizar groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="2f9ca-103">Update groupPolicyDefinitionFile</span></span>

> <span data-ttu-id="2f9ca-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2f9ca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f9ca-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f9ca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f9ca-106">Atualiza as propriedades de um objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="2f9ca-106">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f9ca-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f9ca-107">Prerequisites</span></span>
<span data-ttu-id="2f9ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f9ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f9ca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f9ca-110">Permission type</span></span>|<span data-ttu-id="2f9ca-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f9ca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f9ca-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f9ca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f9ca-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f9ca-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2f9ca-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f9ca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f9ca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f9ca-115">Not supported.</span></span>|
|<span data-ttu-id="2f9ca-116">Application</span><span class="sxs-lookup"><span data-stu-id="2f9ca-116">Application</span></span>|<span data-ttu-id="2f9ca-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f9ca-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f9ca-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f9ca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/definitionFile
```

## <a name="request-headers"></a><span data-ttu-id="2f9ca-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f9ca-119">Request headers</span></span>
|<span data-ttu-id="2f9ca-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f9ca-120">Header</span></span>|<span data-ttu-id="2f9ca-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2f9ca-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f9ca-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f9ca-122">Authorization</span></span>|<span data-ttu-id="2f9ca-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f9ca-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f9ca-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f9ca-124">Accept</span></span>|<span data-ttu-id="2f9ca-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f9ca-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f9ca-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f9ca-126">Request body</span></span>
<span data-ttu-id="2f9ca-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="2f9ca-127">In the request body, supply a JSON representation for the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

<span data-ttu-id="2f9ca-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span><span class="sxs-lookup"><span data-stu-id="2f9ca-128">The following table shows the properties that are required when you create the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span></span>

|<span data-ttu-id="2f9ca-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f9ca-129">Property</span></span>|<span data-ttu-id="2f9ca-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f9ca-130">Type</span></span>|<span data-ttu-id="2f9ca-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f9ca-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f9ca-132">displayName</span><span class="sxs-lookup"><span data-stu-id="2f9ca-132">displayName</span></span>|<span data-ttu-id="2f9ca-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f9ca-133">String</span></span>|<span data-ttu-id="2f9ca-134">O nome amigável localizado do arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="2f9ca-134">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="2f9ca-135">description</span><span class="sxs-lookup"><span data-stu-id="2f9ca-135">description</span></span>|<span data-ttu-id="2f9ca-136">String</span><span class="sxs-lookup"><span data-stu-id="2f9ca-136">String</span></span>|<span data-ttu-id="2f9ca-137">A descrição localizada das configurações de política no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="2f9ca-137">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="2f9ca-138">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="2f9ca-138">The default value is empty.</span></span>|
|<span data-ttu-id="2f9ca-139">languageCodes</span><span class="sxs-lookup"><span data-stu-id="2f9ca-139">languageCodes</span></span>|<span data-ttu-id="2f9ca-140">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f9ca-140">String collection</span></span>|<span data-ttu-id="2f9ca-141">Os códigos de idioma suportados para o arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="2f9ca-141">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="2f9ca-142">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="2f9ca-142">targetPrefix</span></span>|<span data-ttu-id="2f9ca-143">String</span><span class="sxs-lookup"><span data-stu-id="2f9ca-143">String</span></span>|<span data-ttu-id="2f9ca-144">Especifica o nome lógico que se refere ao namespace dentro do arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="2f9ca-144">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="2f9ca-145">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="2f9ca-145">targetNamespace</span></span>|<span data-ttu-id="2f9ca-146">String</span><span class="sxs-lookup"><span data-stu-id="2f9ca-146">String</span></span>|<span data-ttu-id="2f9ca-147">Especifica o URI usado para identificar o namespace no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="2f9ca-147">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="2f9ca-148">PolicyType</span><span class="sxs-lookup"><span data-stu-id="2f9ca-148">policyType</span></span>|[<span data-ttu-id="2f9ca-149">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="2f9ca-149">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="2f9ca-150">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="2f9ca-150">Specifies the type of group policy.</span></span> <span data-ttu-id="2f9ca-151">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="2f9ca-151">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="2f9ca-152">firmware</span><span class="sxs-lookup"><span data-stu-id="2f9ca-152">revision</span></span>|<span data-ttu-id="2f9ca-153">String</span><span class="sxs-lookup"><span data-stu-id="2f9ca-153">String</span></span>|<span data-ttu-id="2f9ca-154">A versão de revisão associada ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="2f9ca-154">The revision version associated with the file.</span></span>|
|<span data-ttu-id="2f9ca-155">id</span><span class="sxs-lookup"><span data-stu-id="2f9ca-155">id</span></span>|<span data-ttu-id="2f9ca-156">String</span><span class="sxs-lookup"><span data-stu-id="2f9ca-156">String</span></span>|<span data-ttu-id="2f9ca-157">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2f9ca-157">Key of the entity.</span></span>|
|<span data-ttu-id="2f9ca-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f9ca-158">lastModifiedDateTime</span></span>|<span data-ttu-id="2f9ca-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f9ca-159">DateTimeOffset</span></span>|<span data-ttu-id="2f9ca-160">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2f9ca-160">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="2f9ca-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f9ca-161">Response</span></span>
<span data-ttu-id="2f9ca-162">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f9ca-162">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f9ca-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f9ca-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f9ca-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f9ca-164">Request</span></span>
<span data-ttu-id="2f9ca-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f9ca-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
Content-type: application/json
Content-length: 358

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
  "revision": "Revision value"
}
```

### <a name="response"></a><span data-ttu-id="2f9ca-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f9ca-166">Response</span></span>
<span data-ttu-id="2f9ca-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f9ca-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 471

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
  "revision": "Revision value",
  "id": "940aa2a1-a2a1-940a-a1a2-0a94a1a20a94",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




