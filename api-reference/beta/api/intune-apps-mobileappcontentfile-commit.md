---
title: ação de confirmação
description: Confirma um arquivo de um determinado aplicativo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2d144108bd28c6428e35d985783fd1730e374e8f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939893"
---
# <a name="commit-action"></a><span data-ttu-id="475a3-103">ação de confirmação</span><span class="sxs-lookup"><span data-stu-id="475a3-103">commit action</span></span>

> <span data-ttu-id="475a3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="475a3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="475a3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="475a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="475a3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="475a3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="475a3-107">Confirma um arquivo de um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="475a3-107">Commits a file of a given app.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="475a3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="475a3-108">Prerequisites</span></span>
<span data-ttu-id="475a3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="475a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="475a3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="475a3-111">Permission type</span></span>|<span data-ttu-id="475a3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="475a3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="475a3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="475a3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="475a3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="475a3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="475a3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="475a3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="475a3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="475a3-116">Not supported.</span></span>|
|<span data-ttu-id="475a3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="475a3-117">Application</span></span>|<span data-ttu-id="475a3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="475a3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="475a3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="475a3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit
```

## <a name="request-headers"></a><span data-ttu-id="475a3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="475a3-120">Request headers</span></span>
|<span data-ttu-id="475a3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="475a3-121">Header</span></span>|<span data-ttu-id="475a3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="475a3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="475a3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="475a3-123">Authorization</span></span>|<span data-ttu-id="475a3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="475a3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="475a3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="475a3-125">Accept</span></span>|<span data-ttu-id="475a3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="475a3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="475a3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="475a3-127">Request body</span></span>
<span data-ttu-id="475a3-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="475a3-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="475a3-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="475a3-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="475a3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="475a3-130">Property</span></span>|<span data-ttu-id="475a3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="475a3-131">Type</span></span>|<span data-ttu-id="475a3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="475a3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="475a3-133">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="475a3-133">fileEncryptionInfo</span></span>|[<span data-ttu-id="475a3-134">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="475a3-134">fileEncryptionInfo</span></span>](../resources/intune-apps-fileencryptioninfo.md)|<span data-ttu-id="475a3-135">Chave de parâmetro das informações sobre criptografia de arquivo.</span><span class="sxs-lookup"><span data-stu-id="475a3-135">File encryption info parameter key.</span></span>|



## <a name="response"></a><span data-ttu-id="475a3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="475a3-136">Response</span></span>
<span data-ttu-id="475a3-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="475a3-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="475a3-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="475a3-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="475a3-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="475a3-139">Request</span></span>
<span data-ttu-id="475a3-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="475a3-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="475a3-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="475a3-141">Response</span></span>
<span data-ttu-id="475a3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="475a3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





