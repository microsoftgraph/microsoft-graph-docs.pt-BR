---
title: Criar groupPolicyObjectFile
description: Crie um novo objeto groupPolicyObjectFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a321b735313373b0d412d722edd849eb1370a2ca
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158994"
---
# <a name="create-grouppolicyobjectfile"></a><span data-ttu-id="feea7-103">Criar groupPolicyObjectFile</span><span class="sxs-lookup"><span data-stu-id="feea7-103">Create groupPolicyObjectFile</span></span>

<span data-ttu-id="feea7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="feea7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="feea7-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="feea7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="feea7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="feea7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="feea7-107">Crie um novo [objeto groupPolicyObjectFile.](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)</span><span class="sxs-lookup"><span data-stu-id="feea7-107">Create a new [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="feea7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="feea7-108">Prerequisites</span></span>
<span data-ttu-id="feea7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="feea7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="feea7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="feea7-111">Permission type</span></span>|<span data-ttu-id="feea7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="feea7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="feea7-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="feea7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="feea7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="feea7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="feea7-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="feea7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="feea7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="feea7-116">Not supported.</span></span>|
|<span data-ttu-id="feea7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="feea7-117">Application</span></span>|<span data-ttu-id="feea7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="feea7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="feea7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="feea7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyObjectFiles
```

## <a name="request-headers"></a><span data-ttu-id="feea7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="feea7-120">Request headers</span></span>
|<span data-ttu-id="feea7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="feea7-121">Header</span></span>|<span data-ttu-id="feea7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="feea7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="feea7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="feea7-123">Authorization</span></span>|<span data-ttu-id="feea7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="feea7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="feea7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="feea7-125">Accept</span></span>|<span data-ttu-id="feea7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="feea7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="feea7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="feea7-127">Request body</span></span>
<span data-ttu-id="feea7-128">No corpo da solicitação, fornece uma representação JSON para o objeto groupPolicyObjectFile.</span><span class="sxs-lookup"><span data-stu-id="feea7-128">In the request body, supply a JSON representation for the groupPolicyObjectFile object.</span></span>

<span data-ttu-id="feea7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o groupPolicyObjectFile.</span><span class="sxs-lookup"><span data-stu-id="feea7-129">The following table shows the properties that are required when you create the groupPolicyObjectFile.</span></span>

|<span data-ttu-id="feea7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="feea7-130">Property</span></span>|<span data-ttu-id="feea7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="feea7-131">Type</span></span>|<span data-ttu-id="feea7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="feea7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="feea7-133">id</span><span class="sxs-lookup"><span data-stu-id="feea7-133">id</span></span>|<span data-ttu-id="feea7-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="feea7-134">String</span></span>|<span data-ttu-id="feea7-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="feea7-135">Not yet documented</span></span>|
|<span data-ttu-id="feea7-136">groupPolicyObjectId</span><span class="sxs-lookup"><span data-stu-id="feea7-136">groupPolicyObjectId</span></span>|<span data-ttu-id="feea7-137">Guid</span><span class="sxs-lookup"><span data-stu-id="feea7-137">Guid</span></span>|<span data-ttu-id="feea7-138">O GUID do objeto de política de grupo do conteúdo XML do GPO</span><span class="sxs-lookup"><span data-stu-id="feea7-138">The Group Policy Object GUID from GPO Xml content</span></span>|
|<span data-ttu-id="feea7-139">ouDistinguishedName</span><span class="sxs-lookup"><span data-stu-id="feea7-139">ouDistinguishedName</span></span>|<span data-ttu-id="feea7-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="feea7-140">String</span></span>|<span data-ttu-id="feea7-141">O nome diferenciado da UO.</span><span class="sxs-lookup"><span data-stu-id="feea7-141">The distinguished name of the OU.</span></span>|
|<span data-ttu-id="feea7-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="feea7-142">createdDateTime</span></span>|<span data-ttu-id="feea7-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="feea7-143">DateTimeOffset</span></span>|<span data-ttu-id="feea7-144">A data e a hora em que GroupPolicy foi carregado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="feea7-144">The date and time at which the GroupPolicy was first uploaded.</span></span>|
|<span data-ttu-id="feea7-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="feea7-145">lastModifiedDateTime</span></span>|<span data-ttu-id="feea7-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="feea7-146">DateTimeOffset</span></span>|<span data-ttu-id="feea7-147">A data e a hora em que GroupPolicyObjectFile foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="feea7-147">The date and time at which the GroupPolicyObjectFile was last modified.</span></span>|
|<span data-ttu-id="feea7-148">content</span><span class="sxs-lookup"><span data-stu-id="feea7-148">content</span></span>|<span data-ttu-id="feea7-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="feea7-149">String</span></span>|<span data-ttu-id="feea7-150">O conteúdo do arquivo de objeto de Política de Grupo.</span><span class="sxs-lookup"><span data-stu-id="feea7-150">The Group Policy Object file content.</span></span>|



## <a name="response"></a><span data-ttu-id="feea7-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="feea7-151">Response</span></span>
<span data-ttu-id="feea7-152">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="feea7-152">If successful, this method returns a `201 Created` response code and a [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="feea7-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="feea7-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="feea7-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="feea7-154">Request</span></span>
<span data-ttu-id="feea7-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="feea7-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="feea7-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="feea7-156">Response</span></span>
<span data-ttu-id="feea7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="feea7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




