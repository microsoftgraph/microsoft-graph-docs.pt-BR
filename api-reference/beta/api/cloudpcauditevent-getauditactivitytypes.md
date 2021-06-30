---
title: 'cloudPcAuditEvent: getAuditActivityTypes'
description: Obter tipos de atividade de auditoria por id de locatário.
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: a6e5fd01d0b2100affa6b5d89c43a50cddbaa533
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211191"
---
# <a name="cloudpcauditevent-getauditactivitytypes"></a><span data-ttu-id="04fcd-103">cloudPcAuditEvent: getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="04fcd-103">cloudPcAuditEvent: getAuditActivityTypes</span></span>

<span data-ttu-id="04fcd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04fcd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04fcd-105">Obter tipos de atividade de auditoria por ID de locatário.</span><span class="sxs-lookup"><span data-stu-id="04fcd-105">Get audit activity types by tenant ID.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="04fcd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="04fcd-106">Permissions</span></span>

<span data-ttu-id="04fcd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04fcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04fcd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04fcd-109">Permission type</span></span>| <span data-ttu-id="04fcd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="04fcd-110">Permissions (from least to most privileged)</span></span> |
|:---|:---|
|<span data-ttu-id="04fcd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04fcd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="04fcd-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04fcd-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="04fcd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04fcd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04fcd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04fcd-114">Not supported.</span></span>|
|<span data-ttu-id="04fcd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04fcd-115">Application</span></span>|<span data-ttu-id="04fcd-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04fcd-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="04fcd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04fcd-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="04fcd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04fcd-118">Request headers</span></span>

| <span data-ttu-id="04fcd-119">Nome</span><span class="sxs-lookup"><span data-stu-id="04fcd-119">Name</span></span>          | <span data-ttu-id="04fcd-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="04fcd-120">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="04fcd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="04fcd-121">Authorization</span></span> | <span data-ttu-id="04fcd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04fcd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04fcd-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04fcd-124">Request body</span></span>

<span data-ttu-id="04fcd-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="04fcd-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04fcd-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="04fcd-126">Response</span></span>

<span data-ttu-id="04fcd-127">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04fcd-127">If successful, this method returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="04fcd-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="04fcd-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="04fcd-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04fcd-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "cloudpcauditevent_getauditactivitytypes"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/auditEvents/getAuditActivityTypes
```

### <a name="response"></a><span data-ttu-id="04fcd-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="04fcd-130">Response</span></span>


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    "Get Audit Activity Types value"
  ]
}
```
