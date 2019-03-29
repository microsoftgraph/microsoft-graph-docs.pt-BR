---
title: Criar mobileAppContentFile
description: Criar um novo objeto mobileAppContentFile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b6c78f6575a1d5f66e9989e876a03839ab2a8849
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957539"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="ee893-103">Criar mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="ee893-103">Create mobileAppContentFile</span></span>

> <span data-ttu-id="ee893-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ee893-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee893-105">Criar um novo objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="ee893-105">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee893-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ee893-106">Prerequisites</span></span>
<span data-ttu-id="ee893-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee893-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee893-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee893-109">Permission type</span></span>|<span data-ttu-id="ee893-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ee893-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee893-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee893-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ee893-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee893-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ee893-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee893-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee893-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee893-114">Not supported.</span></span>|
|<span data-ttu-id="ee893-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee893-115">Application</span></span>|<span data-ttu-id="ee893-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee893-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee893-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee893-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="ee893-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee893-118">Request headers</span></span>
|<span data-ttu-id="ee893-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ee893-119">Header</span></span>|<span data-ttu-id="ee893-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ee893-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee893-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee893-121">Authorization</span></span>|<span data-ttu-id="ee893-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee893-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee893-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ee893-123">Accept</span></span>|<span data-ttu-id="ee893-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ee893-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee893-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee893-125">Request body</span></span>
<span data-ttu-id="ee893-126">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="ee893-126">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="ee893-127">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="ee893-127">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="ee893-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee893-128">Property</span></span>|<span data-ttu-id="ee893-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee893-129">Type</span></span>|<span data-ttu-id="ee893-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee893-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee893-131">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="ee893-131">azureStorageUri</span></span>|<span data-ttu-id="ee893-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee893-132">String</span></span>|<span data-ttu-id="ee893-133">O URI de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="ee893-133">The Azure Storage URI.</span></span>|
|<span data-ttu-id="ee893-134">isCommitted</span><span class="sxs-lookup"><span data-stu-id="ee893-134">isCommitted</span></span>|<span data-ttu-id="ee893-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="ee893-135">Boolean</span></span>|<span data-ttu-id="ee893-136">Um valor que indica se o arquivo tem está confirmado.</span><span class="sxs-lookup"><span data-stu-id="ee893-136">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="ee893-137">id</span><span class="sxs-lookup"><span data-stu-id="ee893-137">id</span></span>|<span data-ttu-id="ee893-138">String</span><span class="sxs-lookup"><span data-stu-id="ee893-138">String</span></span>|<span data-ttu-id="ee893-139">A ID do arquivo.</span><span class="sxs-lookup"><span data-stu-id="ee893-139">The File Id.</span></span>|
|<span data-ttu-id="ee893-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ee893-140">createdDateTime</span></span>|<span data-ttu-id="ee893-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee893-141">DateTimeOffset</span></span>|<span data-ttu-id="ee893-142">A hora em que o arquivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="ee893-142">The time the file was created.</span></span>|
|<span data-ttu-id="ee893-143">name</span><span class="sxs-lookup"><span data-stu-id="ee893-143">name</span></span>|<span data-ttu-id="ee893-144">String</span><span class="sxs-lookup"><span data-stu-id="ee893-144">String</span></span>|<span data-ttu-id="ee893-145">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="ee893-145">the file name.</span></span>|
|<span data-ttu-id="ee893-146">size</span><span class="sxs-lookup"><span data-stu-id="ee893-146">size</span></span>|<span data-ttu-id="ee893-147">Int64</span><span class="sxs-lookup"><span data-stu-id="ee893-147">Int64</span></span>|<span data-ttu-id="ee893-148">O tamanho do arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="ee893-148">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="ee893-149">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="ee893-149">sizeEncrypted</span></span>|<span data-ttu-id="ee893-150">Int64</span><span class="sxs-lookup"><span data-stu-id="ee893-150">Int64</span></span>|<span data-ttu-id="ee893-151">O tamanho do arquivo após a criptografia.</span><span class="sxs-lookup"><span data-stu-id="ee893-151">The size of the file after encryption.</span></span>|
|<span data-ttu-id="ee893-152">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ee893-152">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="ee893-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee893-153">DateTimeOffset</span></span>|<span data-ttu-id="ee893-154">A hora de expiração do URI do armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="ee893-154">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="ee893-155">manifest</span><span class="sxs-lookup"><span data-stu-id="ee893-155">manifest</span></span>|<span data-ttu-id="ee893-156">Binária</span><span class="sxs-lookup"><span data-stu-id="ee893-156">Binary</span></span>|<span data-ttu-id="ee893-157">As informações do manifesto.</span><span class="sxs-lookup"><span data-stu-id="ee893-157">The manifest information.</span></span>|
|<span data-ttu-id="ee893-158">uploadState</span><span class="sxs-lookup"><span data-stu-id="ee893-158">uploadState</span></span>|[<span data-ttu-id="ee893-159">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="ee893-159">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="ee893-160">O estado da solicitação de carregamento atual.</span><span class="sxs-lookup"><span data-stu-id="ee893-160">The state of the current upload request.</span></span> <span data-ttu-id="ee893-161">Os valores possíveis são: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="ee893-161">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="ee893-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee893-162">Response</span></span>
<span data-ttu-id="ee893-163">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee893-163">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee893-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee893-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee893-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee893-165">Request</span></span>
<span data-ttu-id="ee893-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee893-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ee893-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee893-167">Response</span></span>
<span data-ttu-id="ee893-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ee893-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



