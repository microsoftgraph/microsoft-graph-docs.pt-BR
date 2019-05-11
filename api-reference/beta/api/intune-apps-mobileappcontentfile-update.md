---
title: Atualizar mobileAppContentFile
description: Atualiza as propriedades de um objeto mobileAppContentFile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b13499d73179206ef2a5f9859b11a8e60201f81
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935125"
---
# <a name="update-mobileappcontentfile"></a><span data-ttu-id="9bcb1-103">Atualizar mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="9bcb1-103">Update mobileAppContentFile</span></span>

> <span data-ttu-id="9bcb1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9bcb1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bcb1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9bcb1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bcb1-106">Atualiza as propriedades de um objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="9bcb1-106">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9bcb1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9bcb1-107">Prerequisites</span></span>
<span data-ttu-id="9bcb1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bcb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bcb1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9bcb1-110">Permission type</span></span>|<span data-ttu-id="9bcb1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9bcb1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bcb1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9bcb1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9bcb1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bcb1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9bcb1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9bcb1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bcb1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bcb1-115">Not supported.</span></span>|
|<span data-ttu-id="9bcb1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9bcb1-116">Application</span></span>|<span data-ttu-id="9bcb1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bcb1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bcb1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9bcb1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="9bcb1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9bcb1-119">Request headers</span></span>
|<span data-ttu-id="9bcb1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9bcb1-120">Header</span></span>|<span data-ttu-id="9bcb1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9bcb1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bcb1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9bcb1-122">Authorization</span></span>|<span data-ttu-id="9bcb1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9bcb1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bcb1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9bcb1-124">Accept</span></span>|<span data-ttu-id="9bcb1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9bcb1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bcb1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9bcb1-126">Request body</span></span>
<span data-ttu-id="9bcb1-127">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="9bcb1-127">In the request body, supply a JSON representation for the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

<span data-ttu-id="9bcb1-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="9bcb1-128">The following table shows the properties that are required when you create the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>

|<span data-ttu-id="9bcb1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9bcb1-129">Property</span></span>|<span data-ttu-id="9bcb1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bcb1-130">Type</span></span>|<span data-ttu-id="9bcb1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bcb1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bcb1-132">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="9bcb1-132">azureStorageUri</span></span>|<span data-ttu-id="9bcb1-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bcb1-133">String</span></span>|<span data-ttu-id="9bcb1-134">O URI de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="9bcb1-134">The Azure Storage URI.</span></span>|
|<span data-ttu-id="9bcb1-135">isCommitted</span><span class="sxs-lookup"><span data-stu-id="9bcb1-135">isCommitted</span></span>|<span data-ttu-id="9bcb1-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="9bcb1-136">Boolean</span></span>|<span data-ttu-id="9bcb1-137">Um valor que indica se o arquivo tem está confirmado.</span><span class="sxs-lookup"><span data-stu-id="9bcb1-137">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="9bcb1-138">id</span><span class="sxs-lookup"><span data-stu-id="9bcb1-138">id</span></span>|<span data-ttu-id="9bcb1-139">String</span><span class="sxs-lookup"><span data-stu-id="9bcb1-139">String</span></span>|<span data-ttu-id="9bcb1-140">A ID do arquivo.</span><span class="sxs-lookup"><span data-stu-id="9bcb1-140">The File Id.</span></span>|
|<span data-ttu-id="9bcb1-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9bcb1-141">createdDateTime</span></span>|<span data-ttu-id="9bcb1-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bcb1-142">DateTimeOffset</span></span>|<span data-ttu-id="9bcb1-143">A hora em que o arquivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="9bcb1-143">The time the file was created.</span></span>|
|<span data-ttu-id="9bcb1-144">nome</span><span class="sxs-lookup"><span data-stu-id="9bcb1-144">name</span></span>|<span data-ttu-id="9bcb1-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bcb1-145">String</span></span>|<span data-ttu-id="9bcb1-146">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="9bcb1-146">the file name.</span></span>|
|<span data-ttu-id="9bcb1-147">size</span><span class="sxs-lookup"><span data-stu-id="9bcb1-147">size</span></span>|<span data-ttu-id="9bcb1-148">Int64</span><span class="sxs-lookup"><span data-stu-id="9bcb1-148">Int64</span></span>|<span data-ttu-id="9bcb1-149">O tamanho do arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="9bcb1-149">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="9bcb1-150">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="9bcb1-150">sizeEncrypted</span></span>|<span data-ttu-id="9bcb1-151">Int64</span><span class="sxs-lookup"><span data-stu-id="9bcb1-151">Int64</span></span>|<span data-ttu-id="9bcb1-152">O tamanho do arquivo após a criptografia.</span><span class="sxs-lookup"><span data-stu-id="9bcb1-152">The size of the file after encryption.</span></span>|
|<span data-ttu-id="9bcb1-153">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9bcb1-153">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="9bcb1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bcb1-154">DateTimeOffset</span></span>|<span data-ttu-id="9bcb1-155">A hora de expiração do URI do armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="9bcb1-155">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="9bcb1-156">manifest</span><span class="sxs-lookup"><span data-stu-id="9bcb1-156">manifest</span></span>|<span data-ttu-id="9bcb1-157">Binária</span><span class="sxs-lookup"><span data-stu-id="9bcb1-157">Binary</span></span>|<span data-ttu-id="9bcb1-158">As informações do manifesto.</span><span class="sxs-lookup"><span data-stu-id="9bcb1-158">The manifest information.</span></span>|
|<span data-ttu-id="9bcb1-159">uploadState</span><span class="sxs-lookup"><span data-stu-id="9bcb1-159">uploadState</span></span>|[<span data-ttu-id="9bcb1-160">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="9bcb1-160">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="9bcb1-161">O estado da solicitação de carregamento atual.</span><span class="sxs-lookup"><span data-stu-id="9bcb1-161">The state of the current upload request.</span></span> <span data-ttu-id="9bcb1-162">Os valores possíveis são: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="9bcb1-162">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="9bcb1-163">isframeworkfile</span><span class="sxs-lookup"><span data-stu-id="9bcb1-163">isFrameworkFile</span></span>|<span data-ttu-id="9bcb1-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="9bcb1-164">Boolean</span></span>|<span data-ttu-id="9bcb1-165">Um valor que indica se o arquivo é um arquivo de estrutura.</span><span class="sxs-lookup"><span data-stu-id="9bcb1-165">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="9bcb1-166">IsDependency</span><span class="sxs-lookup"><span data-stu-id="9bcb1-166">isDependency</span></span>|<span data-ttu-id="9bcb1-167">Booliano</span><span class="sxs-lookup"><span data-stu-id="9bcb1-167">Boolean</span></span>|<span data-ttu-id="9bcb1-168">Se o arquivo de conteúdo é uma dependência para o arquivo de conteúdo principal.</span><span class="sxs-lookup"><span data-stu-id="9bcb1-168">Whether the content file is a dependency for the main content file.</span></span>|



## <a name="response"></a><span data-ttu-id="9bcb1-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bcb1-169">Response</span></span>
<span data-ttu-id="9bcb1-170">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9bcb1-170">If successful, this method returns a `200 OK` response code and an updated [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bcb1-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9bcb1-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="9bcb1-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bcb1-172">Request</span></span>
<span data-ttu-id="9bcb1-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9bcb1-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
Content-type: application/json
Content-length: 395

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError",
  "isFrameworkFile": true,
  "isDependency": true
}
```

### <a name="response"></a><span data-ttu-id="9bcb1-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bcb1-174">Response</span></span>
<span data-ttu-id="9bcb1-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9bcb1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 503

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "id": "eab2e29b-e29b-eab2-9be2-b2ea9be2b2ea",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError",
  "isFrameworkFile": true,
  "isDependency": true
}
```




