---
title: Criar groupPolicyObjectFile
description: Criar um novo objeto groupPolicyObjectFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 53507ce45286de3689ae248c3873c8fb535007d6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49201118"
---
# <a name="create-grouppolicyobjectfile"></a><span data-ttu-id="64b0d-103">Criar groupPolicyObjectFile</span><span class="sxs-lookup"><span data-stu-id="64b0d-103">Create groupPolicyObjectFile</span></span>

<span data-ttu-id="64b0d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64b0d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64b0d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="64b0d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64b0d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="64b0d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64b0d-107">Criar um novo objeto [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) .</span><span class="sxs-lookup"><span data-stu-id="64b0d-107">Create a new [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64b0d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="64b0d-108">Prerequisites</span></span>
<span data-ttu-id="64b0d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64b0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64b0d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64b0d-111">Permission type</span></span>|<span data-ttu-id="64b0d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="64b0d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64b0d-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64b0d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64b0d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64b0d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="64b0d-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64b0d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64b0d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64b0d-116">Not supported.</span></span>|
|<span data-ttu-id="64b0d-117">Application</span><span class="sxs-lookup"><span data-stu-id="64b0d-117">Application</span></span>|<span data-ttu-id="64b0d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64b0d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64b0d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64b0d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyObjectFiles
```

## <a name="request-headers"></a><span data-ttu-id="64b0d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64b0d-120">Request headers</span></span>
|<span data-ttu-id="64b0d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64b0d-121">Header</span></span>|<span data-ttu-id="64b0d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="64b0d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64b0d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="64b0d-123">Authorization</span></span>|<span data-ttu-id="64b0d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64b0d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64b0d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="64b0d-125">Accept</span></span>|<span data-ttu-id="64b0d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64b0d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64b0d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64b0d-127">Request body</span></span>
<span data-ttu-id="64b0d-128">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyObjectFile.</span><span class="sxs-lookup"><span data-stu-id="64b0d-128">In the request body, supply a JSON representation for the groupPolicyObjectFile object.</span></span>

<span data-ttu-id="64b0d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyObjectFile.</span><span class="sxs-lookup"><span data-stu-id="64b0d-129">The following table shows the properties that are required when you create the groupPolicyObjectFile.</span></span>

|<span data-ttu-id="64b0d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64b0d-130">Property</span></span>|<span data-ttu-id="64b0d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="64b0d-131">Type</span></span>|<span data-ttu-id="64b0d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="64b0d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64b0d-133">id</span><span class="sxs-lookup"><span data-stu-id="64b0d-133">id</span></span>|<span data-ttu-id="64b0d-134">String</span><span class="sxs-lookup"><span data-stu-id="64b0d-134">String</span></span>|<span data-ttu-id="64b0d-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="64b0d-135">Not yet documented</span></span>|
|<span data-ttu-id="64b0d-136">groupPolicyObjectId</span><span class="sxs-lookup"><span data-stu-id="64b0d-136">groupPolicyObjectId</span></span>|<span data-ttu-id="64b0d-137">Guid</span><span class="sxs-lookup"><span data-stu-id="64b0d-137">Guid</span></span>|<span data-ttu-id="64b0d-138">O GUID do objeto da política de grupo do conteúdo XML do GPO</span><span class="sxs-lookup"><span data-stu-id="64b0d-138">The Group Policy Object GUID from GPO Xml content</span></span>|
|<span data-ttu-id="64b0d-139">ouDistinguishedName</span><span class="sxs-lookup"><span data-stu-id="64b0d-139">ouDistinguishedName</span></span>|<span data-ttu-id="64b0d-140">String</span><span class="sxs-lookup"><span data-stu-id="64b0d-140">String</span></span>|<span data-ttu-id="64b0d-141">O nome diferenciado da OU.</span><span class="sxs-lookup"><span data-stu-id="64b0d-141">The distinguished name of the OU.</span></span>|
|<span data-ttu-id="64b0d-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64b0d-142">createdDateTime</span></span>|<span data-ttu-id="64b0d-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64b0d-143">DateTimeOffset</span></span>|<span data-ttu-id="64b0d-144">A data e a hora em que o GroupPolicy foi carregado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="64b0d-144">The date and time at which the GroupPolicy was first uploaded.</span></span>|
|<span data-ttu-id="64b0d-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64b0d-145">lastModifiedDateTime</span></span>|<span data-ttu-id="64b0d-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64b0d-146">DateTimeOffset</span></span>|<span data-ttu-id="64b0d-147">A data e a hora em que o GroupPolicyObjectFile foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="64b0d-147">The date and time at which the GroupPolicyObjectFile was last modified.</span></span>|
|<span data-ttu-id="64b0d-148">content</span><span class="sxs-lookup"><span data-stu-id="64b0d-148">content</span></span>|<span data-ttu-id="64b0d-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64b0d-149">String</span></span>|<span data-ttu-id="64b0d-150">O conteúdo do arquivo do objeto de diretiva de grupo.</span><span class="sxs-lookup"><span data-stu-id="64b0d-150">The Group Policy Object file content.</span></span>|



## <a name="response"></a><span data-ttu-id="64b0d-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="64b0d-151">Response</span></span>
<span data-ttu-id="64b0d-152">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64b0d-152">If successful, this method returns a `201 Created` response code and a [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64b0d-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64b0d-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="64b0d-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64b0d-154">Request</span></span>
<span data-ttu-id="64b0d-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64b0d-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyObjectFiles
Content-type: application/json
Content-length: 217

{
  "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
  "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "content": "Content value"
}
```

### <a name="response"></a><span data-ttu-id="64b0d-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="64b0d-156">Response</span></span>
<span data-ttu-id="64b0d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64b0d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 389

{
  "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
  "id": "65c0499d-499d-65c0-9d49-c0659d49c065",
  "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "content": "Content value"
}
```




