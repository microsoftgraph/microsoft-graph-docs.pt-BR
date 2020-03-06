---
title: Função verifyWindowsEnrollmentAutoDiscovery
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ff32b1c5c8cc06835ca6d23697fd20bea83ba20c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512052"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="9a555-103">Função verifyWindowsEnrollmentAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="9a555-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

<span data-ttu-id="9a555-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a555-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a555-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9a555-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a555-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9a555-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a555-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9a555-107">Prerequisites</span></span>
<span data-ttu-id="9a555-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a555-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a555-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a555-110">Permission type</span></span>|<span data-ttu-id="9a555-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9a555-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a555-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a555-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9a555-113">&nbsp;&nbsp; Integração</span><span class="sxs-lookup"><span data-stu-id="9a555-113">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="9a555-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a555-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9a555-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a555-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a555-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a555-116">Not supported.</span></span>|
|<span data-ttu-id="9a555-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a555-117">Application</span></span>|<span data-ttu-id="9a555-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a555-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a555-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a555-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="9a555-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a555-120">Request headers</span></span>
|<span data-ttu-id="9a555-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9a555-121">Header</span></span>|<span data-ttu-id="9a555-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9a555-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a555-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a555-123">Authorization</span></span>|<span data-ttu-id="9a555-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a555-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a555-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9a555-125">Accept</span></span>|<span data-ttu-id="9a555-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a555-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a555-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a555-127">Request body</span></span>
<span data-ttu-id="9a555-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="9a555-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="9a555-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="9a555-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="9a555-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a555-130">Property</span></span>|<span data-ttu-id="9a555-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a555-131">Type</span></span>|<span data-ttu-id="9a555-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a555-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a555-133">domainName</span><span class="sxs-lookup"><span data-stu-id="9a555-133">domainName</span></span>|<span data-ttu-id="9a555-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a555-134">String</span></span>|<span data-ttu-id="9a555-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9a555-135">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="9a555-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a555-136">Response</span></span>
<span data-ttu-id="9a555-137">Se tiver êxito, essa função retornará o código resposta `200 OK` e um Booliano no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a555-137">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a555-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a555-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="9a555-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a555-139">Request</span></span>
<span data-ttu-id="9a555-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a555-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="9a555-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a555-141">Response</span></span>
<span data-ttu-id="9a555-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a555-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```




