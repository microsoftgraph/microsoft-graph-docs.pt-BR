---
title: função getUserIdsWithFlaggedAppRegistration
description: Ainda não documentado
ms.openlocfilehash: a33f59c1dab1cbdfb34dd62924d8724e71ac2e7e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004798"
---
# <a name="getuseridswithflaggedappregistration-function"></a><span data-ttu-id="97114-103">função getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="97114-103">getUserIdsWithFlaggedAppRegistration function</span></span>

> <span data-ttu-id="97114-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="97114-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97114-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="97114-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="97114-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="97114-106">Prerequisites</span></span>
<span data-ttu-id="97114-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97114-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97114-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97114-109">Permission type</span></span>|<span data-ttu-id="97114-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="97114-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97114-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97114-111">Delegated (work or school account)</span></span>|<span data-ttu-id="97114-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="97114-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="97114-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97114-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97114-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97114-114">Not supported.</span></span>|
|<span data-ttu-id="97114-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97114-115">Application</span></span>|<span data-ttu-id="97114-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97114-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97114-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97114-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

## <a name="request-headers"></a><span data-ttu-id="97114-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97114-118">Request headers</span></span>
|<span data-ttu-id="97114-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="97114-119">Header</span></span>|<span data-ttu-id="97114-120">Valor</span><span class="sxs-lookup"><span data-stu-id="97114-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97114-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="97114-121">Authorization</span></span>|<span data-ttu-id="97114-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97114-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97114-123">Accept</span><span class="sxs-lookup"><span data-stu-id="97114-123">Accept</span></span>|<span data-ttu-id="97114-124">application/json</span><span class="sxs-lookup"><span data-stu-id="97114-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97114-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97114-125">Request body</span></span>
<span data-ttu-id="97114-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="97114-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97114-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="97114-127">Response</span></span>
<span data-ttu-id="97114-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97114-128">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97114-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97114-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="97114-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97114-130">Request</span></span>
<span data-ttu-id="97114-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97114-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

### <a name="response"></a><span data-ttu-id="97114-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="97114-132">Response</span></span>
<span data-ttu-id="97114-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97114-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 79

{
  "value": [
    "Get User Ids With Flagged App Registration value"
  ]
}
```



