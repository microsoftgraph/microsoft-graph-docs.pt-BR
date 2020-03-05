---
title: Atualizar mobileAppContentFile
description: Atualiza as propriedades de um objeto mobileAppContentFile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6ebcaabb809a0feaf95cd2baafcf56b48d7d3e69
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450724"
---
# <a name="update-mobileappcontentfile"></a><span data-ttu-id="4b6b3-103">Atualizar mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="4b6b3-103">Update mobileAppContentFile</span></span>

<span data-ttu-id="4b6b3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4b6b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b6b3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4b6b3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b6b3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4b6b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b6b3-107">Atualiza as propriedades de um objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="4b6b3-107">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b6b3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4b6b3-108">Prerequisites</span></span>
<span data-ttu-id="4b6b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b6b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b6b3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b6b3-111">Permission type</span></span>|<span data-ttu-id="4b6b3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4b6b3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b6b3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b6b3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b6b3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b6b3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4b6b3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b6b3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b6b3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b6b3-116">Not supported.</span></span>|
|<span data-ttu-id="4b6b3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b6b3-117">Application</span></span>|<span data-ttu-id="4b6b3-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b6b3-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b6b3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b6b3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="4b6b3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b6b3-120">Request headers</span></span>
|<span data-ttu-id="4b6b3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4b6b3-121">Header</span></span>|<span data-ttu-id="4b6b3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4b6b3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b6b3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b6b3-123">Authorization</span></span>|<span data-ttu-id="4b6b3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b6b3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b6b3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4b6b3-125">Accept</span></span>|<span data-ttu-id="4b6b3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b6b3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b6b3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b6b3-127">Request body</span></span>
<span data-ttu-id="4b6b3-128">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="4b6b3-128">In the request body, supply a JSON representation for the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

<span data-ttu-id="4b6b3-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="4b6b3-129">The following table shows the properties that are required when you create the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>

|<span data-ttu-id="4b6b3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b6b3-130">Property</span></span>|<span data-ttu-id="4b6b3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b6b3-131">Type</span></span>|<span data-ttu-id="4b6b3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b6b3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b6b3-133">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="4b6b3-133">azureStorageUri</span></span>|<span data-ttu-id="4b6b3-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b6b3-134">String</span></span>|<span data-ttu-id="4b6b3-135">O URI de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="4b6b3-135">The Azure Storage URI.</span></span>|
|<span data-ttu-id="4b6b3-136">isCommitted</span><span class="sxs-lookup"><span data-stu-id="4b6b3-136">isCommitted</span></span>|<span data-ttu-id="4b6b3-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="4b6b3-137">Boolean</span></span>|<span data-ttu-id="4b6b3-138">Um valor que indica se o arquivo tem está confirmado.</span><span class="sxs-lookup"><span data-stu-id="4b6b3-138">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="4b6b3-139">id</span><span class="sxs-lookup"><span data-stu-id="4b6b3-139">id</span></span>|<span data-ttu-id="4b6b3-140">String</span><span class="sxs-lookup"><span data-stu-id="4b6b3-140">String</span></span>|<span data-ttu-id="4b6b3-141">A ID do arquivo.</span><span class="sxs-lookup"><span data-stu-id="4b6b3-141">The File Id.</span></span>|
|<span data-ttu-id="4b6b3-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b6b3-142">createdDateTime</span></span>|<span data-ttu-id="4b6b3-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b6b3-143">DateTimeOffset</span></span>|<span data-ttu-id="4b6b3-144">A hora em que o arquivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="4b6b3-144">The time the file was created.</span></span>|
|<span data-ttu-id="4b6b3-145">nome</span><span class="sxs-lookup"><span data-stu-id="4b6b3-145">name</span></span>|<span data-ttu-id="4b6b3-146">String</span><span class="sxs-lookup"><span data-stu-id="4b6b3-146">String</span></span>|<span data-ttu-id="4b6b3-147">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="4b6b3-147">the file name.</span></span>|
|<span data-ttu-id="4b6b3-148">size</span><span class="sxs-lookup"><span data-stu-id="4b6b3-148">size</span></span>|<span data-ttu-id="4b6b3-149">Int64</span><span class="sxs-lookup"><span data-stu-id="4b6b3-149">Int64</span></span>|<span data-ttu-id="4b6b3-150">O tamanho do arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="4b6b3-150">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="4b6b3-151">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="4b6b3-151">sizeEncrypted</span></span>|<span data-ttu-id="4b6b3-152">Int64</span><span class="sxs-lookup"><span data-stu-id="4b6b3-152">Int64</span></span>|<span data-ttu-id="4b6b3-153">O tamanho do arquivo após a criptografia.</span><span class="sxs-lookup"><span data-stu-id="4b6b3-153">The size of the file after encryption.</span></span>|
|<span data-ttu-id="4b6b3-154">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4b6b3-154">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="4b6b3-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b6b3-155">DateTimeOffset</span></span>|<span data-ttu-id="4b6b3-156">A hora de expiração do URI do armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="4b6b3-156">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="4b6b3-157">manifest</span><span class="sxs-lookup"><span data-stu-id="4b6b3-157">manifest</span></span>|<span data-ttu-id="4b6b3-158">Binária</span><span class="sxs-lookup"><span data-stu-id="4b6b3-158">Binary</span></span>|<span data-ttu-id="4b6b3-159">As informações do manifesto.</span><span class="sxs-lookup"><span data-stu-id="4b6b3-159">The manifest information.</span></span>|
|<span data-ttu-id="4b6b3-160">uploadState</span><span class="sxs-lookup"><span data-stu-id="4b6b3-160">uploadState</span></span>|[<span data-ttu-id="4b6b3-161">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="4b6b3-161">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="4b6b3-162">O estado da solicitação de carregamento atual.</span><span class="sxs-lookup"><span data-stu-id="4b6b3-162">The state of the current upload request.</span></span> <span data-ttu-id="4b6b3-163">Os valores possíveis são: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="4b6b3-163">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="4b6b3-164">isframeworkfile</span><span class="sxs-lookup"><span data-stu-id="4b6b3-164">isFrameworkFile</span></span>|<span data-ttu-id="4b6b3-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b6b3-165">Boolean</span></span>|<span data-ttu-id="4b6b3-166">Um valor que indica se o arquivo é um arquivo de estrutura.</span><span class="sxs-lookup"><span data-stu-id="4b6b3-166">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="4b6b3-167">IsDependency</span><span class="sxs-lookup"><span data-stu-id="4b6b3-167">isDependency</span></span>|<span data-ttu-id="4b6b3-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b6b3-168">Boolean</span></span>|<span data-ttu-id="4b6b3-169">Se o arquivo de conteúdo é uma dependência para o arquivo de conteúdo principal.</span><span class="sxs-lookup"><span data-stu-id="4b6b3-169">Whether the content file is a dependency for the main content file.</span></span>|



## <a name="response"></a><span data-ttu-id="4b6b3-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b6b3-170">Response</span></span>
<span data-ttu-id="4b6b3-171">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b6b3-171">If successful, this method returns a `200 OK` response code and an updated [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b6b3-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b6b3-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b6b3-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b6b3-173">Request</span></span>
<span data-ttu-id="4b6b3-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b6b3-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4b6b3-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b6b3-175">Response</span></span>
<span data-ttu-id="4b6b3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4b6b3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





