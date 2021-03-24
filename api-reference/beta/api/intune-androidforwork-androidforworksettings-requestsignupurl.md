---
title: Ação requestSignupUrl
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9d9a090c5150cc5c90023671f36e0c75acae6977
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141243"
---
# <a name="requestsignupurl-action"></a><span data-ttu-id="f0175-103">Ação requestSignupUrl</span><span class="sxs-lookup"><span data-stu-id="f0175-103">requestSignupUrl action</span></span>

<span data-ttu-id="f0175-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0175-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0175-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f0175-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0175-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f0175-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0175-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f0175-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0175-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f0175-108">Prerequisites</span></span>
<span data-ttu-id="f0175-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0175-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0175-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0175-111">Permission type</span></span>|<span data-ttu-id="f0175-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f0175-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0175-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0175-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0175-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0175-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f0175-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0175-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0175-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0175-116">Not supported.</span></span>|
|<span data-ttu-id="f0175-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0175-117">Application</span></span>|<span data-ttu-id="f0175-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0175-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0175-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0175-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkSettings/requestSignupUrl
```

## <a name="request-headers"></a><span data-ttu-id="f0175-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0175-120">Request headers</span></span>
|<span data-ttu-id="f0175-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f0175-121">Header</span></span>|<span data-ttu-id="f0175-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f0175-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0175-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0175-123">Authorization</span></span>|<span data-ttu-id="f0175-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0175-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0175-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f0175-125">Accept</span></span>|<span data-ttu-id="f0175-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0175-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0175-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0175-127">Request body</span></span>
<span data-ttu-id="f0175-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f0175-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f0175-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="f0175-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f0175-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0175-130">Property</span></span>|<span data-ttu-id="f0175-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0175-131">Type</span></span>|<span data-ttu-id="f0175-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0175-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0175-133">hostName</span><span class="sxs-lookup"><span data-stu-id="f0175-133">hostName</span></span>|<span data-ttu-id="f0175-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0175-134">String</span></span>|<span data-ttu-id="f0175-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f0175-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f0175-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0175-136">Response</span></span>
<span data-ttu-id="f0175-137">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0175-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0175-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0175-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0175-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0175-139">Request</span></span>
<span data-ttu-id="f0175-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0175-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings/requestSignupUrl

Content-type: application/json
Content-length: 37

{
  "hostName": "Host Name value"
}
```

### <a name="response"></a><span data-ttu-id="f0175-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0175-141">Response</span></span>
<span data-ttu-id="f0175-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f0175-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 56

{
  "value": "https://example.com/requestSignupUrl/"
}
```




