---
title: Ação requestSignupUrl
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fbd1ba5f70d94c75824d9585fa93b47960a78400
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446090"
---
# <a name="requestsignupurl-action"></a><span data-ttu-id="3fa72-103">Ação requestSignupUrl</span><span class="sxs-lookup"><span data-stu-id="3fa72-103">requestSignupUrl action</span></span>

<span data-ttu-id="3fa72-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3fa72-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3fa72-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3fa72-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3fa72-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3fa72-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fa72-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3fa72-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3fa72-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3fa72-108">Prerequisites</span></span>
<span data-ttu-id="3fa72-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fa72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fa72-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3fa72-111">Permission type</span></span>|<span data-ttu-id="3fa72-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3fa72-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fa72-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3fa72-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3fa72-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fa72-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3fa72-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3fa72-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fa72-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3fa72-116">Not supported.</span></span>|
|<span data-ttu-id="3fa72-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3fa72-117">Application</span></span>|<span data-ttu-id="3fa72-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fa72-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fa72-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3fa72-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/requestSignupUrl
```

## <a name="request-headers"></a><span data-ttu-id="3fa72-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3fa72-120">Request headers</span></span>
|<span data-ttu-id="3fa72-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3fa72-121">Header</span></span>|<span data-ttu-id="3fa72-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3fa72-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fa72-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3fa72-123">Authorization</span></span>|<span data-ttu-id="3fa72-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3fa72-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fa72-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3fa72-125">Accept</span></span>|<span data-ttu-id="3fa72-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3fa72-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fa72-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3fa72-127">Request body</span></span>
<span data-ttu-id="3fa72-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3fa72-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3fa72-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="3fa72-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3fa72-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3fa72-130">Property</span></span>|<span data-ttu-id="3fa72-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3fa72-131">Type</span></span>|<span data-ttu-id="3fa72-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fa72-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fa72-133">hostName</span><span class="sxs-lookup"><span data-stu-id="3fa72-133">hostName</span></span>|<span data-ttu-id="3fa72-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3fa72-134">String</span></span>|<span data-ttu-id="3fa72-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3fa72-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3fa72-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fa72-136">Response</span></span>
<span data-ttu-id="3fa72-137">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3fa72-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fa72-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3fa72-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fa72-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3fa72-139">Request</span></span>
<span data-ttu-id="3fa72-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3fa72-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/requestSignupUrl

Content-type: application/json
Content-length: 37

{
  "hostName": "Host Name value"
}
```

### <a name="response"></a><span data-ttu-id="3fa72-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fa72-141">Response</span></span>
<span data-ttu-id="3fa72-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3fa72-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 56

{
  "value": "https://example.com/requestSignupUrl/"
}
```





