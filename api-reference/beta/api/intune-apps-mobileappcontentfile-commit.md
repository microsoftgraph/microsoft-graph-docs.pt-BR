---
title: ação de confirmação
description: Confirma um arquivo de um determinado aplicativo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6ad6ab6adf673bda2d2f0472e298544bf782df54
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39935516"
---
# <a name="commit-action"></a><span data-ttu-id="489a8-103">Ação de confirmação</span><span class="sxs-lookup"><span data-stu-id="489a8-103">commit action</span></span>

> <span data-ttu-id="489a8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="489a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="489a8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="489a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="489a8-106">Confirma um arquivo de um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="489a8-106">Commits a file of a given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="489a8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="489a8-107">Prerequisites</span></span>
<span data-ttu-id="489a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="489a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="489a8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="489a8-110">Permission type</span></span>|<span data-ttu-id="489a8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="489a8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="489a8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="489a8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="489a8-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="489a8-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="489a8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="489a8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="489a8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="489a8-115">Not supported.</span></span>|
|<span data-ttu-id="489a8-116">Application</span><span class="sxs-lookup"><span data-stu-id="489a8-116">Application</span></span>|<span data-ttu-id="489a8-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="489a8-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="489a8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="489a8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit
```

## <a name="request-headers"></a><span data-ttu-id="489a8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="489a8-119">Request headers</span></span>
|<span data-ttu-id="489a8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="489a8-120">Header</span></span>|<span data-ttu-id="489a8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="489a8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="489a8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="489a8-122">Authorization</span></span>|<span data-ttu-id="489a8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="489a8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="489a8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="489a8-124">Accept</span></span>|<span data-ttu-id="489a8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="489a8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="489a8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="489a8-126">Request body</span></span>
<span data-ttu-id="489a8-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="489a8-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="489a8-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="489a8-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="489a8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="489a8-129">Property</span></span>|<span data-ttu-id="489a8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="489a8-130">Type</span></span>|<span data-ttu-id="489a8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="489a8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="489a8-132">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="489a8-132">fileEncryptionInfo</span></span>|[<span data-ttu-id="489a8-133">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="489a8-133">fileEncryptionInfo</span></span>](../resources/intune-apps-fileencryptioninfo.md)|<span data-ttu-id="489a8-134">Chave de parâmetro das informações sobre criptografia de arquivo.</span><span class="sxs-lookup"><span data-stu-id="489a8-134">File encryption info parameter key.</span></span>|



## <a name="response"></a><span data-ttu-id="489a8-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="489a8-135">Response</span></span>
<span data-ttu-id="489a8-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="489a8-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="489a8-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="489a8-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="489a8-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="489a8-138">Request</span></span>
<span data-ttu-id="489a8-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="489a8-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit

Content-type: application/json
Content-length: 399

{
  "fileEncryptionInfo": {
    "@odata.type": "microsoft.graph.fileEncryptionInfo",
    "encryptionKey": "ZW5jcnlwdGlvbktleQ==",
    "initializationVector": "aW5pdGlhbGl6YXRpb25WZWN0b3I=",
    "mac": "bWFj",
    "macKey": "bWFjS2V5",
    "profileIdentifier": "Profile Identifier value",
    "fileDigest": "ZmlsZURpZ2VzdA==",
    "fileDigestAlgorithm": "File Digest Algorithm value"
  }
}
```

### <a name="response"></a><span data-ttu-id="489a8-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="489a8-140">Response</span></span>
<span data-ttu-id="489a8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="489a8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





