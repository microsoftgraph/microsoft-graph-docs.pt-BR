---
title: função getUserIdsWithFlaggedAppRegistration
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f24e79ef87af4e7f4f2948dbcc56e23d0bd1822d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968201"
---
# <a name="getuseridswithflaggedappregistration-function"></a><span data-ttu-id="d8cc1-103">função getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="d8cc1-103">getUserIdsWithFlaggedAppRegistration function</span></span>

> <span data-ttu-id="d8cc1-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d8cc1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8cc1-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d8cc1-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d8cc1-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d8cc1-106">Prerequisites</span></span>
<span data-ttu-id="d8cc1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8cc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8cc1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8cc1-109">Permission type</span></span>|<span data-ttu-id="d8cc1-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d8cc1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8cc1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8cc1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d8cc1-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8cc1-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d8cc1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8cc1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8cc1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8cc1-114">Not supported.</span></span>|
|<span data-ttu-id="d8cc1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8cc1-115">Application</span></span>|<span data-ttu-id="d8cc1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8cc1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8cc1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8cc1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

## <a name="request-headers"></a><span data-ttu-id="d8cc1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8cc1-118">Request headers</span></span>
|<span data-ttu-id="d8cc1-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d8cc1-119">Header</span></span>|<span data-ttu-id="d8cc1-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d8cc1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8cc1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8cc1-121">Authorization</span></span>|<span data-ttu-id="d8cc1-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8cc1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8cc1-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d8cc1-123">Accept</span></span>|<span data-ttu-id="d8cc1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d8cc1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8cc1-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8cc1-125">Request body</span></span>
<span data-ttu-id="d8cc1-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d8cc1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8cc1-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8cc1-127">Response</span></span>
<span data-ttu-id="d8cc1-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8cc1-128">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8cc1-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8cc1-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="d8cc1-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8cc1-130">Request</span></span>
<span data-ttu-id="d8cc1-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8cc1-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

### <a name="response"></a><span data-ttu-id="d8cc1-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8cc1-132">Response</span></span>
<span data-ttu-id="d8cc1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8cc1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



