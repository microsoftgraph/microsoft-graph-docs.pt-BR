---
title: Função getAuditCategories
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8a1363f2aef76d5ce2e6c4f9e3e1e20c3bd7d0bf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001905"
---
# <a name="getauditcategories-function"></a><span data-ttu-id="9fb3c-103">Função getAuditCategories</span><span class="sxs-lookup"><span data-stu-id="9fb3c-103">getAuditCategories function</span></span>

> <span data-ttu-id="9fb3c-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9fb3c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fb3c-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9fb3c-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9fb3c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9fb3c-106">Prerequisites</span></span>
<span data-ttu-id="9fb3c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fb3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fb3c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9fb3c-109">Permission type</span></span>|<span data-ttu-id="9fb3c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9fb3c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fb3c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9fb3c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9fb3c-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fb3c-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9fb3c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9fb3c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fb3c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fb3c-114">Not supported.</span></span>|
|<span data-ttu-id="9fb3c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9fb3c-115">Application</span></span>|<span data-ttu-id="9fb3c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fb3c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fb3c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9fb3c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditCategories
```

## <a name="request-headers"></a><span data-ttu-id="9fb3c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9fb3c-118">Request headers</span></span>
|<span data-ttu-id="9fb3c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9fb3c-119">Header</span></span>|<span data-ttu-id="9fb3c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="9fb3c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fb3c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9fb3c-121">Authorization</span></span>|<span data-ttu-id="9fb3c-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fb3c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fb3c-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9fb3c-123">Accept</span></span>|<span data-ttu-id="9fb3c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9fb3c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fb3c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9fb3c-125">Request body</span></span>
<span data-ttu-id="9fb3c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9fb3c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fb3c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fb3c-127">Response</span></span>
<span data-ttu-id="9fb3c-128">Se tiver êxito, essa função retornará o código de resposta `200 OK` e a Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9fb3c-128">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fb3c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9fb3c-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="9fb3c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9fb3c-130">Request</span></span>
<span data-ttu-id="9fb3c-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9fb3c-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditCategories
```

### <a name="response"></a><span data-ttu-id="9fb3c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fb3c-132">Response</span></span>
<span data-ttu-id="9fb3c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9fb3c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



