---
title: Função getAuditCategories
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 513df3b403bcde9839ff2a1e9a7e8568c5720d67
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959297"
---
# <a name="getauditcategories-function"></a><span data-ttu-id="9462f-103">Função getAuditCategories</span><span class="sxs-lookup"><span data-stu-id="9462f-103">getAuditCategories function</span></span>

> <span data-ttu-id="9462f-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9462f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9462f-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9462f-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9462f-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9462f-106">Prerequisites</span></span>
<span data-ttu-id="9462f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9462f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9462f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9462f-109">Permission type</span></span>|<span data-ttu-id="9462f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9462f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9462f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9462f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9462f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9462f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9462f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9462f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9462f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9462f-114">Not supported.</span></span>|
|<span data-ttu-id="9462f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9462f-115">Application</span></span>|<span data-ttu-id="9462f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9462f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9462f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9462f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditCategories
```

## <a name="request-headers"></a><span data-ttu-id="9462f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9462f-118">Request headers</span></span>
|<span data-ttu-id="9462f-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9462f-119">Header</span></span>|<span data-ttu-id="9462f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="9462f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9462f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9462f-121">Authorization</span></span>|<span data-ttu-id="9462f-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9462f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9462f-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9462f-123">Accept</span></span>|<span data-ttu-id="9462f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9462f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9462f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9462f-125">Request body</span></span>
<span data-ttu-id="9462f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9462f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9462f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9462f-127">Response</span></span>
<span data-ttu-id="9462f-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9462f-128">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9462f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9462f-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="9462f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9462f-130">Request</span></span>
<span data-ttu-id="9462f-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9462f-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditCategories
```

### <a name="response"></a><span data-ttu-id="9462f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="9462f-132">Response</span></span>
<span data-ttu-id="9462f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9462f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 57

{
  "value": [
    "Get Audit Categories value"
  ]
}
```



