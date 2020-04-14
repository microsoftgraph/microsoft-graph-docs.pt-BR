---
title: Atualizar groupPolicyOperation
description: Atualiza as propriedades de um objeto groupPolicyOperation.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 365d94e1c7710bf8c1b84878a1b0feff123f3faf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457290"
---
# <a name="update-grouppolicyoperation"></a><span data-ttu-id="1203a-103">Atualizar groupPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="1203a-103">Update groupPolicyOperation</span></span>

<span data-ttu-id="1203a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1203a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1203a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1203a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1203a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1203a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1203a-107">Atualiza as propriedades de um objeto [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="1203a-107">Update the properties of a [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1203a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1203a-108">Prerequisites</span></span>
<span data-ttu-id="1203a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1203a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1203a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1203a-111">Permission type</span></span>|<span data-ttu-id="1203a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1203a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1203a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1203a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1203a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1203a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1203a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1203a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1203a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1203a-116">Not supported.</span></span>|
|<span data-ttu-id="1203a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1203a-117">Application</span></span>|<span data-ttu-id="1203a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1203a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1203a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1203a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/microsoft.graph.groupPolicyUploadedDefinitionFile/groupPolicyOperations/{groupPolicyOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="1203a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1203a-120">Request headers</span></span>
|<span data-ttu-id="1203a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1203a-121">Header</span></span>|<span data-ttu-id="1203a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1203a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1203a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1203a-123">Authorization</span></span>|<span data-ttu-id="1203a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1203a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1203a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1203a-125">Accept</span></span>|<span data-ttu-id="1203a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1203a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1203a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1203a-127">Request body</span></span>
<span data-ttu-id="1203a-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="1203a-128">In the request body, supply a JSON representation for the [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object.</span></span>

<span data-ttu-id="1203a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md).</span><span class="sxs-lookup"><span data-stu-id="1203a-129">The following table shows the properties that are required when you create the [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md).</span></span>

|<span data-ttu-id="1203a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1203a-130">Property</span></span>|<span data-ttu-id="1203a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1203a-131">Type</span></span>|<span data-ttu-id="1203a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1203a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1203a-133">OperationType</span><span class="sxs-lookup"><span data-stu-id="1203a-133">operationType</span></span>|[<span data-ttu-id="1203a-134">groupPolicyOperationType</span><span class="sxs-lookup"><span data-stu-id="1203a-134">groupPolicyOperationType</span></span>](../resources/intune-grouppolicy-grouppolicyoperationtype.md)|<span data-ttu-id="1203a-135">O tipo de operação de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="1203a-135">The type of group policy operation.</span></span> <span data-ttu-id="1203a-136">Os valores possíveis são: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.</span><span class="sxs-lookup"><span data-stu-id="1203a-136">Possible values are: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.</span></span>|
|<span data-ttu-id="1203a-137">operationStatus</span><span class="sxs-lookup"><span data-stu-id="1203a-137">operationStatus</span></span>|[<span data-ttu-id="1203a-138">groupPolicyOperationStatus</span><span class="sxs-lookup"><span data-stu-id="1203a-138">groupPolicyOperationStatus</span></span>](../resources/intune-grouppolicy-grouppolicyoperationstatus.md)|<span data-ttu-id="1203a-139">O status da operação da política de grupo.</span><span class="sxs-lookup"><span data-stu-id="1203a-139">The group policy operation status.</span></span> <span data-ttu-id="1203a-140">Os valores possíveis são: `unknown`, `inProgress`, `success`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="1203a-140">Possible values are: `unknown`, `inProgress`, `success`, `failed`.</span></span>|
|<span data-ttu-id="1203a-141">statusDetails</span><span class="sxs-lookup"><span data-stu-id="1203a-141">statusDetails</span></span>|<span data-ttu-id="1203a-142">String</span><span class="sxs-lookup"><span data-stu-id="1203a-142">String</span></span>|<span data-ttu-id="1203a-143">Detalhes do status da operação da política de grupo.</span><span class="sxs-lookup"><span data-stu-id="1203a-143">The group policy operation status detail.</span></span>|
|<span data-ttu-id="1203a-144">id</span><span class="sxs-lookup"><span data-stu-id="1203a-144">id</span></span>|<span data-ttu-id="1203a-145">String</span><span class="sxs-lookup"><span data-stu-id="1203a-145">String</span></span>|<span data-ttu-id="1203a-146">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1203a-146">Key of the entity.</span></span>|
|<span data-ttu-id="1203a-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1203a-147">lastModifiedDateTime</span></span>|<span data-ttu-id="1203a-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1203a-148">DateTimeOffset</span></span>|<span data-ttu-id="1203a-149">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="1203a-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="1203a-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="1203a-150">Response</span></span>
<span data-ttu-id="1203a-151">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1203a-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1203a-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1203a-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="1203a-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1203a-153">Request</span></span>
<span data-ttu-id="1203a-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1203a-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/microsoft.graph.groupPolicyUploadedDefinitionFile/groupPolicyOperations/{groupPolicyOperationId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.groupPolicyOperation",
  "operationType": "upload",
  "operationStatus": "inProgress",
  "statusDetails": "Status Details value"
}
```

### <a name="response"></a><span data-ttu-id="1203a-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="1203a-155">Response</span></span>
<span data-ttu-id="1203a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1203a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



