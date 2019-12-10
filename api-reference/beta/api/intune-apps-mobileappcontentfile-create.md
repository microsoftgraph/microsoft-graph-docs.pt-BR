---
title: Criar mobileAppContentFile
description: Criar um novo objeto mobileAppContentFile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2db3a73f3e8be20ee440c27fccc441628c02f159
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39935488"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="2d103-103">Criar mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="2d103-103">Create mobileAppContentFile</span></span>

> <span data-ttu-id="2d103-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2d103-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d103-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2d103-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d103-106">Criar um novo objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="2d103-106">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d103-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2d103-107">Prerequisites</span></span>
<span data-ttu-id="2d103-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d103-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d103-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d103-110">Permission type</span></span>|<span data-ttu-id="2d103-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2d103-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d103-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d103-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2d103-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d103-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2d103-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d103-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d103-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d103-115">Not supported.</span></span>|
|<span data-ttu-id="2d103-116">Application</span><span class="sxs-lookup"><span data-stu-id="2d103-116">Application</span></span>|<span data-ttu-id="2d103-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d103-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d103-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d103-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="2d103-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d103-119">Request headers</span></span>
|<span data-ttu-id="2d103-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2d103-120">Header</span></span>|<span data-ttu-id="2d103-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2d103-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d103-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d103-122">Authorization</span></span>|<span data-ttu-id="2d103-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d103-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d103-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2d103-124">Accept</span></span>|<span data-ttu-id="2d103-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2d103-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d103-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d103-126">Request body</span></span>
<span data-ttu-id="2d103-127">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="2d103-127">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="2d103-128">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="2d103-128">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="2d103-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d103-129">Property</span></span>|<span data-ttu-id="2d103-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d103-130">Type</span></span>|<span data-ttu-id="2d103-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d103-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d103-132">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="2d103-132">azureStorageUri</span></span>|<span data-ttu-id="2d103-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d103-133">String</span></span>|<span data-ttu-id="2d103-134">O URI de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="2d103-134">The Azure Storage URI.</span></span>|
|<span data-ttu-id="2d103-135">isCommitted</span><span class="sxs-lookup"><span data-stu-id="2d103-135">isCommitted</span></span>|<span data-ttu-id="2d103-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="2d103-136">Boolean</span></span>|<span data-ttu-id="2d103-137">Um valor que indica se o arquivo tem está confirmado.</span><span class="sxs-lookup"><span data-stu-id="2d103-137">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="2d103-138">id</span><span class="sxs-lookup"><span data-stu-id="2d103-138">id</span></span>|<span data-ttu-id="2d103-139">String</span><span class="sxs-lookup"><span data-stu-id="2d103-139">String</span></span>|<span data-ttu-id="2d103-140">A ID do arquivo.</span><span class="sxs-lookup"><span data-stu-id="2d103-140">The File Id.</span></span>|
|<span data-ttu-id="2d103-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2d103-141">createdDateTime</span></span>|<span data-ttu-id="2d103-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d103-142">DateTimeOffset</span></span>|<span data-ttu-id="2d103-143">A hora em que o arquivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="2d103-143">The time the file was created.</span></span>|
|<span data-ttu-id="2d103-144">name</span><span class="sxs-lookup"><span data-stu-id="2d103-144">name</span></span>|<span data-ttu-id="2d103-145">String</span><span class="sxs-lookup"><span data-stu-id="2d103-145">String</span></span>|<span data-ttu-id="2d103-146">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="2d103-146">the file name.</span></span>|
|<span data-ttu-id="2d103-147">size</span><span class="sxs-lookup"><span data-stu-id="2d103-147">size</span></span>|<span data-ttu-id="2d103-148">Int64</span><span class="sxs-lookup"><span data-stu-id="2d103-148">Int64</span></span>|<span data-ttu-id="2d103-149">O tamanho do arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="2d103-149">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="2d103-150">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="2d103-150">sizeEncrypted</span></span>|<span data-ttu-id="2d103-151">Int64</span><span class="sxs-lookup"><span data-stu-id="2d103-151">Int64</span></span>|<span data-ttu-id="2d103-152">O tamanho do arquivo após a criptografia.</span><span class="sxs-lookup"><span data-stu-id="2d103-152">The size of the file after encryption.</span></span>|
|<span data-ttu-id="2d103-153">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2d103-153">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="2d103-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d103-154">DateTimeOffset</span></span>|<span data-ttu-id="2d103-155">A hora de expiração do URI do armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="2d103-155">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="2d103-156">manifest</span><span class="sxs-lookup"><span data-stu-id="2d103-156">manifest</span></span>|<span data-ttu-id="2d103-157">Binária</span><span class="sxs-lookup"><span data-stu-id="2d103-157">Binary</span></span>|<span data-ttu-id="2d103-158">As informações do manifesto.</span><span class="sxs-lookup"><span data-stu-id="2d103-158">The manifest information.</span></span>|
|<span data-ttu-id="2d103-159">uploadState</span><span class="sxs-lookup"><span data-stu-id="2d103-159">uploadState</span></span>|[<span data-ttu-id="2d103-160">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="2d103-160">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="2d103-161">O estado da solicitação de carregamento atual.</span><span class="sxs-lookup"><span data-stu-id="2d103-161">The state of the current upload request.</span></span> <span data-ttu-id="2d103-162">Os valores possíveis são: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="2d103-162">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="2d103-163">isframeworkfile</span><span class="sxs-lookup"><span data-stu-id="2d103-163">isFrameworkFile</span></span>|<span data-ttu-id="2d103-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d103-164">Boolean</span></span>|<span data-ttu-id="2d103-165">Um valor que indica se o arquivo é um arquivo de estrutura.</span><span class="sxs-lookup"><span data-stu-id="2d103-165">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="2d103-166">IsDependency</span><span class="sxs-lookup"><span data-stu-id="2d103-166">isDependency</span></span>|<span data-ttu-id="2d103-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d103-167">Boolean</span></span>|<span data-ttu-id="2d103-168">Se o arquivo de conteúdo é uma dependência para o arquivo de conteúdo principal.</span><span class="sxs-lookup"><span data-stu-id="2d103-168">Whether the content file is a dependency for the main content file.</span></span>|



## <a name="response"></a><span data-ttu-id="2d103-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d103-169">Response</span></span>
<span data-ttu-id="2d103-170">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d103-170">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d103-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2d103-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d103-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d103-172">Request</span></span>
<span data-ttu-id="2d103-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d103-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
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

### <a name="response"></a><span data-ttu-id="2d103-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d103-174">Response</span></span>
<span data-ttu-id="2d103-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2d103-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





