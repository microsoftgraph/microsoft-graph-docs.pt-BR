---
title: função getUserIdsWithFlaggedAppRegistration
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: e98c25e1a3ac15372f2f3e811fab7e4d7b047794
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362766"
---
# <a name="getuseridswithflaggedappregistration-function"></a><span data-ttu-id="ab7ae-103">função getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="ab7ae-103">getUserIdsWithFlaggedAppRegistration function</span></span>

> <span data-ttu-id="ab7ae-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ab7ae-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab7ae-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ab7ae-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ab7ae-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ab7ae-106">Prerequisites</span></span>
<span data-ttu-id="ab7ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab7ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab7ae-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab7ae-109">Permission type</span></span>|<span data-ttu-id="ab7ae-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ab7ae-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab7ae-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab7ae-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ab7ae-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab7ae-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ab7ae-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab7ae-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab7ae-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab7ae-114">Not supported.</span></span>|
|<span data-ttu-id="ab7ae-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab7ae-115">Application</span></span>|<span data-ttu-id="ab7ae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab7ae-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab7ae-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab7ae-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

## <a name="request-headers"></a><span data-ttu-id="ab7ae-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab7ae-118">Request headers</span></span>
|<span data-ttu-id="ab7ae-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ab7ae-119">Header</span></span>|<span data-ttu-id="ab7ae-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ab7ae-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab7ae-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab7ae-121">Authorization</span></span>|<span data-ttu-id="ab7ae-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab7ae-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab7ae-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ab7ae-123">Accept</span></span>|<span data-ttu-id="ab7ae-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ab7ae-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab7ae-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab7ae-125">Request body</span></span>
<span data-ttu-id="ab7ae-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ab7ae-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab7ae-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab7ae-127">Response</span></span>
<span data-ttu-id="ab7ae-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab7ae-128">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab7ae-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab7ae-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="ab7ae-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab7ae-130">Request</span></span>
<span data-ttu-id="ab7ae-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab7ae-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

### <a name="response"></a><span data-ttu-id="ab7ae-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab7ae-132">Response</span></span>
<span data-ttu-id="ab7ae-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab7ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



