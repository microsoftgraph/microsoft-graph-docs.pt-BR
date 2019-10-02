---
title: Função verifyWindowsEnrollmentAutoDiscovery
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8c2c81257dcc27791cd7db8883b60feeb3544c79
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361431"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="1f655-103">Função verifyWindowsEnrollmentAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="1f655-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="1f655-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1f655-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f655-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1f655-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f655-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1f655-106">Prerequisites</span></span>
<span data-ttu-id="1f655-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f655-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f655-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f655-109">Permission type</span></span>|<span data-ttu-id="1f655-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1f655-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f655-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f655-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1f655-112">&nbsp;&nbsp; Integração</span><span class="sxs-lookup"><span data-stu-id="1f655-112">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="1f655-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f655-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1f655-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f655-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f655-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f655-115">Not supported.</span></span>|
|<span data-ttu-id="1f655-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f655-116">Application</span></span>|<span data-ttu-id="1f655-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f655-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f655-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f655-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="1f655-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f655-119">Request headers</span></span>
|<span data-ttu-id="1f655-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1f655-120">Header</span></span>|<span data-ttu-id="1f655-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1f655-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f655-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f655-122">Authorization</span></span>|<span data-ttu-id="1f655-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f655-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f655-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1f655-124">Accept</span></span>|<span data-ttu-id="1f655-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1f655-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f655-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f655-126">Request body</span></span>
<span data-ttu-id="1f655-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="1f655-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="1f655-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="1f655-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="1f655-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f655-129">Property</span></span>|<span data-ttu-id="1f655-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f655-130">Type</span></span>|<span data-ttu-id="1f655-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f655-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f655-132">domainName</span><span class="sxs-lookup"><span data-stu-id="1f655-132">domainName</span></span>|<span data-ttu-id="1f655-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f655-133">String</span></span>|<span data-ttu-id="1f655-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1f655-134">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="1f655-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f655-135">Response</span></span>
<span data-ttu-id="1f655-136">Se tiver êxito, essa função retornará o código resposta `200 OK` e um Booliano no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f655-136">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f655-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f655-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="1f655-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f655-138">Request</span></span>
<span data-ttu-id="1f655-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f655-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="1f655-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f655-140">Response</span></span>
<span data-ttu-id="1f655-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1f655-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```




