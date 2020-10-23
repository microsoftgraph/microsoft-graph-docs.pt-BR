---
title: Atualizar groupPolicyObjectFile
description: Atualiza as propriedades de um objeto groupPolicyObjectFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6b266b110a0512539018815c0bf4f3cd33700fb3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692993"
---
# <a name="update-grouppolicyobjectfile"></a><span data-ttu-id="06a77-103">Atualizar groupPolicyObjectFile</span><span class="sxs-lookup"><span data-stu-id="06a77-103">Update groupPolicyObjectFile</span></span>

<span data-ttu-id="06a77-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06a77-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06a77-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="06a77-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06a77-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="06a77-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06a77-107">Atualiza as propriedades de um objeto [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) .</span><span class="sxs-lookup"><span data-stu-id="06a77-107">Update the properties of a [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06a77-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="06a77-108">Prerequisites</span></span>
<span data-ttu-id="06a77-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06a77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06a77-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06a77-111">Permission type</span></span>|<span data-ttu-id="06a77-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="06a77-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06a77-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06a77-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06a77-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06a77-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06a77-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06a77-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06a77-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06a77-116">Not supported.</span></span>|
|<span data-ttu-id="06a77-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06a77-117">Application</span></span>|<span data-ttu-id="06a77-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06a77-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06a77-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06a77-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyObjectFiles/{groupPolicyObjectFileId}
```

## <a name="request-headers"></a><span data-ttu-id="06a77-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06a77-120">Request headers</span></span>
|<span data-ttu-id="06a77-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="06a77-121">Header</span></span>|<span data-ttu-id="06a77-122">Valor</span><span class="sxs-lookup"><span data-stu-id="06a77-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06a77-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="06a77-123">Authorization</span></span>|<span data-ttu-id="06a77-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06a77-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06a77-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="06a77-125">Accept</span></span>|<span data-ttu-id="06a77-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06a77-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06a77-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06a77-127">Request body</span></span>
<span data-ttu-id="06a77-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) .</span><span class="sxs-lookup"><span data-stu-id="06a77-128">In the request body, supply a JSON representation for the [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) object.</span></span>

<span data-ttu-id="06a77-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md).</span><span class="sxs-lookup"><span data-stu-id="06a77-129">The following table shows the properties that are required when you create the [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md).</span></span>

|<span data-ttu-id="06a77-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06a77-130">Property</span></span>|<span data-ttu-id="06a77-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="06a77-131">Type</span></span>|<span data-ttu-id="06a77-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="06a77-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06a77-133">id</span><span class="sxs-lookup"><span data-stu-id="06a77-133">id</span></span>|<span data-ttu-id="06a77-134">String</span><span class="sxs-lookup"><span data-stu-id="06a77-134">String</span></span>|<span data-ttu-id="06a77-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="06a77-135">Not yet documented</span></span>|
|<span data-ttu-id="06a77-136">groupPolicyObjectId</span><span class="sxs-lookup"><span data-stu-id="06a77-136">groupPolicyObjectId</span></span>|<span data-ttu-id="06a77-137">Guid</span><span class="sxs-lookup"><span data-stu-id="06a77-137">Guid</span></span>|<span data-ttu-id="06a77-138">O GUID do objeto da política de grupo do conteúdo XML do GPO</span><span class="sxs-lookup"><span data-stu-id="06a77-138">The Group Policy Object GUID from GPO Xml content</span></span>|
|<span data-ttu-id="06a77-139">ouDistinguishedName</span><span class="sxs-lookup"><span data-stu-id="06a77-139">ouDistinguishedName</span></span>|<span data-ttu-id="06a77-140">String</span><span class="sxs-lookup"><span data-stu-id="06a77-140">String</span></span>|<span data-ttu-id="06a77-141">O nome diferenciado da OU.</span><span class="sxs-lookup"><span data-stu-id="06a77-141">The distinguished name of the OU.</span></span>|
|<span data-ttu-id="06a77-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06a77-142">createdDateTime</span></span>|<span data-ttu-id="06a77-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06a77-143">DateTimeOffset</span></span>|<span data-ttu-id="06a77-144">A data e a hora em que o GroupPolicy foi carregado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="06a77-144">The date and time at which the GroupPolicy was first uploaded.</span></span>|
|<span data-ttu-id="06a77-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06a77-145">lastModifiedDateTime</span></span>|<span data-ttu-id="06a77-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06a77-146">DateTimeOffset</span></span>|<span data-ttu-id="06a77-147">A data e a hora em que o GroupPolicyObjectFile foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="06a77-147">The date and time at which the GroupPolicyObjectFile was last modified.</span></span>|
|<span data-ttu-id="06a77-148">content</span><span class="sxs-lookup"><span data-stu-id="06a77-148">content</span></span>|<span data-ttu-id="06a77-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06a77-149">String</span></span>|<span data-ttu-id="06a77-150">O conteúdo do arquivo do objeto de diretiva de grupo.</span><span class="sxs-lookup"><span data-stu-id="06a77-150">The Group Policy Object file content.</span></span>|



## <a name="response"></a><span data-ttu-id="06a77-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="06a77-151">Response</span></span>
<span data-ttu-id="06a77-152">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06a77-152">If successful, this method returns a `200 OK` response code and an updated [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06a77-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06a77-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="06a77-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06a77-154">Request</span></span>
<span data-ttu-id="06a77-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06a77-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyObjectFiles/{groupPolicyObjectFileId}
Content-type: application/json
Content-length: 217

{
  "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
  "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "content": "Content value"
}
```

### <a name="response"></a><span data-ttu-id="06a77-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="06a77-156">Response</span></span>
<span data-ttu-id="06a77-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06a77-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





