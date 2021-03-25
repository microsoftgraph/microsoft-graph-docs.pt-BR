---
title: Atualizar groupPolicyDefinitionFile
description: Atualize as propriedades de um objeto groupPolicyDefinitionFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0910406f564f86decf211285ed472f57792267c5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158889"
---
# <a name="update-grouppolicydefinitionfile"></a><span data-ttu-id="05401-103">Atualizar groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="05401-103">Update groupPolicyDefinitionFile</span></span>

<span data-ttu-id="05401-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05401-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05401-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="05401-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05401-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="05401-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05401-107">Atualize as propriedades de [um objeto groupPolicyDefinitionFile.](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="05401-107">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05401-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="05401-108">Prerequisites</span></span>
<span data-ttu-id="05401-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05401-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05401-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05401-111">Permission type</span></span>|<span data-ttu-id="05401-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="05401-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05401-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05401-113">Delegated (work or school account)</span></span>|<span data-ttu-id="05401-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05401-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="05401-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05401-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05401-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05401-116">Not supported.</span></span>|
|<span data-ttu-id="05401-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05401-117">Application</span></span>|<span data-ttu-id="05401-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05401-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05401-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05401-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/definitionFile
```

## <a name="request-headers"></a><span data-ttu-id="05401-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05401-120">Request headers</span></span>
|<span data-ttu-id="05401-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="05401-121">Header</span></span>|<span data-ttu-id="05401-122">Valor</span><span class="sxs-lookup"><span data-stu-id="05401-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05401-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="05401-123">Authorization</span></span>|<span data-ttu-id="05401-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05401-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05401-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="05401-125">Accept</span></span>|<span data-ttu-id="05401-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05401-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05401-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05401-127">Request body</span></span>
<span data-ttu-id="05401-128">No corpo da solicitação, fornece uma representação JSON para o [objeto groupPolicyDefinitionFile.](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="05401-128">In the request body, supply a JSON representation for the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

<span data-ttu-id="05401-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span><span class="sxs-lookup"><span data-stu-id="05401-129">The following table shows the properties that are required when you create the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span></span>

|<span data-ttu-id="05401-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05401-130">Property</span></span>|<span data-ttu-id="05401-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="05401-131">Type</span></span>|<span data-ttu-id="05401-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="05401-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05401-133">displayName</span><span class="sxs-lookup"><span data-stu-id="05401-133">displayName</span></span>|<span data-ttu-id="05401-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05401-134">String</span></span>|<span data-ttu-id="05401-135">O nome amigável localizado do arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="05401-135">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="05401-136">descrição</span><span class="sxs-lookup"><span data-stu-id="05401-136">description</span></span>|<span data-ttu-id="05401-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05401-137">String</span></span>|<span data-ttu-id="05401-138">A descrição localizada das configurações de política no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="05401-138">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="05401-139">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="05401-139">The default value is empty.</span></span>|
|<span data-ttu-id="05401-140">languageCodes</span><span class="sxs-lookup"><span data-stu-id="05401-140">languageCodes</span></span>|<span data-ttu-id="05401-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="05401-141">String collection</span></span>|<span data-ttu-id="05401-142">Os códigos de idioma com suporte para o arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="05401-142">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="05401-143">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="05401-143">targetPrefix</span></span>|<span data-ttu-id="05401-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05401-144">String</span></span>|<span data-ttu-id="05401-145">Especifica o nome lógico que se refere ao namespace no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="05401-145">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="05401-146">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="05401-146">targetNamespace</span></span>|<span data-ttu-id="05401-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05401-147">String</span></span>|<span data-ttu-id="05401-148">Especifica o URI usado para identificar o namespace no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="05401-148">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="05401-149">policyType</span><span class="sxs-lookup"><span data-stu-id="05401-149">policyType</span></span>|[<span data-ttu-id="05401-150">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="05401-150">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="05401-151">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="05401-151">Specifies the type of group policy.</span></span> <span data-ttu-id="05401-152">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="05401-152">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="05401-153">revision</span><span class="sxs-lookup"><span data-stu-id="05401-153">revision</span></span>|<span data-ttu-id="05401-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05401-154">String</span></span>|<span data-ttu-id="05401-155">A versão de revisão associada ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="05401-155">The revision version associated with the file.</span></span>|
|<span data-ttu-id="05401-156">id</span><span class="sxs-lookup"><span data-stu-id="05401-156">id</span></span>|<span data-ttu-id="05401-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05401-157">String</span></span>|<span data-ttu-id="05401-158">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="05401-158">Key of the entity.</span></span>|
|<span data-ttu-id="05401-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="05401-159">lastModifiedDateTime</span></span>|<span data-ttu-id="05401-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05401-160">DateTimeOffset</span></span>|<span data-ttu-id="05401-161">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="05401-161">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="05401-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="05401-162">Response</span></span>
<span data-ttu-id="05401-163">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05401-163">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05401-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05401-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="05401-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05401-165">Request</span></span>
<span data-ttu-id="05401-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05401-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="05401-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="05401-167">Response</span></span>
<span data-ttu-id="05401-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05401-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




