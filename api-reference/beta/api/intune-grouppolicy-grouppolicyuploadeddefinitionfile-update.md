---
title: Atualizar groupPolicyUploadedDefinitionFile
description: Atualiza as propriedades de um objeto groupPolicyUploadedDefinitionFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 448f1103d9d0397c7d24ea4d97e9bd905705e0b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040599"
---
# <a name="update-grouppolicyuploadeddefinitionfile"></a><span data-ttu-id="b3756-103">Atualizar groupPolicyUploadedDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="b3756-103">Update groupPolicyUploadedDefinitionFile</span></span>

<span data-ttu-id="b3756-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3756-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3756-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b3756-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3756-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b3756-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3756-107">Atualiza as propriedades de um objeto [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="b3756-107">Update the properties of a [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3756-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b3756-108">Prerequisites</span></span>
<span data-ttu-id="b3756-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3756-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3756-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3756-111">Permission type</span></span>|<span data-ttu-id="b3756-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b3756-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3756-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3756-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b3756-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3756-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b3756-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3756-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3756-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3756-116">Not supported.</span></span>|
|<span data-ttu-id="b3756-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3756-117">Application</span></span>|<span data-ttu-id="b3756-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3756-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3756-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3756-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyUploadedDefinitionFiles/{groupPolicyUploadedDefinitionFileId}
```

## <a name="request-headers"></a><span data-ttu-id="b3756-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3756-120">Request headers</span></span>
|<span data-ttu-id="b3756-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b3756-121">Header</span></span>|<span data-ttu-id="b3756-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b3756-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3756-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3756-123">Authorization</span></span>|<span data-ttu-id="b3756-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3756-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3756-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b3756-125">Accept</span></span>|<span data-ttu-id="b3756-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3756-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3756-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3756-127">Request body</span></span>
<span data-ttu-id="b3756-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="b3756-128">In the request body, supply a JSON representation for the [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) object.</span></span>

<span data-ttu-id="b3756-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md).</span><span class="sxs-lookup"><span data-stu-id="b3756-129">The following table shows the properties that are required when you create the [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md).</span></span>

|<span data-ttu-id="b3756-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3756-130">Property</span></span>|<span data-ttu-id="b3756-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3756-131">Type</span></span>|<span data-ttu-id="b3756-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3756-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3756-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b3756-133">displayName</span></span>|<span data-ttu-id="b3756-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3756-134">String</span></span>|<span data-ttu-id="b3756-135">O nome amigável localizado do arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="b3756-135">The localized friendly name of the ADMX file.</span></span> <span data-ttu-id="b3756-136">Herdado de [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="b3756-136">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="b3756-137">description</span><span class="sxs-lookup"><span data-stu-id="b3756-137">description</span></span>|<span data-ttu-id="b3756-138">String</span><span class="sxs-lookup"><span data-stu-id="b3756-138">String</span></span>|<span data-ttu-id="b3756-139">A descrição localizada das configurações de política no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="b3756-139">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="b3756-140">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="b3756-140">The default value is empty.</span></span> <span data-ttu-id="b3756-141">Herdado de [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="b3756-141">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="b3756-142">languageCodes</span><span class="sxs-lookup"><span data-stu-id="b3756-142">languageCodes</span></span>|<span data-ttu-id="b3756-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3756-143">String collection</span></span>|<span data-ttu-id="b3756-144">Os códigos de idioma suportados para o arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="b3756-144">The supported language codes for the ADMX file.</span></span> <span data-ttu-id="b3756-145">Herdado de [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="b3756-145">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="b3756-146">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="b3756-146">targetPrefix</span></span>|<span data-ttu-id="b3756-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3756-147">String</span></span>|<span data-ttu-id="b3756-148">Especifica o nome lógico que se refere ao namespace dentro do arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="b3756-148">Specifies the logical name that refers to the namespace within the ADMX file.</span></span> <span data-ttu-id="b3756-149">Herdado de [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="b3756-149">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="b3756-150">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="b3756-150">targetNamespace</span></span>|<span data-ttu-id="b3756-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3756-151">String</span></span>|<span data-ttu-id="b3756-152">Especifica o URI usado para identificar o namespace no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="b3756-152">Specifies the URI used to identify the namespace within the ADMX file.</span></span> <span data-ttu-id="b3756-153">Herdado de [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="b3756-153">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="b3756-154">PolicyType</span><span class="sxs-lookup"><span data-stu-id="b3756-154">policyType</span></span>|[<span data-ttu-id="b3756-155">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="b3756-155">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="b3756-156">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="b3756-156">Specifies the type of group policy.</span></span> <span data-ttu-id="b3756-157">Herdado de [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span><span class="sxs-lookup"><span data-stu-id="b3756-157">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span></span> <span data-ttu-id="b3756-158">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="b3756-158">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="b3756-159">firmware</span><span class="sxs-lookup"><span data-stu-id="b3756-159">revision</span></span>|<span data-ttu-id="b3756-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3756-160">String</span></span>|<span data-ttu-id="b3756-161">A versão de revisão associada ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="b3756-161">The revision version associated with the file.</span></span> <span data-ttu-id="b3756-162">Herdado de [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="b3756-162">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="b3756-163">id</span><span class="sxs-lookup"><span data-stu-id="b3756-163">id</span></span>|<span data-ttu-id="b3756-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3756-164">String</span></span>|<span data-ttu-id="b3756-165">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b3756-165">Key of the entity.</span></span> <span data-ttu-id="b3756-166">Herdado de [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="b3756-166">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="b3756-167">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3756-167">lastModifiedDateTime</span></span>|<span data-ttu-id="b3756-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3756-168">DateTimeOffset</span></span>|<span data-ttu-id="b3756-169">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b3756-169">The date and time the entity was last modified.</span></span> <span data-ttu-id="b3756-170">Herdado de [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="b3756-170">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="b3756-171">fileName</span><span class="sxs-lookup"><span data-stu-id="b3756-171">fileName</span></span>|<span data-ttu-id="b3756-172">String</span><span class="sxs-lookup"><span data-stu-id="b3756-172">String</span></span>|<span data-ttu-id="b3756-173">O nome de arquivo do arquivo ADML carregado.</span><span class="sxs-lookup"><span data-stu-id="b3756-173">The file name of the uploaded ADML file.</span></span>|
|<span data-ttu-id="b3756-174">status</span><span class="sxs-lookup"><span data-stu-id="b3756-174">status</span></span>|[<span data-ttu-id="b3756-175">groupPolicyUploadedDefinitionFileStatus</span><span class="sxs-lookup"><span data-stu-id="b3756-175">groupPolicyUploadedDefinitionFileStatus</span></span>](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfilestatus.md)|<span data-ttu-id="b3756-176">O status de upload do arquivo ADMX carregado.</span><span class="sxs-lookup"><span data-stu-id="b3756-176">The upload status of the uploaded ADMX file.</span></span> <span data-ttu-id="b3756-177">Os valores possíveis são: `none`, `uploadInProgress`, `available`, `assigned`, `removalInProgress`, `uploadFailed`, `removalFailed`.</span><span class="sxs-lookup"><span data-stu-id="b3756-177">Possible values are: `none`, `uploadInProgress`, `available`, `assigned`, `removalInProgress`, `uploadFailed`, `removalFailed`.</span></span>|
|<span data-ttu-id="b3756-178">conteúdo</span><span class="sxs-lookup"><span data-stu-id="b3756-178">content</span></span>|<span data-ttu-id="b3756-179">Binária</span><span class="sxs-lookup"><span data-stu-id="b3756-179">Binary</span></span>|<span data-ttu-id="b3756-180">O conteúdo do arquivo ADMX carregado.</span><span class="sxs-lookup"><span data-stu-id="b3756-180">The contents of the uploaded ADMX file.</span></span>|
|<span data-ttu-id="b3756-181">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="b3756-181">uploadDateTime</span></span>|<span data-ttu-id="b3756-182">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3756-182">DateTimeOffset</span></span>|<span data-ttu-id="b3756-183">O tempo carregado do arquivo ADMX carregado.</span><span class="sxs-lookup"><span data-stu-id="b3756-183">The uploaded time of the uploaded ADMX file.</span></span>|
|<span data-ttu-id="b3756-184">defaultLanguageCode</span><span class="sxs-lookup"><span data-stu-id="b3756-184">defaultLanguageCode</span></span>|<span data-ttu-id="b3756-185">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3756-185">String</span></span>|<span data-ttu-id="b3756-186">O idioma padrão do arquivo ADMX carregado.</span><span class="sxs-lookup"><span data-stu-id="b3756-186">The default language of the uploaded ADMX file.</span></span>|
|<span data-ttu-id="b3756-187">groupPolicyUploadedLanguageFiles</span><span class="sxs-lookup"><span data-stu-id="b3756-187">groupPolicyUploadedLanguageFiles</span></span>|<span data-ttu-id="b3756-188">coleção [groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md)</span><span class="sxs-lookup"><span data-stu-id="b3756-188">[groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md) collection</span></span>|<span data-ttu-id="b3756-189">A lista de arquivos ADML associados ao arquivo ADMX carregado.</span><span class="sxs-lookup"><span data-stu-id="b3756-189">The list of ADML files associated with the uploaded ADMX file.</span></span>|



## <a name="response"></a><span data-ttu-id="b3756-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3756-190">Response</span></span>
<span data-ttu-id="b3756-191">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3756-191">If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3756-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3756-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3756-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3756-193">Request</span></span>
<span data-ttu-id="b3756-194">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3756-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyUploadedDefinitionFiles/{groupPolicyUploadedDefinitionFileId}
Content-type: application/json
Content-length: 922

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested",
  "revision": "Revision value",
  "fileName": "File Name value",
  "status": "uploadInProgress",
  "content": "Y29udGVudA==",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00",
  "defaultLanguageCode": "Default Language Code value",
  "groupPolicyUploadedLanguageFiles": [
    {
      "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile",
      "fileName": "File Name value",
      "languageCode": "Language Code value",
      "content": "Y29udGVudA==",
      "id": "Id value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b3756-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3756-195">Response</span></span>
<span data-ttu-id="b3756-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3756-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1035

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested",
  "revision": "Revision value",
  "id": "0ce1a8cf-a8cf-0ce1-cfa8-e10ccfa8e10c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "fileName": "File Name value",
  "status": "uploadInProgress",
  "content": "Y29udGVudA==",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00",
  "defaultLanguageCode": "Default Language Code value",
  "groupPolicyUploadedLanguageFiles": [
    {
      "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile",
      "fileName": "File Name value",
      "languageCode": "Language Code value",
      "content": "Y29udGVudA==",
      "id": "Id value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```






