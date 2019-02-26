---
title: Função getAuditCategories
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e85bf6031e881025fe62e902e66add87b0b7c4da
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261639"
---
# <a name="getauditcategories-function"></a><span data-ttu-id="d3902-103">Função getAuditCategories</span><span class="sxs-lookup"><span data-stu-id="d3902-103">getAuditCategories function</span></span>

> <span data-ttu-id="d3902-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d3902-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3902-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d3902-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3902-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d3902-106">Prerequisites</span></span>
<span data-ttu-id="d3902-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d3902-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d3902-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3902-109">Permission type</span></span>|<span data-ttu-id="d3902-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d3902-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3902-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3902-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d3902-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3902-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d3902-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3902-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3902-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3902-114">Not supported.</span></span>|
|<span data-ttu-id="d3902-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3902-115">Application</span></span>|<span data-ttu-id="d3902-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3902-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3902-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3902-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditCategories
```

## <a name="request-headers"></a><span data-ttu-id="d3902-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3902-118">Request headers</span></span>
|<span data-ttu-id="d3902-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3902-119">Header</span></span>|<span data-ttu-id="d3902-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d3902-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3902-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3902-121">Authorization</span></span>|<span data-ttu-id="d3902-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3902-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3902-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d3902-123">Accept</span></span>|<span data-ttu-id="d3902-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d3902-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3902-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3902-125">Request body</span></span>
<span data-ttu-id="d3902-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d3902-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3902-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3902-127">Response</span></span>
<span data-ttu-id="d3902-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3902-128">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3902-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3902-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3902-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3902-130">Request</span></span>
<span data-ttu-id="d3902-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3902-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditCategories
```

### <a name="response"></a><span data-ttu-id="d3902-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3902-132">Response</span></span>
<span data-ttu-id="d3902-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3902-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



