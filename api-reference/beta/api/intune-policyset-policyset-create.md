---
title: Criar policySet
description: Crie um novo objeto policySet.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 864df7c89a6dbbcc80932e87f6616c79d52eca99
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134638"
---
# <a name="create-policyset"></a><span data-ttu-id="79394-103">Criar policySet</span><span class="sxs-lookup"><span data-stu-id="79394-103">Create policySet</span></span>

<span data-ttu-id="79394-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79394-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79394-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="79394-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79394-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="79394-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79394-107">Crie um novo [objeto policySet.](../resources/intune-policyset-policyset.md)</span><span class="sxs-lookup"><span data-stu-id="79394-107">Create a new [policySet](../resources/intune-policyset-policyset.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79394-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="79394-108">Prerequisites</span></span>
<span data-ttu-id="79394-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79394-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79394-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79394-111">Permission type</span></span>|<span data-ttu-id="79394-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="79394-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79394-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79394-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79394-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79394-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="79394-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79394-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79394-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79394-116">Not supported.</span></span>|
|<span data-ttu-id="79394-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79394-117">Application</span></span>|<span data-ttu-id="79394-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79394-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79394-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79394-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets
```

## <a name="request-headers"></a><span data-ttu-id="79394-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79394-120">Request headers</span></span>
|<span data-ttu-id="79394-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="79394-121">Header</span></span>|<span data-ttu-id="79394-122">Valor</span><span class="sxs-lookup"><span data-stu-id="79394-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79394-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="79394-123">Authorization</span></span>|<span data-ttu-id="79394-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79394-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79394-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="79394-125">Accept</span></span>|<span data-ttu-id="79394-126">application/json</span><span class="sxs-lookup"><span data-stu-id="79394-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79394-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79394-127">Request body</span></span>
<span data-ttu-id="79394-128">No corpo da solicitação, fornece uma representação JSON para o objeto policySet.</span><span class="sxs-lookup"><span data-stu-id="79394-128">In the request body, supply a JSON representation for the policySet object.</span></span>

<span data-ttu-id="79394-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o policySet.</span><span class="sxs-lookup"><span data-stu-id="79394-129">The following table shows the properties that are required when you create the policySet.</span></span>

|<span data-ttu-id="79394-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79394-130">Property</span></span>|<span data-ttu-id="79394-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="79394-131">Type</span></span>|<span data-ttu-id="79394-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="79394-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79394-133">id</span><span class="sxs-lookup"><span data-stu-id="79394-133">id</span></span>|<span data-ttu-id="79394-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79394-134">String</span></span>|<span data-ttu-id="79394-135">Chave do PolicySet.</span><span class="sxs-lookup"><span data-stu-id="79394-135">Key of the PolicySet.</span></span>|
|<span data-ttu-id="79394-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79394-136">createdDateTime</span></span>|<span data-ttu-id="79394-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79394-137">DateTimeOffset</span></span>|<span data-ttu-id="79394-138">Hora de criação do PolicySet.</span><span class="sxs-lookup"><span data-stu-id="79394-138">Creation time of the PolicySet.</span></span>|
|<span data-ttu-id="79394-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="79394-139">lastModifiedDateTime</span></span>|<span data-ttu-id="79394-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79394-140">DateTimeOffset</span></span>|<span data-ttu-id="79394-141">Última hora modificada do PolicySet.</span><span class="sxs-lookup"><span data-stu-id="79394-141">Last modified time of the PolicySet.</span></span>|
|<span data-ttu-id="79394-142">displayName</span><span class="sxs-lookup"><span data-stu-id="79394-142">displayName</span></span>|<span data-ttu-id="79394-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79394-143">String</span></span>|<span data-ttu-id="79394-144">DisplayName do PolicySet.</span><span class="sxs-lookup"><span data-stu-id="79394-144">DisplayName of the PolicySet.</span></span>|
|<span data-ttu-id="79394-145">descrição</span><span class="sxs-lookup"><span data-stu-id="79394-145">description</span></span>|<span data-ttu-id="79394-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79394-146">String</span></span>|<span data-ttu-id="79394-147">Descrição do PolicySet.</span><span class="sxs-lookup"><span data-stu-id="79394-147">Description of the PolicySet.</span></span>|
|<span data-ttu-id="79394-148">status</span><span class="sxs-lookup"><span data-stu-id="79394-148">status</span></span>|[<span data-ttu-id="79394-149">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="79394-149">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="79394-150">Status de validação/atribuição do PolicySet.</span><span class="sxs-lookup"><span data-stu-id="79394-150">Validation/assignment status of the PolicySet.</span></span> <span data-ttu-id="79394-151">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="79394-151">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="79394-152">errorCode</span><span class="sxs-lookup"><span data-stu-id="79394-152">errorCode</span></span>|[<span data-ttu-id="79394-153">errorCode</span><span class="sxs-lookup"><span data-stu-id="79394-153">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="79394-154">Código de erro se ocorrer algum.</span><span class="sxs-lookup"><span data-stu-id="79394-154">Error code if any occured.</span></span> <span data-ttu-id="79394-155">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="79394-155">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="79394-156">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="79394-156">guidedDeploymentTags</span></span>|<span data-ttu-id="79394-157">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="79394-157">String collection</span></span>|<span data-ttu-id="79394-158">Marcas da implantação guiada</span><span class="sxs-lookup"><span data-stu-id="79394-158">Tags of the guided deployment</span></span>|
|<span data-ttu-id="79394-159">roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="79394-159">roleScopeTags</span></span>|<span data-ttu-id="79394-160">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="79394-160">String collection</span></span>|<span data-ttu-id="79394-161">RoleScopeTags do PolicySet</span><span class="sxs-lookup"><span data-stu-id="79394-161">RoleScopeTags of the PolicySet</span></span>|



## <a name="response"></a><span data-ttu-id="79394-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="79394-162">Response</span></span>
<span data-ttu-id="79394-163">Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [policySet](../resources/intune-policyset-policyset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79394-163">If successful, this method returns a `201 Created` response code and a [policySet](../resources/intune-policyset-policyset.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79394-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79394-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="79394-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79394-165">Request</span></span>
<span data-ttu-id="79394-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="79394-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets
Content-type: application/json
Content-length: 317

{
  "@odata.type": "#microsoft.graph.policySet",
  "displayName": "Display Name value",
  "description": "Description value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "roleScopeTags": [
    "Role Scope Tags value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="79394-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="79394-167">Response</span></span>
<span data-ttu-id="79394-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="79394-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 489

{
  "@odata.type": "#microsoft.graph.policySet",
  "id": "653cb373-b373-653c-73b3-3c6573b33c65",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "roleScopeTags": [
    "Role Scope Tags value"
  ]
}
```




