---
title: ação de confirmação
description: Confirma um arquivo de um determinado aplicativo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d5dbe643d1bcdd0dc40e95d1a00c5e61d1d4fa71
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515950"
---
# <a name="commit-action"></a><span data-ttu-id="fd85e-103">Ação de confirmação</span><span class="sxs-lookup"><span data-stu-id="fd85e-103">commit action</span></span>

<span data-ttu-id="fd85e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd85e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fd85e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fd85e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd85e-106">Confirma um arquivo de um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fd85e-106">Commits a file of a given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd85e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fd85e-107">Prerequisites</span></span>
<span data-ttu-id="fd85e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd85e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd85e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd85e-110">Permission type</span></span>|<span data-ttu-id="fd85e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fd85e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd85e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd85e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fd85e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd85e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fd85e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd85e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd85e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd85e-115">Not supported.</span></span>|
|<span data-ttu-id="fd85e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd85e-116">Application</span></span>|<span data-ttu-id="fd85e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd85e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd85e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd85e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit
```

## <a name="request-headers"></a><span data-ttu-id="fd85e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd85e-119">Request headers</span></span>
|<span data-ttu-id="fd85e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fd85e-120">Header</span></span>|<span data-ttu-id="fd85e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fd85e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd85e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd85e-122">Authorization</span></span>|<span data-ttu-id="fd85e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd85e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd85e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fd85e-124">Accept</span></span>|<span data-ttu-id="fd85e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fd85e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd85e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd85e-126">Request body</span></span>
<span data-ttu-id="fd85e-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="fd85e-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fd85e-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="fd85e-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fd85e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd85e-129">Property</span></span>|<span data-ttu-id="fd85e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd85e-130">Type</span></span>|<span data-ttu-id="fd85e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd85e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd85e-132">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="fd85e-132">fileEncryptionInfo</span></span>|[<span data-ttu-id="fd85e-133">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="fd85e-133">fileEncryptionInfo</span></span>](../resources/intune-apps-fileencryptioninfo.md)|<span data-ttu-id="fd85e-134">Chave de parâmetro das informações sobre criptografia de arquivo.</span><span class="sxs-lookup"><span data-stu-id="fd85e-134">File encryption info parameter key.</span></span>|



## <a name="response"></a><span data-ttu-id="fd85e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd85e-135">Response</span></span>
<span data-ttu-id="fd85e-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fd85e-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fd85e-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd85e-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd85e-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd85e-138">Request</span></span>
<span data-ttu-id="fd85e-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd85e-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fd85e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd85e-140">Response</span></span>
<span data-ttu-id="fd85e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fd85e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




