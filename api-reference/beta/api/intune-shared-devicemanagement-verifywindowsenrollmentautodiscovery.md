---
title: Função verifyWindowsEnrollmentAutoDiscovery
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ee4dbb7e5eacd30f1be31f9996b5b6304f9bfc4e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965309"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="82225-103">Função verifyWindowsEnrollmentAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="82225-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="82225-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="82225-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="82225-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="82225-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="82225-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="82225-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82225-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="82225-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="82225-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="82225-108">Prerequisites</span></span>
<span data-ttu-id="82225-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82225-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82225-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82225-111">Permission type</span></span>|<span data-ttu-id="82225-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="82225-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82225-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82225-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="82225-114">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="82225-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="82225-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82225-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="82225-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82225-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82225-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82225-117">Not supported.</span></span>|
|<span data-ttu-id="82225-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82225-118">Application</span></span>|<span data-ttu-id="82225-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82225-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82225-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82225-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="82225-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82225-121">Request headers</span></span>
|<span data-ttu-id="82225-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="82225-122">Header</span></span>|<span data-ttu-id="82225-123">Valor</span><span class="sxs-lookup"><span data-stu-id="82225-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82225-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="82225-124">Authorization</span></span>|<span data-ttu-id="82225-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82225-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82225-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="82225-126">Accept</span></span>|<span data-ttu-id="82225-127">application/json</span><span class="sxs-lookup"><span data-stu-id="82225-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82225-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82225-128">Request body</span></span>
<span data-ttu-id="82225-129">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="82225-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="82225-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="82225-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="82225-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82225-131">Property</span></span>|<span data-ttu-id="82225-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="82225-132">Type</span></span>|<span data-ttu-id="82225-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="82225-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82225-134">domainName</span><span class="sxs-lookup"><span data-stu-id="82225-134">domainName</span></span>|<span data-ttu-id="82225-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82225-135">String</span></span>|<span data-ttu-id="82225-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="82225-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="82225-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="82225-137">Response</span></span>
<span data-ttu-id="82225-138">Se tiver êxito, essa função retornará o código resposta `200 OK` e um Booliano no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="82225-138">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82225-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82225-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="82225-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82225-140">Request</span></span>
<span data-ttu-id="82225-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="82225-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="82225-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="82225-142">Response</span></span>
<span data-ttu-id="82225-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="82225-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```



