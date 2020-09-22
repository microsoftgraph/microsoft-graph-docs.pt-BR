---
title: Atualizar groupPolicyDefinitionFile
description: Atualiza as propriedades de um objeto groupPolicyDefinitionFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 28387a3afdd8111cf8212ca9a52d923da3ae0b20
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48068249"
---
# <a name="update-grouppolicydefinitionfile"></a><span data-ttu-id="9cf51-103">Atualizar groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="9cf51-103">Update groupPolicyDefinitionFile</span></span>

<span data-ttu-id="9cf51-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cf51-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9cf51-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9cf51-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9cf51-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9cf51-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cf51-107">Atualiza as propriedades de um objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="9cf51-107">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9cf51-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9cf51-108">Prerequisites</span></span>
<span data-ttu-id="9cf51-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cf51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cf51-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9cf51-111">Permission type</span></span>|<span data-ttu-id="9cf51-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9cf51-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cf51-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9cf51-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9cf51-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cf51-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9cf51-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9cf51-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cf51-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cf51-116">Not supported.</span></span>|
|<span data-ttu-id="9cf51-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9cf51-117">Application</span></span>|<span data-ttu-id="9cf51-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cf51-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cf51-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9cf51-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/definitionFile
```

## <a name="request-headers"></a><span data-ttu-id="9cf51-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9cf51-120">Request headers</span></span>
|<span data-ttu-id="9cf51-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9cf51-121">Header</span></span>|<span data-ttu-id="9cf51-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9cf51-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9cf51-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9cf51-123">Authorization</span></span>|<span data-ttu-id="9cf51-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cf51-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9cf51-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9cf51-125">Accept</span></span>|<span data-ttu-id="9cf51-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9cf51-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cf51-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9cf51-127">Request body</span></span>
<span data-ttu-id="9cf51-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="9cf51-128">In the request body, supply a JSON representation for the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

<span data-ttu-id="9cf51-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span><span class="sxs-lookup"><span data-stu-id="9cf51-129">The following table shows the properties that are required when you create the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span></span>

|<span data-ttu-id="9cf51-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9cf51-130">Property</span></span>|<span data-ttu-id="9cf51-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cf51-131">Type</span></span>|<span data-ttu-id="9cf51-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cf51-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cf51-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9cf51-133">displayName</span></span>|<span data-ttu-id="9cf51-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9cf51-134">String</span></span>|<span data-ttu-id="9cf51-135">O nome amigável localizado do arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="9cf51-135">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="9cf51-136">description</span><span class="sxs-lookup"><span data-stu-id="9cf51-136">description</span></span>|<span data-ttu-id="9cf51-137">String</span><span class="sxs-lookup"><span data-stu-id="9cf51-137">String</span></span>|<span data-ttu-id="9cf51-138">A descrição localizada das configurações de política no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="9cf51-138">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="9cf51-139">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="9cf51-139">The default value is empty.</span></span>|
|<span data-ttu-id="9cf51-140">languageCodes</span><span class="sxs-lookup"><span data-stu-id="9cf51-140">languageCodes</span></span>|<span data-ttu-id="9cf51-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9cf51-141">String collection</span></span>|<span data-ttu-id="9cf51-142">Os códigos de idioma suportados para o arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="9cf51-142">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="9cf51-143">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="9cf51-143">targetPrefix</span></span>|<span data-ttu-id="9cf51-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9cf51-144">String</span></span>|<span data-ttu-id="9cf51-145">Especifica o nome lógico que se refere ao namespace dentro do arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="9cf51-145">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="9cf51-146">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="9cf51-146">targetNamespace</span></span>|<span data-ttu-id="9cf51-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9cf51-147">String</span></span>|<span data-ttu-id="9cf51-148">Especifica o URI usado para identificar o namespace no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="9cf51-148">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="9cf51-149">PolicyType</span><span class="sxs-lookup"><span data-stu-id="9cf51-149">policyType</span></span>|[<span data-ttu-id="9cf51-150">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="9cf51-150">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="9cf51-151">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="9cf51-151">Specifies the type of group policy.</span></span> <span data-ttu-id="9cf51-152">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="9cf51-152">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="9cf51-153">firmware</span><span class="sxs-lookup"><span data-stu-id="9cf51-153">revision</span></span>|<span data-ttu-id="9cf51-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9cf51-154">String</span></span>|<span data-ttu-id="9cf51-155">A versão de revisão associada ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="9cf51-155">The revision version associated with the file.</span></span>|
|<span data-ttu-id="9cf51-156">id</span><span class="sxs-lookup"><span data-stu-id="9cf51-156">id</span></span>|<span data-ttu-id="9cf51-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9cf51-157">String</span></span>|<span data-ttu-id="9cf51-158">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9cf51-158">Key of the entity.</span></span>|
|<span data-ttu-id="9cf51-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9cf51-159">lastModifiedDateTime</span></span>|<span data-ttu-id="9cf51-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9cf51-160">DateTimeOffset</span></span>|<span data-ttu-id="9cf51-161">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9cf51-161">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="9cf51-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cf51-162">Response</span></span>
<span data-ttu-id="9cf51-163">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9cf51-163">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cf51-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9cf51-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="9cf51-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9cf51-165">Request</span></span>
<span data-ttu-id="9cf51-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9cf51-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9cf51-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cf51-167">Response</span></span>
<span data-ttu-id="9cf51-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9cf51-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






