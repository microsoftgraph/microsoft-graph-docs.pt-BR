---
title: Criar groupPolicyOperation
description: Crie um novo objeto groupPolicyOperation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4023978bbfd544e73b010c59a3507857f64e29d1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157482"
---
# <a name="create-grouppolicyoperation"></a><span data-ttu-id="82346-103">Criar groupPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="82346-103">Create groupPolicyOperation</span></span>

<span data-ttu-id="82346-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82346-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82346-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="82346-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82346-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="82346-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82346-107">Crie um novo [objeto groupPolicyOperation.](../resources/intune-grouppolicy-grouppolicyoperation.md)</span><span class="sxs-lookup"><span data-stu-id="82346-107">Create a new [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82346-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="82346-108">Prerequisites</span></span>
<span data-ttu-id="82346-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82346-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82346-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82346-111">Permission type</span></span>|<span data-ttu-id="82346-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="82346-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82346-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82346-113">Delegated (work or school account)</span></span>|<span data-ttu-id="82346-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82346-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82346-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82346-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82346-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82346-116">Not supported.</span></span>|
|<span data-ttu-id="82346-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82346-117">Application</span></span>|<span data-ttu-id="82346-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82346-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82346-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82346-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/microsoft.graph.groupPolicyUploadedDefinitionFile/groupPolicyOperations
```

## <a name="request-headers"></a><span data-ttu-id="82346-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82346-120">Request headers</span></span>
|<span data-ttu-id="82346-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="82346-121">Header</span></span>|<span data-ttu-id="82346-122">Valor</span><span class="sxs-lookup"><span data-stu-id="82346-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82346-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="82346-123">Authorization</span></span>|<span data-ttu-id="82346-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82346-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82346-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="82346-125">Accept</span></span>|<span data-ttu-id="82346-126">application/json</span><span class="sxs-lookup"><span data-stu-id="82346-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82346-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82346-127">Request body</span></span>
<span data-ttu-id="82346-128">No corpo da solicitação, fornece uma representação JSON para o objeto groupPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="82346-128">In the request body, supply a JSON representation for the groupPolicyOperation object.</span></span>

<span data-ttu-id="82346-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o groupPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="82346-129">The following table shows the properties that are required when you create the groupPolicyOperation.</span></span>

|<span data-ttu-id="82346-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82346-130">Property</span></span>|<span data-ttu-id="82346-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="82346-131">Type</span></span>|<span data-ttu-id="82346-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="82346-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82346-133">operationType</span><span class="sxs-lookup"><span data-stu-id="82346-133">operationType</span></span>|[<span data-ttu-id="82346-134">groupPolicyOperationType</span><span class="sxs-lookup"><span data-stu-id="82346-134">groupPolicyOperationType</span></span>](../resources/intune-grouppolicy-grouppolicyoperationtype.md)|<span data-ttu-id="82346-135">O tipo de operação de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="82346-135">The type of group policy operation.</span></span> <span data-ttu-id="82346-136">Os valores possíveis são: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.</span><span class="sxs-lookup"><span data-stu-id="82346-136">Possible values are: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.</span></span>|
|<span data-ttu-id="82346-137">operationStatus</span><span class="sxs-lookup"><span data-stu-id="82346-137">operationStatus</span></span>|[<span data-ttu-id="82346-138">groupPolicyOperationStatus</span><span class="sxs-lookup"><span data-stu-id="82346-138">groupPolicyOperationStatus</span></span>](../resources/intune-grouppolicy-grouppolicyoperationstatus.md)|<span data-ttu-id="82346-139">O status da operação de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="82346-139">The group policy operation status.</span></span> <span data-ttu-id="82346-140">Os valores possíveis são: `unknown`, `inProgress`, `success`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="82346-140">Possible values are: `unknown`, `inProgress`, `success`, `failed`.</span></span>|
|<span data-ttu-id="82346-141">statusDetails</span><span class="sxs-lookup"><span data-stu-id="82346-141">statusDetails</span></span>|<span data-ttu-id="82346-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82346-142">String</span></span>|<span data-ttu-id="82346-143">O detalhe do status da operação de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="82346-143">The group policy operation status detail.</span></span>|
|<span data-ttu-id="82346-144">id</span><span class="sxs-lookup"><span data-stu-id="82346-144">id</span></span>|<span data-ttu-id="82346-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82346-145">String</span></span>|<span data-ttu-id="82346-146">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="82346-146">Key of the entity.</span></span>|
|<span data-ttu-id="82346-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="82346-147">lastModifiedDateTime</span></span>|<span data-ttu-id="82346-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82346-148">DateTimeOffset</span></span>|<span data-ttu-id="82346-149">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="82346-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="82346-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="82346-150">Response</span></span>
<span data-ttu-id="82346-151">Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="82346-151">If successful, this method returns a `201 Created` response code and a [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82346-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82346-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="82346-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82346-153">Request</span></span>
<span data-ttu-id="82346-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="82346-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/microsoft.graph.groupPolicyUploadedDefinitionFile/groupPolicyOperations
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.groupPolicyOperation",
  "operationType": "upload",
  "operationStatus": "inProgress",
  "statusDetails": "Status Details value"
}
```

### <a name="response"></a><span data-ttu-id="82346-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="82346-155">Response</span></span>
<span data-ttu-id="82346-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="82346-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.groupPolicyOperation",
  "operationType": "upload",
  "operationStatus": "inProgress",
  "statusDetails": "Status Details value",
  "id": "4d18865b-865b-4d18-5b86-184d5b86184d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




