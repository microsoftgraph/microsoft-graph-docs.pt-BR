---
title: Criar mobileAppContentFile
description: Criar um novo objeto mobileAppContentFile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 28d8ff58b4808e44cbcd2278c7e4169f4c2ccb03
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515943"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="bea72-103">Criar mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="bea72-103">Create mobileAppContentFile</span></span>

<span data-ttu-id="bea72-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bea72-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bea72-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bea72-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bea72-106">Criar um novo objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="bea72-106">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bea72-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bea72-107">Prerequisites</span></span>
<span data-ttu-id="bea72-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bea72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bea72-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bea72-110">Permission type</span></span>|<span data-ttu-id="bea72-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bea72-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bea72-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bea72-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bea72-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bea72-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bea72-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bea72-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bea72-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bea72-115">Not supported.</span></span>|
|<span data-ttu-id="bea72-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bea72-116">Application</span></span>|<span data-ttu-id="bea72-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bea72-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bea72-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bea72-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="bea72-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bea72-119">Request headers</span></span>
|<span data-ttu-id="bea72-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bea72-120">Header</span></span>|<span data-ttu-id="bea72-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bea72-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bea72-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bea72-122">Authorization</span></span>|<span data-ttu-id="bea72-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bea72-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bea72-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bea72-124">Accept</span></span>|<span data-ttu-id="bea72-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bea72-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bea72-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bea72-126">Request body</span></span>
<span data-ttu-id="bea72-127">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="bea72-127">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="bea72-128">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="bea72-128">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="bea72-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bea72-129">Property</span></span>|<span data-ttu-id="bea72-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="bea72-130">Type</span></span>|<span data-ttu-id="bea72-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="bea72-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bea72-132">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="bea72-132">azureStorageUri</span></span>|<span data-ttu-id="bea72-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bea72-133">String</span></span>|<span data-ttu-id="bea72-134">O URI de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="bea72-134">The Azure Storage URI.</span></span>|
|<span data-ttu-id="bea72-135">isCommitted</span><span class="sxs-lookup"><span data-stu-id="bea72-135">isCommitted</span></span>|<span data-ttu-id="bea72-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="bea72-136">Boolean</span></span>|<span data-ttu-id="bea72-137">Um valor que indica se o arquivo tem está confirmado.</span><span class="sxs-lookup"><span data-stu-id="bea72-137">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="bea72-138">id</span><span class="sxs-lookup"><span data-stu-id="bea72-138">id</span></span>|<span data-ttu-id="bea72-139">String</span><span class="sxs-lookup"><span data-stu-id="bea72-139">String</span></span>|<span data-ttu-id="bea72-140">A ID do arquivo.</span><span class="sxs-lookup"><span data-stu-id="bea72-140">The File Id.</span></span>|
|<span data-ttu-id="bea72-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bea72-141">createdDateTime</span></span>|<span data-ttu-id="bea72-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bea72-142">DateTimeOffset</span></span>|<span data-ttu-id="bea72-143">A hora em que o arquivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="bea72-143">The time the file was created.</span></span>|
|<span data-ttu-id="bea72-144">nome</span><span class="sxs-lookup"><span data-stu-id="bea72-144">name</span></span>|<span data-ttu-id="bea72-145">String</span><span class="sxs-lookup"><span data-stu-id="bea72-145">String</span></span>|<span data-ttu-id="bea72-146">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="bea72-146">the file name.</span></span>|
|<span data-ttu-id="bea72-147">size</span><span class="sxs-lookup"><span data-stu-id="bea72-147">size</span></span>|<span data-ttu-id="bea72-148">Int64</span><span class="sxs-lookup"><span data-stu-id="bea72-148">Int64</span></span>|<span data-ttu-id="bea72-149">O tamanho do arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="bea72-149">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="bea72-150">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="bea72-150">sizeEncrypted</span></span>|<span data-ttu-id="bea72-151">Int64</span><span class="sxs-lookup"><span data-stu-id="bea72-151">Int64</span></span>|<span data-ttu-id="bea72-152">O tamanho do arquivo após a criptografia.</span><span class="sxs-lookup"><span data-stu-id="bea72-152">The size of the file after encryption.</span></span>|
|<span data-ttu-id="bea72-153">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bea72-153">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="bea72-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bea72-154">DateTimeOffset</span></span>|<span data-ttu-id="bea72-155">A hora de expiração do URI do armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="bea72-155">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="bea72-156">manifest</span><span class="sxs-lookup"><span data-stu-id="bea72-156">manifest</span></span>|<span data-ttu-id="bea72-157">Binária</span><span class="sxs-lookup"><span data-stu-id="bea72-157">Binary</span></span>|<span data-ttu-id="bea72-158">As informações do manifesto.</span><span class="sxs-lookup"><span data-stu-id="bea72-158">The manifest information.</span></span>|
|<span data-ttu-id="bea72-159">uploadState</span><span class="sxs-lookup"><span data-stu-id="bea72-159">uploadState</span></span>|[<span data-ttu-id="bea72-160">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="bea72-160">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="bea72-161">O estado da solicitação de carregamento atual.</span><span class="sxs-lookup"><span data-stu-id="bea72-161">The state of the current upload request.</span></span> <span data-ttu-id="bea72-162">Os valores possíveis são: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="bea72-162">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="bea72-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="bea72-163">Response</span></span>
<span data-ttu-id="bea72-164">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bea72-164">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bea72-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bea72-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="bea72-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bea72-166">Request</span></span>
<span data-ttu-id="bea72-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bea72-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bea72-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="bea72-168">Response</span></span>
<span data-ttu-id="bea72-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bea72-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




