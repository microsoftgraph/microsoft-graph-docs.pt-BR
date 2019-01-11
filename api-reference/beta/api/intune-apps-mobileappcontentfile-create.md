---
title: Criar mobileAppContentFile
description: Criar um novo objeto mobileAppContentFile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f6b8098a4311c723627d671980bfb006d4cab036
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883241"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="c13f9-103">Criar mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="c13f9-103">Create mobileAppContentFile</span></span>

> <span data-ttu-id="c13f9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c13f9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c13f9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c13f9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c13f9-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c13f9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c13f9-107">Criar um novo objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="c13f9-107">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c13f9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c13f9-108">Prerequisites</span></span>
<span data-ttu-id="c13f9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c13f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c13f9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c13f9-111">Permission type</span></span>|<span data-ttu-id="c13f9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c13f9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c13f9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c13f9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c13f9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c13f9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c13f9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c13f9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c13f9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c13f9-116">Not supported.</span></span>|
|<span data-ttu-id="c13f9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c13f9-117">Application</span></span>|<span data-ttu-id="c13f9-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c13f9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c13f9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c13f9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="c13f9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c13f9-120">Request headers</span></span>
|<span data-ttu-id="c13f9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c13f9-121">Header</span></span>|<span data-ttu-id="c13f9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c13f9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c13f9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c13f9-123">Authorization</span></span>|<span data-ttu-id="c13f9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c13f9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c13f9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c13f9-125">Accept</span></span>|<span data-ttu-id="c13f9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c13f9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c13f9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c13f9-127">Request body</span></span>
<span data-ttu-id="c13f9-128">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="c13f9-128">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="c13f9-129">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="c13f9-129">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="c13f9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c13f9-130">Property</span></span>|<span data-ttu-id="c13f9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c13f9-131">Type</span></span>|<span data-ttu-id="c13f9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c13f9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c13f9-133">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="c13f9-133">azureStorageUri</span></span>|<span data-ttu-id="c13f9-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c13f9-134">String</span></span>|<span data-ttu-id="c13f9-135">O URI de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="c13f9-135">The Azure Storage URI.</span></span>|
|<span data-ttu-id="c13f9-136">isCommitted</span><span class="sxs-lookup"><span data-stu-id="c13f9-136">isCommitted</span></span>|<span data-ttu-id="c13f9-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="c13f9-137">Boolean</span></span>|<span data-ttu-id="c13f9-138">Um valor que indica se o arquivo tem está confirmado.</span><span class="sxs-lookup"><span data-stu-id="c13f9-138">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="c13f9-139">id</span><span class="sxs-lookup"><span data-stu-id="c13f9-139">id</span></span>|<span data-ttu-id="c13f9-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c13f9-140">String</span></span>|<span data-ttu-id="c13f9-141">A ID do arquivo.</span><span class="sxs-lookup"><span data-stu-id="c13f9-141">The File Id.</span></span>|
|<span data-ttu-id="c13f9-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c13f9-142">createdDateTime</span></span>|<span data-ttu-id="c13f9-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c13f9-143">DateTimeOffset</span></span>|<span data-ttu-id="c13f9-144">A hora em que o arquivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="c13f9-144">The time the file was created.</span></span>|
|<span data-ttu-id="c13f9-145">name</span><span class="sxs-lookup"><span data-stu-id="c13f9-145">name</span></span>|<span data-ttu-id="c13f9-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c13f9-146">String</span></span>|<span data-ttu-id="c13f9-147">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="c13f9-147">the file name.</span></span>|
|<span data-ttu-id="c13f9-148">size</span><span class="sxs-lookup"><span data-stu-id="c13f9-148">size</span></span>|<span data-ttu-id="c13f9-149">Int64</span><span class="sxs-lookup"><span data-stu-id="c13f9-149">Int64</span></span>|<span data-ttu-id="c13f9-150">O tamanho do arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="c13f9-150">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="c13f9-151">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="c13f9-151">sizeEncrypted</span></span>|<span data-ttu-id="c13f9-152">Int64</span><span class="sxs-lookup"><span data-stu-id="c13f9-152">Int64</span></span>|<span data-ttu-id="c13f9-153">O tamanho do arquivo após a criptografia.</span><span class="sxs-lookup"><span data-stu-id="c13f9-153">The size of the file after encryption.</span></span>|
|<span data-ttu-id="c13f9-154">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c13f9-154">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="c13f9-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c13f9-155">DateTimeOffset</span></span>|<span data-ttu-id="c13f9-156">A hora de expiração do URI do armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="c13f9-156">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="c13f9-157">manifest</span><span class="sxs-lookup"><span data-stu-id="c13f9-157">manifest</span></span>|<span data-ttu-id="c13f9-158">Binária</span><span class="sxs-lookup"><span data-stu-id="c13f9-158">Binary</span></span>|<span data-ttu-id="c13f9-159">As informações do manifesto.</span><span class="sxs-lookup"><span data-stu-id="c13f9-159">The manifest information.</span></span>|
|<span data-ttu-id="c13f9-160">uploadState</span><span class="sxs-lookup"><span data-stu-id="c13f9-160">uploadState</span></span>|[<span data-ttu-id="c13f9-161">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="c13f9-161">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="c13f9-162">O estado da solicitação de carregamento atual.</span><span class="sxs-lookup"><span data-stu-id="c13f9-162">The state of the current upload request.</span></span> <span data-ttu-id="c13f9-163">Os valores possíveis são: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="c13f9-163">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="c13f9-164">isFrameworkFile</span><span class="sxs-lookup"><span data-stu-id="c13f9-164">isFrameworkFile</span></span>|<span data-ttu-id="c13f9-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="c13f9-165">Boolean</span></span>|<span data-ttu-id="c13f9-166">Um valor que indica se o arquivo é um arquivo framework.</span><span class="sxs-lookup"><span data-stu-id="c13f9-166">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="c13f9-167">isDependency</span><span class="sxs-lookup"><span data-stu-id="c13f9-167">isDependency</span></span>|<span data-ttu-id="c13f9-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="c13f9-168">Boolean</span></span>|<span data-ttu-id="c13f9-169">Se o arquivo de conteúdo é uma dependência para o arquivo de conteúdo principal.</span><span class="sxs-lookup"><span data-stu-id="c13f9-169">Whether the content file is a dependency for the main content file.</span></span>|



## <a name="response"></a><span data-ttu-id="c13f9-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="c13f9-170">Response</span></span>
<span data-ttu-id="c13f9-171">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c13f9-171">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c13f9-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c13f9-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="c13f9-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c13f9-173">Request</span></span>
<span data-ttu-id="c13f9-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c13f9-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c13f9-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="c13f9-175">Response</span></span>
<span data-ttu-id="c13f9-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c13f9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





