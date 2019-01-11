---
title: Função verifyWindowsEnrollmentAutoDiscovery
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 144fb484a9d372c2f3173b300274901c9fdc3dd1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823657"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="9fefd-103">Função verifyWindowsEnrollmentAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="9fefd-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="9fefd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9fefd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9fefd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9fefd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9fefd-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9fefd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9fefd-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9fefd-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9fefd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9fefd-108">Prerequisites</span></span>
<span data-ttu-id="9fefd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fefd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fefd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9fefd-111">Permission type</span></span>|<span data-ttu-id="9fefd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9fefd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fefd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9fefd-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9fefd-114">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="9fefd-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="9fefd-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fefd-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9fefd-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9fefd-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fefd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fefd-117">Not supported.</span></span>|
|<span data-ttu-id="9fefd-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9fefd-118">Application</span></span>|<span data-ttu-id="9fefd-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fefd-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fefd-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9fefd-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="9fefd-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9fefd-121">Request headers</span></span>
|<span data-ttu-id="9fefd-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9fefd-122">Header</span></span>|<span data-ttu-id="9fefd-123">Valor</span><span class="sxs-lookup"><span data-stu-id="9fefd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fefd-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9fefd-124">Authorization</span></span>|<span data-ttu-id="9fefd-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fefd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fefd-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9fefd-126">Accept</span></span>|<span data-ttu-id="9fefd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9fefd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fefd-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9fefd-128">Request body</span></span>
<span data-ttu-id="9fefd-129">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="9fefd-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="9fefd-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="9fefd-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="9fefd-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9fefd-131">Property</span></span>|<span data-ttu-id="9fefd-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fefd-132">Type</span></span>|<span data-ttu-id="9fefd-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fefd-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fefd-134">domainName</span><span class="sxs-lookup"><span data-stu-id="9fefd-134">domainName</span></span>|<span data-ttu-id="9fefd-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9fefd-135">String</span></span>|<span data-ttu-id="9fefd-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9fefd-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9fefd-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fefd-137">Response</span></span>
<span data-ttu-id="9fefd-138">Se tiver êxito, essa função retornará o código resposta `200 OK` e um Booliano no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9fefd-138">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fefd-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9fefd-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="9fefd-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9fefd-140">Request</span></span>
<span data-ttu-id="9fefd-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9fefd-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="9fefd-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fefd-142">Response</span></span>
<span data-ttu-id="9fefd-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9fefd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```



