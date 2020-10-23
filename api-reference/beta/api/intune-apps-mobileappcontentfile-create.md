---
title: Criar mobileAppContentFile
description: Criar um novo objeto mobileAppContentFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0bb4f988804cf9e28f1221f89734d766e6c987ea
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48695954"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="0fa0d-103">Criar mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="0fa0d-103">Create mobileAppContentFile</span></span>

<span data-ttu-id="0fa0d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fa0d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0fa0d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0fa0d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fa0d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0fa0d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fa0d-107">Criar um novo objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="0fa0d-107">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0fa0d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0fa0d-108">Prerequisites</span></span>
<span data-ttu-id="0fa0d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fa0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fa0d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0fa0d-111">Permission type</span></span>|<span data-ttu-id="0fa0d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0fa0d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fa0d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0fa0d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0fa0d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fa0d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0fa0d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0fa0d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fa0d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0fa0d-116">Not supported.</span></span>|
|<span data-ttu-id="0fa0d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0fa0d-117">Application</span></span>|<span data-ttu-id="0fa0d-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fa0d-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fa0d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0fa0d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="0fa0d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0fa0d-120">Request headers</span></span>
|<span data-ttu-id="0fa0d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0fa0d-121">Header</span></span>|<span data-ttu-id="0fa0d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0fa0d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0fa0d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0fa0d-123">Authorization</span></span>|<span data-ttu-id="0fa0d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0fa0d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0fa0d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0fa0d-125">Accept</span></span>|<span data-ttu-id="0fa0d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0fa0d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fa0d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0fa0d-127">Request body</span></span>
<span data-ttu-id="0fa0d-128">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="0fa0d-128">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="0fa0d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="0fa0d-129">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="0fa0d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0fa0d-130">Property</span></span>|<span data-ttu-id="0fa0d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0fa0d-131">Type</span></span>|<span data-ttu-id="0fa0d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0fa0d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fa0d-133">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="0fa0d-133">azureStorageUri</span></span>|<span data-ttu-id="0fa0d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0fa0d-134">String</span></span>|<span data-ttu-id="0fa0d-135">O URI de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="0fa0d-135">The Azure Storage URI.</span></span>|
|<span data-ttu-id="0fa0d-136">isCommitted</span><span class="sxs-lookup"><span data-stu-id="0fa0d-136">isCommitted</span></span>|<span data-ttu-id="0fa0d-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="0fa0d-137">Boolean</span></span>|<span data-ttu-id="0fa0d-138">Um valor que indica se o arquivo tem está confirmado.</span><span class="sxs-lookup"><span data-stu-id="0fa0d-138">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="0fa0d-139">id</span><span class="sxs-lookup"><span data-stu-id="0fa0d-139">id</span></span>|<span data-ttu-id="0fa0d-140">String</span><span class="sxs-lookup"><span data-stu-id="0fa0d-140">String</span></span>|<span data-ttu-id="0fa0d-141">A ID do arquivo.</span><span class="sxs-lookup"><span data-stu-id="0fa0d-141">The File Id.</span></span>|
|<span data-ttu-id="0fa0d-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0fa0d-142">createdDateTime</span></span>|<span data-ttu-id="0fa0d-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fa0d-143">DateTimeOffset</span></span>|<span data-ttu-id="0fa0d-144">A hora em que o arquivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="0fa0d-144">The time the file was created.</span></span>|
|<span data-ttu-id="0fa0d-145">nome</span><span class="sxs-lookup"><span data-stu-id="0fa0d-145">name</span></span>|<span data-ttu-id="0fa0d-146">String</span><span class="sxs-lookup"><span data-stu-id="0fa0d-146">String</span></span>|<span data-ttu-id="0fa0d-147">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="0fa0d-147">the file name.</span></span>|
|<span data-ttu-id="0fa0d-148">size</span><span class="sxs-lookup"><span data-stu-id="0fa0d-148">size</span></span>|<span data-ttu-id="0fa0d-149">Int64</span><span class="sxs-lookup"><span data-stu-id="0fa0d-149">Int64</span></span>|<span data-ttu-id="0fa0d-150">O tamanho do arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="0fa0d-150">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="0fa0d-151">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="0fa0d-151">sizeEncrypted</span></span>|<span data-ttu-id="0fa0d-152">Int64</span><span class="sxs-lookup"><span data-stu-id="0fa0d-152">Int64</span></span>|<span data-ttu-id="0fa0d-153">O tamanho do arquivo após a criptografia.</span><span class="sxs-lookup"><span data-stu-id="0fa0d-153">The size of the file after encryption.</span></span>|
|<span data-ttu-id="0fa0d-154">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0fa0d-154">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="0fa0d-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fa0d-155">DateTimeOffset</span></span>|<span data-ttu-id="0fa0d-156">A hora de expiração do URI do armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="0fa0d-156">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="0fa0d-157">manifest</span><span class="sxs-lookup"><span data-stu-id="0fa0d-157">manifest</span></span>|<span data-ttu-id="0fa0d-158">Binária</span><span class="sxs-lookup"><span data-stu-id="0fa0d-158">Binary</span></span>|<span data-ttu-id="0fa0d-159">As informações do manifesto.</span><span class="sxs-lookup"><span data-stu-id="0fa0d-159">The manifest information.</span></span>|
|<span data-ttu-id="0fa0d-160">uploadState</span><span class="sxs-lookup"><span data-stu-id="0fa0d-160">uploadState</span></span>|[<span data-ttu-id="0fa0d-161">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="0fa0d-161">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="0fa0d-162">O estado da solicitação de carregamento atual.</span><span class="sxs-lookup"><span data-stu-id="0fa0d-162">The state of the current upload request.</span></span> <span data-ttu-id="0fa0d-163">Os valores possíveis são: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="0fa0d-163">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="0fa0d-164">isframeworkfile</span><span class="sxs-lookup"><span data-stu-id="0fa0d-164">isFrameworkFile</span></span>|<span data-ttu-id="0fa0d-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="0fa0d-165">Boolean</span></span>|<span data-ttu-id="0fa0d-166">Um valor que indica se o arquivo é um arquivo de estrutura.</span><span class="sxs-lookup"><span data-stu-id="0fa0d-166">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="0fa0d-167">IsDependency</span><span class="sxs-lookup"><span data-stu-id="0fa0d-167">isDependency</span></span>|<span data-ttu-id="0fa0d-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="0fa0d-168">Boolean</span></span>|<span data-ttu-id="0fa0d-169">Se o arquivo de conteúdo é uma dependência para o arquivo de conteúdo principal.</span><span class="sxs-lookup"><span data-stu-id="0fa0d-169">Whether the content file is a dependency for the main content file.</span></span>|



## <a name="response"></a><span data-ttu-id="0fa0d-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fa0d-170">Response</span></span>
<span data-ttu-id="0fa0d-171">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fa0d-171">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fa0d-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0fa0d-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="0fa0d-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fa0d-173">Request</span></span>
<span data-ttu-id="0fa0d-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fa0d-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0fa0d-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fa0d-175">Response</span></span>
<span data-ttu-id="0fa0d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0fa0d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





