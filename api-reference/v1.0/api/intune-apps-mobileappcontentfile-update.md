---
title: Atualizar mobileAppContentFile
description: Atualiza as propriedades de um objeto mobileAppContentFile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a5a88759c531c8350aafdb62de10c49afa83d37
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253824"
---
# <a name="update-mobileappcontentfile"></a><span data-ttu-id="409b6-103">Atualizar mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="409b6-103">Update mobileAppContentFile</span></span>

> <span data-ttu-id="409b6-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="409b6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="409b6-105">Atualiza as propriedades de um objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="409b6-105">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="409b6-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="409b6-106">Prerequisites</span></span>
<span data-ttu-id="409b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="409b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="409b6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="409b6-109">Permission type</span></span>|<span data-ttu-id="409b6-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="409b6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="409b6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="409b6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="409b6-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="409b6-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="409b6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="409b6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="409b6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="409b6-114">Not supported.</span></span>|
|<span data-ttu-id="409b6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="409b6-115">Application</span></span>|<span data-ttu-id="409b6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="409b6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="409b6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="409b6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="409b6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="409b6-118">Request headers</span></span>
|<span data-ttu-id="409b6-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="409b6-119">Header</span></span>|<span data-ttu-id="409b6-120">Valor</span><span class="sxs-lookup"><span data-stu-id="409b6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="409b6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="409b6-121">Authorization</span></span>|<span data-ttu-id="409b6-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="409b6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="409b6-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="409b6-123">Accept</span></span>|<span data-ttu-id="409b6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="409b6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="409b6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="409b6-125">Request body</span></span>
<span data-ttu-id="409b6-126">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="409b6-126">In the request body, supply a JSON representation for the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

<span data-ttu-id="409b6-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="409b6-127">The following table shows the properties that are required when you create the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>

|<span data-ttu-id="409b6-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="409b6-128">Property</span></span>|<span data-ttu-id="409b6-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="409b6-129">Type</span></span>|<span data-ttu-id="409b6-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="409b6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="409b6-131">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="409b6-131">azureStorageUri</span></span>|<span data-ttu-id="409b6-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="409b6-132">String</span></span>|<span data-ttu-id="409b6-133">O URI de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="409b6-133">The Azure Storage URI.</span></span>|
|<span data-ttu-id="409b6-134">isCommitted</span><span class="sxs-lookup"><span data-stu-id="409b6-134">isCommitted</span></span>|<span data-ttu-id="409b6-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="409b6-135">Boolean</span></span>|<span data-ttu-id="409b6-136">Um valor que indica se o arquivo tem está confirmado.</span><span class="sxs-lookup"><span data-stu-id="409b6-136">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="409b6-137">id</span><span class="sxs-lookup"><span data-stu-id="409b6-137">id</span></span>|<span data-ttu-id="409b6-138">String</span><span class="sxs-lookup"><span data-stu-id="409b6-138">String</span></span>|<span data-ttu-id="409b6-139">A ID do arquivo.</span><span class="sxs-lookup"><span data-stu-id="409b6-139">The File Id.</span></span>|
|<span data-ttu-id="409b6-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="409b6-140">createdDateTime</span></span>|<span data-ttu-id="409b6-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="409b6-141">DateTimeOffset</span></span>|<span data-ttu-id="409b6-142">A hora em que o arquivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="409b6-142">The time the file was created.</span></span>|
|<span data-ttu-id="409b6-143">name</span><span class="sxs-lookup"><span data-stu-id="409b6-143">name</span></span>|<span data-ttu-id="409b6-144">String</span><span class="sxs-lookup"><span data-stu-id="409b6-144">String</span></span>|<span data-ttu-id="409b6-145">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="409b6-145">the file name.</span></span>|
|<span data-ttu-id="409b6-146">size</span><span class="sxs-lookup"><span data-stu-id="409b6-146">size</span></span>|<span data-ttu-id="409b6-147">Int64</span><span class="sxs-lookup"><span data-stu-id="409b6-147">Int64</span></span>|<span data-ttu-id="409b6-148">O tamanho do arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="409b6-148">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="409b6-149">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="409b6-149">sizeEncrypted</span></span>|<span data-ttu-id="409b6-150">Int64</span><span class="sxs-lookup"><span data-stu-id="409b6-150">Int64</span></span>|<span data-ttu-id="409b6-151">O tamanho do arquivo após a criptografia.</span><span class="sxs-lookup"><span data-stu-id="409b6-151">The size of the file after encryption.</span></span>|
|<span data-ttu-id="409b6-152">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="409b6-152">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="409b6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="409b6-153">DateTimeOffset</span></span>|<span data-ttu-id="409b6-154">A hora de expiração do URI do armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="409b6-154">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="409b6-155">manifest</span><span class="sxs-lookup"><span data-stu-id="409b6-155">manifest</span></span>|<span data-ttu-id="409b6-156">Binária</span><span class="sxs-lookup"><span data-stu-id="409b6-156">Binary</span></span>|<span data-ttu-id="409b6-157">As informações do manifesto.</span><span class="sxs-lookup"><span data-stu-id="409b6-157">The manifest information.</span></span>|
|<span data-ttu-id="409b6-158">uploadState</span><span class="sxs-lookup"><span data-stu-id="409b6-158">uploadState</span></span>|[<span data-ttu-id="409b6-159">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="409b6-159">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="409b6-160">O estado da solicitação de carregamento atual.</span><span class="sxs-lookup"><span data-stu-id="409b6-160">The state of the current upload request.</span></span> <span data-ttu-id="409b6-161">Os valores possíveis são: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="409b6-161">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="409b6-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="409b6-162">Response</span></span>
<span data-ttu-id="409b6-163">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="409b6-163">If successful, this method returns a `200 OK` response code and an updated [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="409b6-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="409b6-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="409b6-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="409b6-165">Request</span></span>
<span data-ttu-id="409b6-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="409b6-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="409b6-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="409b6-167">Response</span></span>
<span data-ttu-id="409b6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="409b6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



