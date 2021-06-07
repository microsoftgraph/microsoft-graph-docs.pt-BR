---
title: ação de confirmação
description: Confirma um arquivo de um determinado aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fc2f4a3db1b53958a5055a302f9e4db57e19e91e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754067"
---
# <a name="commit-action"></a><span data-ttu-id="a10be-103">Ação de confirmação</span><span class="sxs-lookup"><span data-stu-id="a10be-103">commit action</span></span>

<span data-ttu-id="a10be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a10be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a10be-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a10be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a10be-106">Confirma um arquivo de um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a10be-106">Commits a file of a given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a10be-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a10be-107">Prerequisites</span></span>
<span data-ttu-id="a10be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a10be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a10be-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a10be-110">Permission type</span></span>|<span data-ttu-id="a10be-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a10be-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a10be-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a10be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a10be-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a10be-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a10be-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a10be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a10be-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a10be-115">Not supported.</span></span>|
|<span data-ttu-id="a10be-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a10be-116">Application</span></span>|<span data-ttu-id="a10be-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a10be-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a10be-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a10be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit
```

## <a name="request-headers"></a><span data-ttu-id="a10be-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a10be-119">Request headers</span></span>
|<span data-ttu-id="a10be-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a10be-120">Header</span></span>|<span data-ttu-id="a10be-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a10be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a10be-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a10be-122">Authorization</span></span>|<span data-ttu-id="a10be-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a10be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a10be-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a10be-124">Accept</span></span>|<span data-ttu-id="a10be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a10be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a10be-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a10be-126">Request body</span></span>
<span data-ttu-id="a10be-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="a10be-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a10be-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="a10be-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a10be-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a10be-129">Property</span></span>|<span data-ttu-id="a10be-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a10be-130">Type</span></span>|<span data-ttu-id="a10be-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a10be-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a10be-132">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="a10be-132">fileEncryptionInfo</span></span>|[<span data-ttu-id="a10be-133">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="a10be-133">fileEncryptionInfo</span></span>](../resources/intune-apps-fileencryptioninfo.md)|<span data-ttu-id="a10be-134">Chave de parâmetro das informações sobre criptografia de arquivo.</span><span class="sxs-lookup"><span data-stu-id="a10be-134">File encryption info parameter key.</span></span>|



## <a name="response"></a><span data-ttu-id="a10be-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a10be-135">Response</span></span>
<span data-ttu-id="a10be-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a10be-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a10be-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a10be-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="a10be-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a10be-138">Request</span></span>
<span data-ttu-id="a10be-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a10be-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit

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

### <a name="response"></a><span data-ttu-id="a10be-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a10be-140">Response</span></span>
<span data-ttu-id="a10be-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a10be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




