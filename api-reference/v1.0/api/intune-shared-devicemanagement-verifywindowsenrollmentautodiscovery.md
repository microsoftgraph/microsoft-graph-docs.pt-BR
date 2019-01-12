---
title: Função verifyWindowsEnrollmentAutoDiscovery
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6090b0a050a493e26a5536f9f04f7c1e448cca98
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918067"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="f6268-103">Função verifyWindowsEnrollmentAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="f6268-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="f6268-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f6268-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f6268-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f6268-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f6268-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f6268-106">Prerequisites</span></span>
<span data-ttu-id="f6268-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6268-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6268-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6268-109">Permission type</span></span>|<span data-ttu-id="f6268-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f6268-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6268-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6268-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f6268-112">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="f6268-112">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="f6268-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6268-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f6268-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6268-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6268-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6268-115">Not supported.</span></span>|
|<span data-ttu-id="f6268-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6268-116">Application</span></span>|<span data-ttu-id="f6268-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6268-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6268-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6268-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="f6268-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6268-119">Request headers</span></span>
|<span data-ttu-id="f6268-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f6268-120">Header</span></span>|<span data-ttu-id="f6268-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f6268-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6268-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6268-122">Authorization</span></span>|<span data-ttu-id="f6268-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6268-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6268-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f6268-124">Accept</span></span>|<span data-ttu-id="f6268-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f6268-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6268-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6268-126">Request body</span></span>
<span data-ttu-id="f6268-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="f6268-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="f6268-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="f6268-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="f6268-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f6268-129">Property</span></span>|<span data-ttu-id="f6268-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6268-130">Type</span></span>|<span data-ttu-id="f6268-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6268-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6268-132">domainName</span><span class="sxs-lookup"><span data-stu-id="f6268-132">domainName</span></span>|<span data-ttu-id="f6268-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6268-133">String</span></span>|<span data-ttu-id="f6268-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f6268-134">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="f6268-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6268-135">Response</span></span>
<span data-ttu-id="f6268-136">Se tiver êxito, essa função retornará o código resposta `200 OK` e um Booliano no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6268-136">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6268-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f6268-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="f6268-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6268-138">Request</span></span>
<span data-ttu-id="f6268-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6268-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="f6268-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6268-140">Response</span></span>
<span data-ttu-id="f6268-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f6268-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```



