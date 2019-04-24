---
title: Ação requestSignupUrl
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c4b7c0fd26994182aa7040f770f748d47994d6ce
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32498169"
---
# <a name="requestsignupurl-action"></a><span data-ttu-id="5a533-103">Ação requestSignupUrl</span><span class="sxs-lookup"><span data-stu-id="5a533-103">requestSignupUrl action</span></span>

> <span data-ttu-id="5a533-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5a533-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a533-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5a533-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a533-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5a533-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a533-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5a533-107">Prerequisites</span></span>
<span data-ttu-id="5a533-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a533-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a533-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a533-110">Permission type</span></span>|<span data-ttu-id="5a533-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5a533-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a533-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a533-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5a533-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a533-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5a533-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a533-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a533-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a533-115">Not supported.</span></span>|
|<span data-ttu-id="5a533-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a533-116">Application</span></span>|<span data-ttu-id="5a533-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a533-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a533-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a533-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/requestSignupUrl
```

## <a name="request-headers"></a><span data-ttu-id="5a533-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a533-119">Request headers</span></span>
|<span data-ttu-id="5a533-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5a533-120">Header</span></span>|<span data-ttu-id="5a533-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5a533-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a533-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a533-122">Authorization</span></span>|<span data-ttu-id="5a533-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a533-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a533-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5a533-124">Accept</span></span>|<span data-ttu-id="5a533-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5a533-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a533-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a533-126">Request body</span></span>
<span data-ttu-id="5a533-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="5a533-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5a533-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="5a533-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5a533-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a533-129">Property</span></span>|<span data-ttu-id="5a533-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a533-130">Type</span></span>|<span data-ttu-id="5a533-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a533-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a533-132">hostName</span><span class="sxs-lookup"><span data-stu-id="5a533-132">hostName</span></span>|<span data-ttu-id="5a533-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a533-133">String</span></span>|<span data-ttu-id="5a533-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5a533-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5a533-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a533-135">Response</span></span>
<span data-ttu-id="5a533-136">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a533-136">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a533-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a533-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a533-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a533-138">Request</span></span>
<span data-ttu-id="5a533-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a533-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/requestSignupUrl

Content-type: application/json
Content-length: 37

{
  "hostName": "Host Name value"
}
```

### <a name="response"></a><span data-ttu-id="5a533-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a533-140">Response</span></span>
<span data-ttu-id="5a533-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5a533-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 56

{
  "value": "https://example.com/requestSignupUrl/"
}
```





