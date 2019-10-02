---
title: Função getAuditCategories
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e4936bbd47b22440e96e27df85002c98c016aeb0
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354844"
---
# <a name="getauditcategories-function"></a><span data-ttu-id="e6b93-103">Função getAuditCategories</span><span class="sxs-lookup"><span data-stu-id="e6b93-103">getAuditCategories function</span></span>

> <span data-ttu-id="e6b93-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e6b93-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6b93-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e6b93-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6b93-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e6b93-106">Prerequisites</span></span>
<span data-ttu-id="e6b93-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6b93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6b93-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6b93-109">Permission type</span></span>|<span data-ttu-id="e6b93-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e6b93-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6b93-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6b93-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e6b93-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6b93-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e6b93-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6b93-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6b93-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6b93-114">Not supported.</span></span>|
|<span data-ttu-id="e6b93-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6b93-115">Application</span></span>|<span data-ttu-id="e6b93-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6b93-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6b93-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6b93-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditCategories
```

## <a name="request-headers"></a><span data-ttu-id="e6b93-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6b93-118">Request headers</span></span>
|<span data-ttu-id="e6b93-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e6b93-119">Header</span></span>|<span data-ttu-id="e6b93-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e6b93-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6b93-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6b93-121">Authorization</span></span>|<span data-ttu-id="e6b93-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6b93-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6b93-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e6b93-123">Accept</span></span>|<span data-ttu-id="e6b93-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e6b93-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6b93-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6b93-125">Request body</span></span>
<span data-ttu-id="e6b93-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e6b93-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6b93-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6b93-127">Response</span></span>
<span data-ttu-id="e6b93-128">Se tiver êxito, essa função retornará o código de resposta `200 OK` e a Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6b93-128">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6b93-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6b93-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6b93-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6b93-130">Request</span></span>
<span data-ttu-id="e6b93-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6b93-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditCategories
```

### <a name="response"></a><span data-ttu-id="e6b93-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6b93-132">Response</span></span>
<span data-ttu-id="e6b93-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6b93-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




