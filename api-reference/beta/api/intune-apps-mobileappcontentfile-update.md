---
title: Atualizar mobileAppContentFile
description: Atualiza as propriedades de um objeto mobileAppContentFile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 100ba93f87bd210a7e1dcc6a22816e7b3e27f7de
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39935376"
---
# <a name="update-mobileappcontentfile"></a><span data-ttu-id="c4866-103">Atualizar mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="c4866-103">Update mobileAppContentFile</span></span>

> <span data-ttu-id="c4866-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c4866-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4866-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c4866-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4866-106">Atualiza as propriedades de um objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="c4866-106">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4866-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c4866-107">Prerequisites</span></span>
<span data-ttu-id="c4866-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4866-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4866-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4866-110">Permission type</span></span>|<span data-ttu-id="c4866-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c4866-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4866-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4866-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c4866-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4866-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c4866-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4866-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4866-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4866-115">Not supported.</span></span>|
|<span data-ttu-id="c4866-116">Application</span><span class="sxs-lookup"><span data-stu-id="c4866-116">Application</span></span>|<span data-ttu-id="c4866-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4866-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4866-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4866-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="c4866-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4866-119">Request headers</span></span>
|<span data-ttu-id="c4866-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c4866-120">Header</span></span>|<span data-ttu-id="c4866-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c4866-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4866-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4866-122">Authorization</span></span>|<span data-ttu-id="c4866-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4866-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4866-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c4866-124">Accept</span></span>|<span data-ttu-id="c4866-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c4866-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4866-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4866-126">Request body</span></span>
<span data-ttu-id="c4866-127">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="c4866-127">In the request body, supply a JSON representation for the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

<span data-ttu-id="c4866-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="c4866-128">The following table shows the properties that are required when you create the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>

|<span data-ttu-id="c4866-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4866-129">Property</span></span>|<span data-ttu-id="c4866-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4866-130">Type</span></span>|<span data-ttu-id="c4866-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4866-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4866-132">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="c4866-132">azureStorageUri</span></span>|<span data-ttu-id="c4866-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4866-133">String</span></span>|<span data-ttu-id="c4866-134">O URI de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="c4866-134">The Azure Storage URI.</span></span>|
|<span data-ttu-id="c4866-135">isCommitted</span><span class="sxs-lookup"><span data-stu-id="c4866-135">isCommitted</span></span>|<span data-ttu-id="c4866-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="c4866-136">Boolean</span></span>|<span data-ttu-id="c4866-137">Um valor que indica se o arquivo tem está confirmado.</span><span class="sxs-lookup"><span data-stu-id="c4866-137">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="c4866-138">id</span><span class="sxs-lookup"><span data-stu-id="c4866-138">id</span></span>|<span data-ttu-id="c4866-139">String</span><span class="sxs-lookup"><span data-stu-id="c4866-139">String</span></span>|<span data-ttu-id="c4866-140">A ID do arquivo.</span><span class="sxs-lookup"><span data-stu-id="c4866-140">The File Id.</span></span>|
|<span data-ttu-id="c4866-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c4866-141">createdDateTime</span></span>|<span data-ttu-id="c4866-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4866-142">DateTimeOffset</span></span>|<span data-ttu-id="c4866-143">A hora em que o arquivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="c4866-143">The time the file was created.</span></span>|
|<span data-ttu-id="c4866-144">name</span><span class="sxs-lookup"><span data-stu-id="c4866-144">name</span></span>|<span data-ttu-id="c4866-145">String</span><span class="sxs-lookup"><span data-stu-id="c4866-145">String</span></span>|<span data-ttu-id="c4866-146">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="c4866-146">the file name.</span></span>|
|<span data-ttu-id="c4866-147">size</span><span class="sxs-lookup"><span data-stu-id="c4866-147">size</span></span>|<span data-ttu-id="c4866-148">Int64</span><span class="sxs-lookup"><span data-stu-id="c4866-148">Int64</span></span>|<span data-ttu-id="c4866-149">O tamanho do arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="c4866-149">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="c4866-150">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="c4866-150">sizeEncrypted</span></span>|<span data-ttu-id="c4866-151">Int64</span><span class="sxs-lookup"><span data-stu-id="c4866-151">Int64</span></span>|<span data-ttu-id="c4866-152">O tamanho do arquivo após a criptografia.</span><span class="sxs-lookup"><span data-stu-id="c4866-152">The size of the file after encryption.</span></span>|
|<span data-ttu-id="c4866-153">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c4866-153">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="c4866-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4866-154">DateTimeOffset</span></span>|<span data-ttu-id="c4866-155">A hora de expiração do URI do armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="c4866-155">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="c4866-156">manifest</span><span class="sxs-lookup"><span data-stu-id="c4866-156">manifest</span></span>|<span data-ttu-id="c4866-157">Binária</span><span class="sxs-lookup"><span data-stu-id="c4866-157">Binary</span></span>|<span data-ttu-id="c4866-158">As informações do manifesto.</span><span class="sxs-lookup"><span data-stu-id="c4866-158">The manifest information.</span></span>|
|<span data-ttu-id="c4866-159">uploadState</span><span class="sxs-lookup"><span data-stu-id="c4866-159">uploadState</span></span>|[<span data-ttu-id="c4866-160">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="c4866-160">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="c4866-161">O estado da solicitação de carregamento atual.</span><span class="sxs-lookup"><span data-stu-id="c4866-161">The state of the current upload request.</span></span> <span data-ttu-id="c4866-162">Os valores possíveis são: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="c4866-162">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="c4866-163">isframeworkfile</span><span class="sxs-lookup"><span data-stu-id="c4866-163">isFrameworkFile</span></span>|<span data-ttu-id="c4866-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4866-164">Boolean</span></span>|<span data-ttu-id="c4866-165">Um valor que indica se o arquivo é um arquivo de estrutura.</span><span class="sxs-lookup"><span data-stu-id="c4866-165">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="c4866-166">IsDependency</span><span class="sxs-lookup"><span data-stu-id="c4866-166">isDependency</span></span>|<span data-ttu-id="c4866-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4866-167">Boolean</span></span>|<span data-ttu-id="c4866-168">Se o arquivo de conteúdo é uma dependência para o arquivo de conteúdo principal.</span><span class="sxs-lookup"><span data-stu-id="c4866-168">Whether the content file is a dependency for the main content file.</span></span>|



## <a name="response"></a><span data-ttu-id="c4866-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4866-169">Response</span></span>
<span data-ttu-id="c4866-170">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4866-170">If successful, this method returns a `200 OK` response code and an updated [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4866-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4866-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4866-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4866-172">Request</span></span>
<span data-ttu-id="c4866-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4866-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c4866-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4866-174">Response</span></span>
<span data-ttu-id="c4866-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4866-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





