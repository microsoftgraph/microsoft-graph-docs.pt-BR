---
title: Atualizar groupPolicyObjectFile
description: Atualize as propriedades de um objeto groupPolicyObjectFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: efe599f7b894629ca4b1b1d5c2d3492b76bc9b9e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158959"
---
# <a name="update-grouppolicyobjectfile"></a><span data-ttu-id="667ca-103">Atualizar groupPolicyObjectFile</span><span class="sxs-lookup"><span data-stu-id="667ca-103">Update groupPolicyObjectFile</span></span>

<span data-ttu-id="667ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="667ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="667ca-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="667ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="667ca-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="667ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="667ca-107">Atualize as propriedades de [um objeto groupPolicyObjectFile.](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)</span><span class="sxs-lookup"><span data-stu-id="667ca-107">Update the properties of a [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="667ca-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="667ca-108">Prerequisites</span></span>
<span data-ttu-id="667ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="667ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="667ca-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="667ca-111">Permission type</span></span>|<span data-ttu-id="667ca-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="667ca-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="667ca-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="667ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="667ca-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="667ca-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="667ca-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="667ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="667ca-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="667ca-116">Not supported.</span></span>|
|<span data-ttu-id="667ca-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="667ca-117">Application</span></span>|<span data-ttu-id="667ca-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="667ca-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="667ca-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="667ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyObjectFiles/{groupPolicyObjectFileId}
```

## <a name="request-headers"></a><span data-ttu-id="667ca-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="667ca-120">Request headers</span></span>
|<span data-ttu-id="667ca-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="667ca-121">Header</span></span>|<span data-ttu-id="667ca-122">Valor</span><span class="sxs-lookup"><span data-stu-id="667ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="667ca-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="667ca-123">Authorization</span></span>|<span data-ttu-id="667ca-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="667ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="667ca-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="667ca-125">Accept</span></span>|<span data-ttu-id="667ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="667ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="667ca-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="667ca-127">Request body</span></span>
<span data-ttu-id="667ca-128">No corpo da solicitação, fornece uma representação JSON para o [objeto groupPolicyObjectFile.](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)</span><span class="sxs-lookup"><span data-stu-id="667ca-128">In the request body, supply a JSON representation for the [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) object.</span></span>

<span data-ttu-id="667ca-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md).</span><span class="sxs-lookup"><span data-stu-id="667ca-129">The following table shows the properties that are required when you create the [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md).</span></span>

|<span data-ttu-id="667ca-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="667ca-130">Property</span></span>|<span data-ttu-id="667ca-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="667ca-131">Type</span></span>|<span data-ttu-id="667ca-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="667ca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="667ca-133">id</span><span class="sxs-lookup"><span data-stu-id="667ca-133">id</span></span>|<span data-ttu-id="667ca-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="667ca-134">String</span></span>|<span data-ttu-id="667ca-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="667ca-135">Not yet documented</span></span>|
|<span data-ttu-id="667ca-136">groupPolicyObjectId</span><span class="sxs-lookup"><span data-stu-id="667ca-136">groupPolicyObjectId</span></span>|<span data-ttu-id="667ca-137">Guid</span><span class="sxs-lookup"><span data-stu-id="667ca-137">Guid</span></span>|<span data-ttu-id="667ca-138">O GUID do objeto de política de grupo do conteúdo XML do GPO</span><span class="sxs-lookup"><span data-stu-id="667ca-138">The Group Policy Object GUID from GPO Xml content</span></span>|
|<span data-ttu-id="667ca-139">ouDistinguishedName</span><span class="sxs-lookup"><span data-stu-id="667ca-139">ouDistinguishedName</span></span>|<span data-ttu-id="667ca-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="667ca-140">String</span></span>|<span data-ttu-id="667ca-141">O nome diferenciado da UO.</span><span class="sxs-lookup"><span data-stu-id="667ca-141">The distinguished name of the OU.</span></span>|
|<span data-ttu-id="667ca-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="667ca-142">createdDateTime</span></span>|<span data-ttu-id="667ca-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="667ca-143">DateTimeOffset</span></span>|<span data-ttu-id="667ca-144">A data e a hora em que GroupPolicy foi carregado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="667ca-144">The date and time at which the GroupPolicy was first uploaded.</span></span>|
|<span data-ttu-id="667ca-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="667ca-145">lastModifiedDateTime</span></span>|<span data-ttu-id="667ca-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="667ca-146">DateTimeOffset</span></span>|<span data-ttu-id="667ca-147">A data e a hora em que GroupPolicyObjectFile foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="667ca-147">The date and time at which the GroupPolicyObjectFile was last modified.</span></span>|
|<span data-ttu-id="667ca-148">content</span><span class="sxs-lookup"><span data-stu-id="667ca-148">content</span></span>|<span data-ttu-id="667ca-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="667ca-149">String</span></span>|<span data-ttu-id="667ca-150">O conteúdo do arquivo de objeto de Política de Grupo.</span><span class="sxs-lookup"><span data-stu-id="667ca-150">The Group Policy Object file content.</span></span>|



## <a name="response"></a><span data-ttu-id="667ca-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="667ca-151">Response</span></span>
<span data-ttu-id="667ca-152">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="667ca-152">If successful, this method returns a `200 OK` response code and an updated [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="667ca-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="667ca-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="667ca-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="667ca-154">Request</span></span>
<span data-ttu-id="667ca-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="667ca-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="667ca-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="667ca-156">Response</span></span>
<span data-ttu-id="667ca-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="667ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




