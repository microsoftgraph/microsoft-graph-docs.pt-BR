---
title: Atualizar mobileAppContentFile
description: Atualiza as propriedades de um objeto mobileAppContentFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1e2d577685e2f1764446993486d1a3d845d4824a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758747"
---
# <a name="update-mobileappcontentfile"></a><span data-ttu-id="c3898-103">Atualizar mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="c3898-103">Update mobileAppContentFile</span></span>

<span data-ttu-id="c3898-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3898-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3898-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c3898-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3898-106">Atualiza as propriedades de um objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="c3898-106">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3898-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c3898-107">Prerequisites</span></span>
<span data-ttu-id="c3898-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3898-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3898-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3898-110">Permission type</span></span>|<span data-ttu-id="c3898-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3898-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3898-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3898-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c3898-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3898-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c3898-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3898-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3898-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3898-115">Not supported.</span></span>|
|<span data-ttu-id="c3898-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3898-116">Application</span></span>|<span data-ttu-id="c3898-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3898-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3898-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3898-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="c3898-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3898-119">Request headers</span></span>
|<span data-ttu-id="c3898-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c3898-120">Header</span></span>|<span data-ttu-id="c3898-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c3898-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3898-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3898-122">Authorization</span></span>|<span data-ttu-id="c3898-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3898-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3898-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c3898-124">Accept</span></span>|<span data-ttu-id="c3898-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c3898-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3898-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3898-126">Request body</span></span>
<span data-ttu-id="c3898-127">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="c3898-127">In the request body, supply a JSON representation for the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

<span data-ttu-id="c3898-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="c3898-128">The following table shows the properties that are required when you create the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>

|<span data-ttu-id="c3898-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3898-129">Property</span></span>|<span data-ttu-id="c3898-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3898-130">Type</span></span>|<span data-ttu-id="c3898-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3898-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3898-132">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="c3898-132">azureStorageUri</span></span>|<span data-ttu-id="c3898-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3898-133">String</span></span>|<span data-ttu-id="c3898-134">O URI de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="c3898-134">The Azure Storage URI.</span></span>|
|<span data-ttu-id="c3898-135">isCommitted</span><span class="sxs-lookup"><span data-stu-id="c3898-135">isCommitted</span></span>|<span data-ttu-id="c3898-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="c3898-136">Boolean</span></span>|<span data-ttu-id="c3898-137">Um valor que indica se o arquivo tem está confirmado.</span><span class="sxs-lookup"><span data-stu-id="c3898-137">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="c3898-138">id</span><span class="sxs-lookup"><span data-stu-id="c3898-138">id</span></span>|<span data-ttu-id="c3898-139">String</span><span class="sxs-lookup"><span data-stu-id="c3898-139">String</span></span>|<span data-ttu-id="c3898-140">A ID do arquivo.</span><span class="sxs-lookup"><span data-stu-id="c3898-140">The File Id.</span></span>|
|<span data-ttu-id="c3898-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3898-141">createdDateTime</span></span>|<span data-ttu-id="c3898-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3898-142">DateTimeOffset</span></span>|<span data-ttu-id="c3898-143">A hora em que o arquivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="c3898-143">The time the file was created.</span></span>|
|<span data-ttu-id="c3898-144">nome</span><span class="sxs-lookup"><span data-stu-id="c3898-144">name</span></span>|<span data-ttu-id="c3898-145">String</span><span class="sxs-lookup"><span data-stu-id="c3898-145">String</span></span>|<span data-ttu-id="c3898-146">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="c3898-146">the file name.</span></span>|
|<span data-ttu-id="c3898-147">size</span><span class="sxs-lookup"><span data-stu-id="c3898-147">size</span></span>|<span data-ttu-id="c3898-148">Int64</span><span class="sxs-lookup"><span data-stu-id="c3898-148">Int64</span></span>|<span data-ttu-id="c3898-149">O tamanho do arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="c3898-149">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="c3898-150">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="c3898-150">sizeEncrypted</span></span>|<span data-ttu-id="c3898-151">Int64</span><span class="sxs-lookup"><span data-stu-id="c3898-151">Int64</span></span>|<span data-ttu-id="c3898-152">O tamanho do arquivo após a criptografia.</span><span class="sxs-lookup"><span data-stu-id="c3898-152">The size of the file after encryption.</span></span>|
|<span data-ttu-id="c3898-153">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c3898-153">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="c3898-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3898-154">DateTimeOffset</span></span>|<span data-ttu-id="c3898-155">A hora de expiração do URI do armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="c3898-155">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="c3898-156">manifest</span><span class="sxs-lookup"><span data-stu-id="c3898-156">manifest</span></span>|<span data-ttu-id="c3898-157">Binária</span><span class="sxs-lookup"><span data-stu-id="c3898-157">Binary</span></span>|<span data-ttu-id="c3898-158">As informações do manifesto.</span><span class="sxs-lookup"><span data-stu-id="c3898-158">The manifest information.</span></span>|
|<span data-ttu-id="c3898-159">uploadState</span><span class="sxs-lookup"><span data-stu-id="c3898-159">uploadState</span></span>|[<span data-ttu-id="c3898-160">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="c3898-160">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="c3898-161">O estado da solicitação de carregamento atual.</span><span class="sxs-lookup"><span data-stu-id="c3898-161">The state of the current upload request.</span></span> <span data-ttu-id="c3898-162">Os valores possíveis são: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="c3898-162">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="c3898-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3898-163">Response</span></span>
<span data-ttu-id="c3898-164">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3898-164">If successful, this method returns a `200 OK` response code and an updated [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3898-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c3898-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3898-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3898-166">Request</span></span>
<span data-ttu-id="c3898-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3898-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
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

### <a name="response"></a><span data-ttu-id="c3898-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3898-168">Response</span></span>
<span data-ttu-id="c3898-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c3898-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




