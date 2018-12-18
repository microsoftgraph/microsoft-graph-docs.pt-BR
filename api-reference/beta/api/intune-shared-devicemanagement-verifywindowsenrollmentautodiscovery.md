---
title: Função verifyWindowsEnrollmentAutoDiscovery
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: 31dd340b996747a0de358c795bac098abfd3ba59
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317903"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="a5aa0-103">Função verifyWindowsEnrollmentAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="a5aa0-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="a5aa0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a5aa0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5aa0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a5aa0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5aa0-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a5aa0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5aa0-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a5aa0-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a5aa0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a5aa0-108">Prerequisites</span></span>
<span data-ttu-id="a5aa0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5aa0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5aa0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5aa0-111">Permission type</span></span>|<span data-ttu-id="a5aa0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a5aa0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5aa0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5aa0-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a5aa0-114">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="a5aa0-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="a5aa0-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5aa0-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a5aa0-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5aa0-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5aa0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5aa0-117">Not supported.</span></span>|
|<span data-ttu-id="a5aa0-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5aa0-118">Application</span></span>|<span data-ttu-id="a5aa0-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5aa0-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5aa0-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5aa0-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="a5aa0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5aa0-121">Request headers</span></span>
|<span data-ttu-id="a5aa0-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a5aa0-122">Header</span></span>|<span data-ttu-id="a5aa0-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a5aa0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5aa0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5aa0-124">Authorization</span></span>|<span data-ttu-id="a5aa0-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5aa0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5aa0-126">Accept</span><span class="sxs-lookup"><span data-stu-id="a5aa0-126">Accept</span></span>|<span data-ttu-id="a5aa0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a5aa0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5aa0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5aa0-128">Request body</span></span>
<span data-ttu-id="a5aa0-129">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="a5aa0-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="a5aa0-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="a5aa0-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="a5aa0-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5aa0-131">Property</span></span>|<span data-ttu-id="a5aa0-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5aa0-132">Type</span></span>|<span data-ttu-id="a5aa0-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5aa0-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5aa0-134">domainName</span><span class="sxs-lookup"><span data-stu-id="a5aa0-134">domainName</span></span>|<span data-ttu-id="a5aa0-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5aa0-135">String</span></span>|<span data-ttu-id="a5aa0-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a5aa0-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a5aa0-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5aa0-137">Response</span></span>
<span data-ttu-id="a5aa0-138">Se tiver êxito, essa função retornará o código resposta `200 OK` e um Booliano no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5aa0-138">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5aa0-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5aa0-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="a5aa0-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5aa0-140">Request</span></span>
<span data-ttu-id="a5aa0-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5aa0-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="a5aa0-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5aa0-142">Response</span></span>
<span data-ttu-id="a5aa0-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a5aa0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```



