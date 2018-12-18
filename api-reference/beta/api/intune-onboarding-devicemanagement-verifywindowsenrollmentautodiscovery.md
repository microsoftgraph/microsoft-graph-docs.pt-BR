---
title: Função verifyWindowsEnrollmentAutoDiscovery
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: c093490b27db844db434b05725e48464d9792cb7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344804"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="8d189-103">Função verifyWindowsEnrollmentAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="8d189-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="8d189-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8d189-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d189-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8d189-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8d189-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8d189-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d189-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8d189-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8d189-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8d189-108">Prerequisites</span></span>
<span data-ttu-id="8d189-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d189-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d189-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d189-111">Permission type</span></span>|<span data-ttu-id="8d189-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8d189-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d189-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d189-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d189-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d189-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8d189-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d189-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d189-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d189-116">Not supported.</span></span>|
|<span data-ttu-id="8d189-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d189-117">Application</span></span>|<span data-ttu-id="8d189-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d189-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d189-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d189-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="8d189-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d189-120">Request headers</span></span>
|<span data-ttu-id="8d189-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8d189-121">Header</span></span>|<span data-ttu-id="8d189-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8d189-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d189-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d189-123">Authorization</span></span>|<span data-ttu-id="8d189-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d189-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d189-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8d189-125">Accept</span></span>|<span data-ttu-id="8d189-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d189-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d189-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d189-127">Request body</span></span>
<span data-ttu-id="8d189-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="8d189-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="8d189-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="8d189-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="8d189-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d189-130">Property</span></span>|<span data-ttu-id="8d189-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d189-131">Type</span></span>|<span data-ttu-id="8d189-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d189-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d189-133">domainName</span><span class="sxs-lookup"><span data-stu-id="8d189-133">domainName</span></span>|<span data-ttu-id="8d189-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d189-134">String</span></span>|<span data-ttu-id="8d189-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8d189-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8d189-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d189-136">Response</span></span>
<span data-ttu-id="8d189-137">Se tiver êxito, essa função retornará o código resposta `200 OK` e um Booliano no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d189-137">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d189-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d189-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="8d189-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d189-139">Request</span></span>
<span data-ttu-id="8d189-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d189-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="8d189-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d189-141">Response</span></span>
<span data-ttu-id="8d189-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8d189-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```





