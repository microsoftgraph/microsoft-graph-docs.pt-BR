---
title: Obter configurações para análise de usuário
description: Recupere as propriedades do objeto de configurações para a análise do usuário.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 90eb06744051c480ed8ab17895fdf6b993912829
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450693"
---
# <a name="get-settings-for-user-analytics"></a><span data-ttu-id="ca6c5-103">Obter configurações para análise de usuário</span><span class="sxs-lookup"><span data-stu-id="ca6c5-103">Get settings for user analytics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca6c5-104">Recupere as propriedades de um objeto de [configurações](../resources/settings.md) conforme aplicável para a API de análise.</span><span class="sxs-lookup"><span data-stu-id="ca6c5-104">Retrieve the properties of a [settings](../resources/settings.md) object as applicable for the analytics API.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca6c5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ca6c5-105">Permissions</span></span>

<span data-ttu-id="ca6c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca6c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ca6c5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca6c5-108">Permission type</span></span>                        | <span data-ttu-id="ca6c5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ca6c5-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ca6c5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca6c5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ca6c5-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="ca6c5-111">User.Read</span></span> |
| <span data-ttu-id="ca6c5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca6c5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca6c5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca6c5-113">Not supported.</span></span> |
| <span data-ttu-id="ca6c5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca6c5-114">Application</span></span>                            | <span data-ttu-id="ca6c5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca6c5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca6c5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca6c5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" }-->

```http
GET https://graph.microsoft.com/beta/me/analytics/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ca6c5-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ca6c5-117">Optional query parameters</span></span>

<span data-ttu-id="ca6c5-118">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ca6c5-118">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca6c5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca6c5-119">Request headers</span></span>

| <span data-ttu-id="ca6c5-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ca6c5-120">Name</span></span>      |<span data-ttu-id="ca6c5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca6c5-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ca6c5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca6c5-122">Authorization</span></span> | <span data-ttu-id="ca6c5-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="ca6c5-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca6c5-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca6c5-124">Request body</span></span>

<span data-ttu-id="ca6c5-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ca6c5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca6c5-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca6c5-126">Response</span></span>

<span data-ttu-id="ca6c5-127">Se bem-sucedido, este método retorna um `200 OK` código de resposta e o objeto de [configurações](../resources/settings.md) solicitadas no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca6c5-127">If successful, this method returns a `200 OK` response code and the requested [settings](../resources/settings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ca6c5-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ca6c5-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ca6c5-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca6c5-129">Request</span></span>

<span data-ttu-id="ca6c5-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca6c5-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->

```http
GET https://graph.microsoft.com/beta/me/analytics/settings
```

### <a name="response"></a><span data-ttu-id="ca6c5-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca6c5-131">Response</span></span>

<span data-ttu-id="ca6c5-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ca6c5-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.settings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('12ab2b12-4b1a-43a1-adac-1a123456cd78')/analytics/settings",
    "hasLicense": true,
    "hasOptedOut": false,
    "hasGraphMailbox": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->