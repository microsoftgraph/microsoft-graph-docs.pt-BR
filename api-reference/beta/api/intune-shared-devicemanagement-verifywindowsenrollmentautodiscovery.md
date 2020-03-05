---
title: Função verifyWindowsEnrollmentAutoDiscovery
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9713724c48c97d3ce62d7396275110d085cdc8a0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458536"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="67a75-103">Função verifyWindowsEnrollmentAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="67a75-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

<span data-ttu-id="67a75-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="67a75-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67a75-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="67a75-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="67a75-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="67a75-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67a75-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67a75-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67a75-108">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="67a75-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="67a75-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="67a75-109">Prerequisites</span></span>
<span data-ttu-id="67a75-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67a75-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67a75-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67a75-112">Permission type</span></span>|<span data-ttu-id="67a75-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="67a75-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67a75-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67a75-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="67a75-115">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="67a75-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="67a75-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67a75-116">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="67a75-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67a75-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67a75-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67a75-118">Not supported.</span></span>|
|<span data-ttu-id="67a75-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67a75-119">Application</span></span>||
| <span data-ttu-id="67a75-120">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="67a75-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="67a75-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67a75-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="67a75-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67a75-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="67a75-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67a75-123">Request headers</span></span>
|<span data-ttu-id="67a75-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67a75-124">Header</span></span>|<span data-ttu-id="67a75-125">Valor</span><span class="sxs-lookup"><span data-stu-id="67a75-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67a75-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="67a75-126">Authorization</span></span>|<span data-ttu-id="67a75-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67a75-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67a75-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="67a75-128">Accept</span></span>|<span data-ttu-id="67a75-129">application/json</span><span class="sxs-lookup"><span data-stu-id="67a75-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67a75-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67a75-130">Request body</span></span>
<span data-ttu-id="67a75-131">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="67a75-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="67a75-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="67a75-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="67a75-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67a75-133">Property</span></span>|<span data-ttu-id="67a75-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="67a75-134">Type</span></span>|<span data-ttu-id="67a75-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="67a75-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67a75-136">domainName</span><span class="sxs-lookup"><span data-stu-id="67a75-136">domainName</span></span>|<span data-ttu-id="67a75-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67a75-137">String</span></span>|<span data-ttu-id="67a75-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="67a75-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="67a75-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="67a75-139">Response</span></span>
<span data-ttu-id="67a75-140">Se tiver êxito, essa função retornará o código resposta `200 OK` e um Booliano no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67a75-140">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67a75-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67a75-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="67a75-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67a75-142">Request</span></span>
<span data-ttu-id="67a75-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67a75-143">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="67a75-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="67a75-144">Response</span></span>
<span data-ttu-id="67a75-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67a75-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```











