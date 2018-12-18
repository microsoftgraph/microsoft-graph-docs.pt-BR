---
title: Atualizar mobileAppContentFile
description: Atualiza as propriedades de um objeto mobileAppContentFile.
author: tfitzmac
ms.openlocfilehash: 7117fe10ca2f191607c6d5a4823cc39a9fcc8cb9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309601"
---
# <a name="update-mobileappcontentfile"></a><span data-ttu-id="2462c-103">Atualizar mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="2462c-103">Update mobileAppContentFile</span></span>

> <span data-ttu-id="2462c-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2462c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2462c-105">Atualiza as propriedades de um objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="2462c-105">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2462c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2462c-106">Prerequisites</span></span>
<span data-ttu-id="2462c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2462c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2462c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2462c-109">Permission type</span></span>|<span data-ttu-id="2462c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2462c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2462c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2462c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2462c-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2462c-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2462c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2462c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2462c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2462c-114">Not supported.</span></span>|
|<span data-ttu-id="2462c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2462c-115">Application</span></span>|<span data-ttu-id="2462c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2462c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2462c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2462c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="2462c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2462c-118">Request headers</span></span>
|<span data-ttu-id="2462c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2462c-119">Header</span></span>|<span data-ttu-id="2462c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="2462c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2462c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2462c-121">Authorization</span></span>|<span data-ttu-id="2462c-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2462c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2462c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2462c-123">Accept</span></span>|<span data-ttu-id="2462c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2462c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2462c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2462c-125">Request body</span></span>
<span data-ttu-id="2462c-126">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="2462c-126">In the request body, supply a JSON representation for the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

<span data-ttu-id="2462c-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="2462c-127">The following table shows the properties that are required when you create the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>

|<span data-ttu-id="2462c-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2462c-128">Property</span></span>|<span data-ttu-id="2462c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="2462c-129">Type</span></span>|<span data-ttu-id="2462c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="2462c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2462c-131">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="2462c-131">azureStorageUri</span></span>|<span data-ttu-id="2462c-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2462c-132">String</span></span>|<span data-ttu-id="2462c-133">O URI de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="2462c-133">The Azure Storage URI.</span></span>|
|<span data-ttu-id="2462c-134">isCommitted</span><span class="sxs-lookup"><span data-stu-id="2462c-134">isCommitted</span></span>|<span data-ttu-id="2462c-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="2462c-135">Boolean</span></span>|<span data-ttu-id="2462c-136">Um valor que indica se o arquivo tem está confirmado.</span><span class="sxs-lookup"><span data-stu-id="2462c-136">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="2462c-137">id</span><span class="sxs-lookup"><span data-stu-id="2462c-137">id</span></span>|<span data-ttu-id="2462c-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2462c-138">String</span></span>|<span data-ttu-id="2462c-139">A ID do arquivo.</span><span class="sxs-lookup"><span data-stu-id="2462c-139">The File Id.</span></span>|
|<span data-ttu-id="2462c-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2462c-140">createdDateTime</span></span>|<span data-ttu-id="2462c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2462c-141">DateTimeOffset</span></span>|<span data-ttu-id="2462c-142">A hora em que o arquivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="2462c-142">The time the file was created.</span></span>|
|<span data-ttu-id="2462c-143">name</span><span class="sxs-lookup"><span data-stu-id="2462c-143">name</span></span>|<span data-ttu-id="2462c-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2462c-144">String</span></span>|<span data-ttu-id="2462c-145">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="2462c-145">the file name.</span></span>|
|<span data-ttu-id="2462c-146">size</span><span class="sxs-lookup"><span data-stu-id="2462c-146">size</span></span>|<span data-ttu-id="2462c-147">Int64</span><span class="sxs-lookup"><span data-stu-id="2462c-147">Int64</span></span>|<span data-ttu-id="2462c-148">O tamanho do arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="2462c-148">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="2462c-149">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="2462c-149">sizeEncrypted</span></span>|<span data-ttu-id="2462c-150">Int64</span><span class="sxs-lookup"><span data-stu-id="2462c-150">Int64</span></span>|<span data-ttu-id="2462c-151">O tamanho do arquivo após a criptografia.</span><span class="sxs-lookup"><span data-stu-id="2462c-151">The size of the file after encryption.</span></span>|
|<span data-ttu-id="2462c-152">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2462c-152">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="2462c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2462c-153">DateTimeOffset</span></span>|<span data-ttu-id="2462c-154">A hora de expiração do URI do armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="2462c-154">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="2462c-155">manifest</span><span class="sxs-lookup"><span data-stu-id="2462c-155">manifest</span></span>|<span data-ttu-id="2462c-156">Binária</span><span class="sxs-lookup"><span data-stu-id="2462c-156">Binary</span></span>|<span data-ttu-id="2462c-157">As informações do manifesto.</span><span class="sxs-lookup"><span data-stu-id="2462c-157">The manifest information.</span></span>|
|<span data-ttu-id="2462c-158">uploadState</span><span class="sxs-lookup"><span data-stu-id="2462c-158">uploadState</span></span>|[<span data-ttu-id="2462c-159">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="2462c-159">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="2462c-160">O estado da solicitação de carregamento atual.</span><span class="sxs-lookup"><span data-stu-id="2462c-160">The state of the current upload request.</span></span> <span data-ttu-id="2462c-161">Os valores possíveis são: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="2462c-161">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="2462c-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="2462c-162">Response</span></span>
<span data-ttu-id="2462c-163">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2462c-163">If successful, this method returns a `200 OK` response code and an updated [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2462c-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2462c-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="2462c-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2462c-165">Request</span></span>
<span data-ttu-id="2462c-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2462c-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2462c-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="2462c-167">Response</span></span>
<span data-ttu-id="2462c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2462c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



