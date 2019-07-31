---
title: ação de confirmação
description: Confirma um arquivo de um determinado aplicativo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 55ace6d773ee441542e5569c83b5b3b57ce8b289
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35960871"
---
# <a name="commit-action"></a><span data-ttu-id="080ee-103">Ação de confirmação</span><span class="sxs-lookup"><span data-stu-id="080ee-103">commit action</span></span>

> <span data-ttu-id="080ee-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="080ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="080ee-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="080ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="080ee-106">Confirma um arquivo de um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="080ee-106">Commits a file of a given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="080ee-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="080ee-107">Prerequisites</span></span>
<span data-ttu-id="080ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="080ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="080ee-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="080ee-110">Permission type</span></span>|<span data-ttu-id="080ee-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="080ee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="080ee-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="080ee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="080ee-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="080ee-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="080ee-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="080ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="080ee-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="080ee-115">Not supported.</span></span>|
|<span data-ttu-id="080ee-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="080ee-116">Application</span></span>|<span data-ttu-id="080ee-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="080ee-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="080ee-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="080ee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit
```

## <a name="request-headers"></a><span data-ttu-id="080ee-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="080ee-119">Request headers</span></span>
|<span data-ttu-id="080ee-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="080ee-120">Header</span></span>|<span data-ttu-id="080ee-121">Valor</span><span class="sxs-lookup"><span data-stu-id="080ee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="080ee-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="080ee-122">Authorization</span></span>|<span data-ttu-id="080ee-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="080ee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="080ee-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="080ee-124">Accept</span></span>|<span data-ttu-id="080ee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="080ee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="080ee-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="080ee-126">Request body</span></span>
<span data-ttu-id="080ee-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="080ee-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="080ee-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="080ee-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="080ee-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="080ee-129">Property</span></span>|<span data-ttu-id="080ee-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="080ee-130">Type</span></span>|<span data-ttu-id="080ee-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="080ee-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="080ee-132">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="080ee-132">fileEncryptionInfo</span></span>|[<span data-ttu-id="080ee-133">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="080ee-133">fileEncryptionInfo</span></span>](../resources/intune-apps-fileencryptioninfo.md)|<span data-ttu-id="080ee-134">Chave de parâmetro das informações sobre criptografia de arquivo.</span><span class="sxs-lookup"><span data-stu-id="080ee-134">File encryption info parameter key.</span></span>|



## <a name="response"></a><span data-ttu-id="080ee-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="080ee-135">Response</span></span>
<span data-ttu-id="080ee-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="080ee-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="080ee-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="080ee-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="080ee-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="080ee-138">Request</span></span>
<span data-ttu-id="080ee-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="080ee-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="080ee-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="080ee-140">Response</span></span>
<span data-ttu-id="080ee-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="080ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





