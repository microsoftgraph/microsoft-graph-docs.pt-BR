---
title: Atualizar groupPolicyDefinitionFile
description: Atualiza as propriedades de um objeto groupPolicyDefinitionFile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8343106ee53e4e2e038200cd897224d9a0d9d18f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721980"
---
# <a name="update-grouppolicydefinitionfile"></a><span data-ttu-id="3dca4-103">Atualizar groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="3dca4-103">Update groupPolicyDefinitionFile</span></span>

> <span data-ttu-id="3dca4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3dca4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3dca4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3dca4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3dca4-106">Atualiza as propriedades de um objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="3dca4-106">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3dca4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3dca4-107">Prerequisites</span></span>
<span data-ttu-id="3dca4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3dca4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3dca4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3dca4-110">Permission type</span></span>|<span data-ttu-id="3dca4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3dca4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3dca4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3dca4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3dca4-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dca4-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3dca4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3dca4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3dca4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3dca4-115">Not supported.</span></span>|
|<span data-ttu-id="3dca4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3dca4-116">Application</span></span>|<span data-ttu-id="3dca4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3dca4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3dca4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3dca4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile
```

## <a name="request-headers"></a><span data-ttu-id="3dca4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3dca4-119">Request headers</span></span>
|<span data-ttu-id="3dca4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3dca4-120">Header</span></span>|<span data-ttu-id="3dca4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3dca4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3dca4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3dca4-122">Authorization</span></span>|<span data-ttu-id="3dca4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3dca4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3dca4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3dca4-124">Accept</span></span>|<span data-ttu-id="3dca4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3dca4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3dca4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3dca4-126">Request body</span></span>
<span data-ttu-id="3dca4-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="3dca4-127">In the request body, supply a JSON representation for the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

<span data-ttu-id="3dca4-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span><span class="sxs-lookup"><span data-stu-id="3dca4-128">The following table shows the properties that are required when you create the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span></span>

|<span data-ttu-id="3dca4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3dca4-129">Property</span></span>|<span data-ttu-id="3dca4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3dca4-130">Type</span></span>|<span data-ttu-id="3dca4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3dca4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3dca4-132">displayName</span><span class="sxs-lookup"><span data-stu-id="3dca4-132">displayName</span></span>|<span data-ttu-id="3dca4-133">String</span><span class="sxs-lookup"><span data-stu-id="3dca4-133">String</span></span>|<span data-ttu-id="3dca4-134">O nome amigável localizado do arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="3dca4-134">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="3dca4-135">descrição</span><span class="sxs-lookup"><span data-stu-id="3dca4-135">description</span></span>|<span data-ttu-id="3dca4-136">String</span><span class="sxs-lookup"><span data-stu-id="3dca4-136">String</span></span>|<span data-ttu-id="3dca4-137">A descrição localizada das configurações de política no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="3dca4-137">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="3dca4-138">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="3dca4-138">The default value is empty.</span></span>|
|<span data-ttu-id="3dca4-139">languageCodes</span><span class="sxs-lookup"><span data-stu-id="3dca4-139">languageCodes</span></span>|<span data-ttu-id="3dca4-140">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3dca4-140">String collection</span></span>|<span data-ttu-id="3dca4-141">Os códigos de idioma suportados para o arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="3dca4-141">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="3dca4-142">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="3dca4-142">targetPrefix</span></span>|<span data-ttu-id="3dca4-143">String</span><span class="sxs-lookup"><span data-stu-id="3dca4-143">String</span></span>|<span data-ttu-id="3dca4-144">Especifica o nome lógico que se refere ao namespace dentro do arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="3dca4-144">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="3dca4-145">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="3dca4-145">targetNamespace</span></span>|<span data-ttu-id="3dca4-146">String</span><span class="sxs-lookup"><span data-stu-id="3dca4-146">String</span></span>|<span data-ttu-id="3dca4-147">Especifica o URI usado para identificar o namespace no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="3dca4-147">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="3dca4-148">PolicyType</span><span class="sxs-lookup"><span data-stu-id="3dca4-148">policyType</span></span>|[<span data-ttu-id="3dca4-149">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="3dca4-149">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="3dca4-150">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="3dca4-150">Specifies the type of group policy.</span></span> <span data-ttu-id="3dca4-151">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="3dca4-151">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="3dca4-152">firmware</span><span class="sxs-lookup"><span data-stu-id="3dca4-152">revision</span></span>|<span data-ttu-id="3dca4-153">String</span><span class="sxs-lookup"><span data-stu-id="3dca4-153">String</span></span>|<span data-ttu-id="3dca4-154">A versão de revisão associada ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="3dca4-154">The revision version associated with the file.</span></span>|
|<span data-ttu-id="3dca4-155">id</span><span class="sxs-lookup"><span data-stu-id="3dca4-155">id</span></span>|<span data-ttu-id="3dca4-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3dca4-156">String</span></span>|<span data-ttu-id="3dca4-157">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3dca4-157">Key of the entity.</span></span>|
|<span data-ttu-id="3dca4-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3dca4-158">lastModifiedDateTime</span></span>|<span data-ttu-id="3dca4-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3dca4-159">DateTimeOffset</span></span>|<span data-ttu-id="3dca4-160">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3dca4-160">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="3dca4-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="3dca4-161">Response</span></span>
<span data-ttu-id="3dca4-162">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3dca4-162">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3dca4-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3dca4-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="3dca4-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3dca4-164">Request</span></span>
<span data-ttu-id="3dca4-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3dca4-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3dca4-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="3dca4-166">Response</span></span>
<span data-ttu-id="3dca4-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3dca4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





