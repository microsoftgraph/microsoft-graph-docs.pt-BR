---
title: Criar mobileAppContentFile
description: Criar um novo objeto mobileAppContentFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c1b525eefdf6349217aaa05a94f2d21849b59a89
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759683"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="442c5-103">Criar mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="442c5-103">Create mobileAppContentFile</span></span>

<span data-ttu-id="442c5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="442c5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="442c5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="442c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="442c5-106">Criar um novo objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="442c5-106">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="442c5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="442c5-107">Prerequisites</span></span>
<span data-ttu-id="442c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="442c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="442c5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="442c5-110">Permission type</span></span>|<span data-ttu-id="442c5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="442c5-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="442c5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="442c5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="442c5-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="442c5-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="442c5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="442c5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="442c5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="442c5-115">Not supported.</span></span>|
|<span data-ttu-id="442c5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="442c5-116">Application</span></span>|<span data-ttu-id="442c5-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="442c5-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="442c5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="442c5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="442c5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="442c5-119">Request headers</span></span>
|<span data-ttu-id="442c5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="442c5-120">Header</span></span>|<span data-ttu-id="442c5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="442c5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="442c5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="442c5-122">Authorization</span></span>|<span data-ttu-id="442c5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="442c5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="442c5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="442c5-124">Accept</span></span>|<span data-ttu-id="442c5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="442c5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="442c5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="442c5-126">Request body</span></span>
<span data-ttu-id="442c5-127">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="442c5-127">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="442c5-128">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="442c5-128">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="442c5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="442c5-129">Property</span></span>|<span data-ttu-id="442c5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="442c5-130">Type</span></span>|<span data-ttu-id="442c5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="442c5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="442c5-132">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="442c5-132">azureStorageUri</span></span>|<span data-ttu-id="442c5-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="442c5-133">String</span></span>|<span data-ttu-id="442c5-134">O URI de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="442c5-134">The Azure Storage URI.</span></span>|
|<span data-ttu-id="442c5-135">isCommitted</span><span class="sxs-lookup"><span data-stu-id="442c5-135">isCommitted</span></span>|<span data-ttu-id="442c5-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="442c5-136">Boolean</span></span>|<span data-ttu-id="442c5-137">Um valor que indica se o arquivo tem está confirmado.</span><span class="sxs-lookup"><span data-stu-id="442c5-137">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="442c5-138">id</span><span class="sxs-lookup"><span data-stu-id="442c5-138">id</span></span>|<span data-ttu-id="442c5-139">String</span><span class="sxs-lookup"><span data-stu-id="442c5-139">String</span></span>|<span data-ttu-id="442c5-140">A ID do arquivo.</span><span class="sxs-lookup"><span data-stu-id="442c5-140">The File Id.</span></span>|
|<span data-ttu-id="442c5-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="442c5-141">createdDateTime</span></span>|<span data-ttu-id="442c5-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="442c5-142">DateTimeOffset</span></span>|<span data-ttu-id="442c5-143">A hora em que o arquivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="442c5-143">The time the file was created.</span></span>|
|<span data-ttu-id="442c5-144">nome</span><span class="sxs-lookup"><span data-stu-id="442c5-144">name</span></span>|<span data-ttu-id="442c5-145">String</span><span class="sxs-lookup"><span data-stu-id="442c5-145">String</span></span>|<span data-ttu-id="442c5-146">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="442c5-146">the file name.</span></span>|
|<span data-ttu-id="442c5-147">size</span><span class="sxs-lookup"><span data-stu-id="442c5-147">size</span></span>|<span data-ttu-id="442c5-148">Int64</span><span class="sxs-lookup"><span data-stu-id="442c5-148">Int64</span></span>|<span data-ttu-id="442c5-149">O tamanho do arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="442c5-149">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="442c5-150">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="442c5-150">sizeEncrypted</span></span>|<span data-ttu-id="442c5-151">Int64</span><span class="sxs-lookup"><span data-stu-id="442c5-151">Int64</span></span>|<span data-ttu-id="442c5-152">O tamanho do arquivo após a criptografia.</span><span class="sxs-lookup"><span data-stu-id="442c5-152">The size of the file after encryption.</span></span>|
|<span data-ttu-id="442c5-153">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="442c5-153">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="442c5-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="442c5-154">DateTimeOffset</span></span>|<span data-ttu-id="442c5-155">A hora de expiração do URI do armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="442c5-155">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="442c5-156">manifest</span><span class="sxs-lookup"><span data-stu-id="442c5-156">manifest</span></span>|<span data-ttu-id="442c5-157">Binária</span><span class="sxs-lookup"><span data-stu-id="442c5-157">Binary</span></span>|<span data-ttu-id="442c5-158">As informações do manifesto.</span><span class="sxs-lookup"><span data-stu-id="442c5-158">The manifest information.</span></span>|
|<span data-ttu-id="442c5-159">uploadState</span><span class="sxs-lookup"><span data-stu-id="442c5-159">uploadState</span></span>|[<span data-ttu-id="442c5-160">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="442c5-160">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="442c5-161">O estado da solicitação de carregamento atual.</span><span class="sxs-lookup"><span data-stu-id="442c5-161">The state of the current upload request.</span></span> <span data-ttu-id="442c5-162">Os valores possíveis são: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="442c5-162">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="442c5-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="442c5-163">Response</span></span>
<span data-ttu-id="442c5-164">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="442c5-164">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="442c5-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="442c5-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="442c5-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="442c5-166">Request</span></span>
<span data-ttu-id="442c5-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="442c5-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError"
}
```

### <a name="response"></a><span data-ttu-id="442c5-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="442c5-168">Response</span></span>
<span data-ttu-id="442c5-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="442c5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 450

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
  "uploadState": "transientError"
}
```




