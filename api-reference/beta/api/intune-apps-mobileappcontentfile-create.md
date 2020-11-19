---
title: Criar mobileAppContentFile
description: Criar um novo objeto mobileAppContentFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8b81d338601629cbf2de871907d5e9245a500196
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49248767"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="f6bc6-103">Criar mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="f6bc6-103">Create mobileAppContentFile</span></span>

<span data-ttu-id="f6bc6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6bc6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6bc6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f6bc6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6bc6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f6bc6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6bc6-107">Criar um novo objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="f6bc6-107">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6bc6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f6bc6-108">Prerequisites</span></span>
<span data-ttu-id="f6bc6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6bc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6bc6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6bc6-111">Permission type</span></span>|<span data-ttu-id="f6bc6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f6bc6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6bc6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6bc6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f6bc6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6bc6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f6bc6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6bc6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6bc6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6bc6-116">Not supported.</span></span>|
|<span data-ttu-id="f6bc6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6bc6-117">Application</span></span>|<span data-ttu-id="f6bc6-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6bc6-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6bc6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6bc6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="f6bc6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6bc6-120">Request headers</span></span>
|<span data-ttu-id="f6bc6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f6bc6-121">Header</span></span>|<span data-ttu-id="f6bc6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f6bc6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6bc6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6bc6-123">Authorization</span></span>|<span data-ttu-id="f6bc6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6bc6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6bc6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f6bc6-125">Accept</span></span>|<span data-ttu-id="f6bc6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f6bc6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6bc6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6bc6-127">Request body</span></span>
<span data-ttu-id="f6bc6-128">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="f6bc6-128">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="f6bc6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="f6bc6-129">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="f6bc6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f6bc6-130">Property</span></span>|<span data-ttu-id="f6bc6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6bc6-131">Type</span></span>|<span data-ttu-id="f6bc6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6bc6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6bc6-133">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="f6bc6-133">azureStorageUri</span></span>|<span data-ttu-id="f6bc6-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6bc6-134">String</span></span>|<span data-ttu-id="f6bc6-135">O URI de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="f6bc6-135">The Azure Storage URI.</span></span>|
|<span data-ttu-id="f6bc6-136">isCommitted</span><span class="sxs-lookup"><span data-stu-id="f6bc6-136">isCommitted</span></span>|<span data-ttu-id="f6bc6-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="f6bc6-137">Boolean</span></span>|<span data-ttu-id="f6bc6-138">Um valor que indica se o arquivo tem está confirmado.</span><span class="sxs-lookup"><span data-stu-id="f6bc6-138">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="f6bc6-139">id</span><span class="sxs-lookup"><span data-stu-id="f6bc6-139">id</span></span>|<span data-ttu-id="f6bc6-140">String</span><span class="sxs-lookup"><span data-stu-id="f6bc6-140">String</span></span>|<span data-ttu-id="f6bc6-141">A ID do arquivo.</span><span class="sxs-lookup"><span data-stu-id="f6bc6-141">The File Id.</span></span>|
|<span data-ttu-id="f6bc6-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f6bc6-142">createdDateTime</span></span>|<span data-ttu-id="f6bc6-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6bc6-143">DateTimeOffset</span></span>|<span data-ttu-id="f6bc6-144">A hora em que o arquivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="f6bc6-144">The time the file was created.</span></span>|
|<span data-ttu-id="f6bc6-145">nome</span><span class="sxs-lookup"><span data-stu-id="f6bc6-145">name</span></span>|<span data-ttu-id="f6bc6-146">String</span><span class="sxs-lookup"><span data-stu-id="f6bc6-146">String</span></span>|<span data-ttu-id="f6bc6-147">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="f6bc6-147">the file name.</span></span>|
|<span data-ttu-id="f6bc6-148">size</span><span class="sxs-lookup"><span data-stu-id="f6bc6-148">size</span></span>|<span data-ttu-id="f6bc6-149">Int64</span><span class="sxs-lookup"><span data-stu-id="f6bc6-149">Int64</span></span>|<span data-ttu-id="f6bc6-150">O tamanho do arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="f6bc6-150">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="f6bc6-151">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="f6bc6-151">sizeEncrypted</span></span>|<span data-ttu-id="f6bc6-152">Int64</span><span class="sxs-lookup"><span data-stu-id="f6bc6-152">Int64</span></span>|<span data-ttu-id="f6bc6-153">O tamanho do arquivo após a criptografia.</span><span class="sxs-lookup"><span data-stu-id="f6bc6-153">The size of the file after encryption.</span></span>|
|<span data-ttu-id="f6bc6-154">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f6bc6-154">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="f6bc6-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6bc6-155">DateTimeOffset</span></span>|<span data-ttu-id="f6bc6-156">A hora de expiração do URI do armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="f6bc6-156">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="f6bc6-157">manifest</span><span class="sxs-lookup"><span data-stu-id="f6bc6-157">manifest</span></span>|<span data-ttu-id="f6bc6-158">Binária</span><span class="sxs-lookup"><span data-stu-id="f6bc6-158">Binary</span></span>|<span data-ttu-id="f6bc6-159">As informações do manifesto.</span><span class="sxs-lookup"><span data-stu-id="f6bc6-159">The manifest information.</span></span>|
|<span data-ttu-id="f6bc6-160">uploadState</span><span class="sxs-lookup"><span data-stu-id="f6bc6-160">uploadState</span></span>|[<span data-ttu-id="f6bc6-161">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="f6bc6-161">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="f6bc6-162">O estado da solicitação de carregamento atual.</span><span class="sxs-lookup"><span data-stu-id="f6bc6-162">The state of the current upload request.</span></span> <span data-ttu-id="f6bc6-163">Os valores possíveis são: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="f6bc6-163">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="f6bc6-164">isframeworkfile</span><span class="sxs-lookup"><span data-stu-id="f6bc6-164">isFrameworkFile</span></span>|<span data-ttu-id="f6bc6-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="f6bc6-165">Boolean</span></span>|<span data-ttu-id="f6bc6-166">Um valor que indica se o arquivo é um arquivo de estrutura.</span><span class="sxs-lookup"><span data-stu-id="f6bc6-166">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="f6bc6-167">IsDependency</span><span class="sxs-lookup"><span data-stu-id="f6bc6-167">isDependency</span></span>|<span data-ttu-id="f6bc6-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="f6bc6-168">Boolean</span></span>|<span data-ttu-id="f6bc6-169">Se o arquivo de conteúdo é uma dependência para o arquivo de conteúdo principal.</span><span class="sxs-lookup"><span data-stu-id="f6bc6-169">Whether the content file is a dependency for the main content file.</span></span>|



## <a name="response"></a><span data-ttu-id="f6bc6-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6bc6-170">Response</span></span>
<span data-ttu-id="f6bc6-171">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6bc6-171">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6bc6-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f6bc6-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6bc6-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6bc6-173">Request</span></span>
<span data-ttu-id="f6bc6-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6bc6-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f6bc6-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6bc6-175">Response</span></span>
<span data-ttu-id="f6bc6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f6bc6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




