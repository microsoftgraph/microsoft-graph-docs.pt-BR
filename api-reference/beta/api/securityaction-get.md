---
title: Obter ação de segurança
description: Recupere as propriedades e os relacionamentos do objeto SecurityAction.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 336a8a73d0ec161f26dd3fcbd36caf86097108f5
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366914"
---
# <a name="get-security-action"></a><span data-ttu-id="47547-103">Obter ação de segurança</span><span class="sxs-lookup"><span data-stu-id="47547-103">Get security action</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47547-104">Recupere as propriedades e os relacionamentos de [](../resources/securityaction.md) um objeto SecurityAction.</span><span class="sxs-lookup"><span data-stu-id="47547-104">Retrieve the properties and relationships of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="47547-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="47547-105">Permissions</span></span>

<span data-ttu-id="47547-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47547-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="47547-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47547-108">Permission type</span></span>                        | <span data-ttu-id="47547-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47547-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="47547-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47547-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="47547-111">SecurityActions. Read. All, SecurityActions. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="47547-111">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span></span> |
| <span data-ttu-id="47547-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47547-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47547-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47547-113">Not supported.</span></span> |
| <span data-ttu-id="47547-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47547-114">Application</span></span>                            | <span data-ttu-id="47547-115">SecurityActions. Read. All, SecurityActions. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="47547-115">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="47547-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47547-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securityActions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="47547-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="47547-117">Optional query parameters</span></span>

<span data-ttu-id="47547-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="47547-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="47547-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="47547-119">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="47547-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47547-120">Request headers</span></span>

| <span data-ttu-id="47547-121">Nome</span><span class="sxs-lookup"><span data-stu-id="47547-121">Name</span></span>      |<span data-ttu-id="47547-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="47547-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="47547-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="47547-123">Authorization</span></span> | <span data-ttu-id="47547-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="47547-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="47547-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47547-125">Request body</span></span>

<span data-ttu-id="47547-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47547-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47547-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="47547-127">Response</span></span>

<span data-ttu-id="47547-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [SecurityAction](../resources/securityaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47547-128">If successful, this method returns a `200 OK` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="47547-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="47547-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="47547-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47547-130">Request</span></span>

<span data-ttu-id="47547-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="47547-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_securityaction"
}-->

```http
GET https://graph.microsoft.com/beta/security/securityActions/{id}
```

### <a name="response"></a><span data-ttu-id="47547-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="47547-132">Response</span></span>

<span data-ttu-id="47547-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="47547-133">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="47547-134">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="47547-134">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="47547-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="47547-135">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securityAction"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "actionReason": "actionReason-value",
  "appId": "appId-value",
  "azureTenantId": "azureTenantId-value",
  "clientContext": "clientContext-value",
  "completedDateTime": "datetime-value",
  "createdDateTime": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get securityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
