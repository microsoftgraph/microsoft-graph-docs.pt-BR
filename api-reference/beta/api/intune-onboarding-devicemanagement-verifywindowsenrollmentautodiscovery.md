---
title: Função verifyWindowsEnrollmentAutoDiscovery
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cb14317a132d4368a354d8655df56452100bf5a0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894296"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="d116a-103">Função verifyWindowsEnrollmentAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="d116a-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="d116a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d116a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d116a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d116a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d116a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d116a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d116a-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d116a-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d116a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d116a-108">Prerequisites</span></span>
<span data-ttu-id="d116a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d116a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d116a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d116a-111">Permission type</span></span>|<span data-ttu-id="d116a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d116a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d116a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d116a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d116a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d116a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d116a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d116a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d116a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d116a-116">Not supported.</span></span>|
|<span data-ttu-id="d116a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d116a-117">Application</span></span>|<span data-ttu-id="d116a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d116a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d116a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d116a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="d116a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d116a-120">Request headers</span></span>
|<span data-ttu-id="d116a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d116a-121">Header</span></span>|<span data-ttu-id="d116a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d116a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d116a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d116a-123">Authorization</span></span>|<span data-ttu-id="d116a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d116a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d116a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d116a-125">Accept</span></span>|<span data-ttu-id="d116a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d116a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d116a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d116a-127">Request body</span></span>
<span data-ttu-id="d116a-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="d116a-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="d116a-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="d116a-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="d116a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d116a-130">Property</span></span>|<span data-ttu-id="d116a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d116a-131">Type</span></span>|<span data-ttu-id="d116a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d116a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d116a-133">domainName</span><span class="sxs-lookup"><span data-stu-id="d116a-133">domainName</span></span>|<span data-ttu-id="d116a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d116a-134">String</span></span>|<span data-ttu-id="d116a-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d116a-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d116a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d116a-136">Response</span></span>
<span data-ttu-id="d116a-137">Se tiver êxito, essa função retornará o código resposta `200 OK` e um Booliano no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d116a-137">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d116a-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d116a-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="d116a-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d116a-139">Request</span></span>
<span data-ttu-id="d116a-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d116a-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="d116a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d116a-141">Response</span></span>
<span data-ttu-id="d116a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d116a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```





