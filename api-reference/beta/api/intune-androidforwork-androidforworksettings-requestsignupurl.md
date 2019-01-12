---
title: Ação requestSignupUrl
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 901d0bb67fa5992aa0931afc70660c22cd5ffeca
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980038"
---
# <a name="requestsignupurl-action"></a><span data-ttu-id="473c4-103">Ação requestSignupUrl</span><span class="sxs-lookup"><span data-stu-id="473c4-103">requestSignupUrl action</span></span>

> <span data-ttu-id="473c4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="473c4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="473c4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="473c4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="473c4-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="473c4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="473c4-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="473c4-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="473c4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="473c4-108">Prerequisites</span></span>
<span data-ttu-id="473c4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="473c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="473c4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="473c4-111">Permission type</span></span>|<span data-ttu-id="473c4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="473c4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="473c4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="473c4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="473c4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="473c4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="473c4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="473c4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="473c4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="473c4-116">Not supported.</span></span>|
|<span data-ttu-id="473c4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="473c4-117">Application</span></span>|<span data-ttu-id="473c4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="473c4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="473c4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="473c4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkSettings/requestSignupUrl
```

## <a name="request-headers"></a><span data-ttu-id="473c4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="473c4-120">Request headers</span></span>
|<span data-ttu-id="473c4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="473c4-121">Header</span></span>|<span data-ttu-id="473c4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="473c4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="473c4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="473c4-123">Authorization</span></span>|<span data-ttu-id="473c4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="473c4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="473c4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="473c4-125">Accept</span></span>|<span data-ttu-id="473c4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="473c4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="473c4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="473c4-127">Request body</span></span>
<span data-ttu-id="473c4-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="473c4-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="473c4-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="473c4-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="473c4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="473c4-130">Property</span></span>|<span data-ttu-id="473c4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="473c4-131">Type</span></span>|<span data-ttu-id="473c4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="473c4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="473c4-133">hostName</span><span class="sxs-lookup"><span data-stu-id="473c4-133">hostName</span></span>|<span data-ttu-id="473c4-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="473c4-134">String</span></span>|<span data-ttu-id="473c4-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="473c4-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="473c4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="473c4-136">Response</span></span>
<span data-ttu-id="473c4-137">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="473c4-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="473c4-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="473c4-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="473c4-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="473c4-139">Request</span></span>
<span data-ttu-id="473c4-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="473c4-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings/requestSignupUrl

Content-type: application/json
Content-length: 37

{
  "hostName": "Host Name value"
}
```

### <a name="response"></a><span data-ttu-id="473c4-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="473c4-141">Response</span></span>
<span data-ttu-id="473c4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="473c4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 56

{
  "value": "https://example.com/requestSignupUrl/"
}
```





