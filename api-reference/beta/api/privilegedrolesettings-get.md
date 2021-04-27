---
title: Get privilegedRoleSettings
description: Recupere as configurações de função para a função determinada. Um objeto privilegedRoleSettings será retornado.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 73c2a01c171ec39f2702b5bf9ce6a3138a93456b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052884"
---
# <a name="get-privilegedrolesettings"></a><span data-ttu-id="42043-104">Get privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="42043-104">Get privilegedRoleSettings</span></span>

<span data-ttu-id="42043-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42043-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42043-106">Recupere as configurações de função para a função determinada.</span><span class="sxs-lookup"><span data-stu-id="42043-106">Retrieve the role settings for the given role.</span></span> <span data-ttu-id="42043-107">Um [objeto privilegedRoleSettings](../resources/privilegedrolesettings.md) será retornado.</span><span class="sxs-lookup"><span data-stu-id="42043-107">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="42043-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="42043-108">Permissions</span></span>

<span data-ttu-id="42043-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42043-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="42043-111">O solicitante precisa ter uma das seguintes funções: Administrador de Função _Privilegiada,_ _Administrador Global,_ Administrador de Segurança _ou_ Leitor de _Segurança._</span><span class="sxs-lookup"><span data-stu-id="42043-111">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="42043-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42043-112">Permission type</span></span>      | <span data-ttu-id="42043-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42043-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42043-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42043-114">Delegated (work or school account)</span></span> | <span data-ttu-id="42043-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="42043-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="42043-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42043-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42043-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42043-117">Not supported.</span></span>    |
|<span data-ttu-id="42043-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42043-118">Application</span></span> | <span data-ttu-id="42043-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42043-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="42043-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42043-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="42043-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="42043-121">Optional query parameters</span></span>
<span data-ttu-id="42043-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="42043-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="42043-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42043-123">Request headers</span></span>
| <span data-ttu-id="42043-124">Nome</span><span class="sxs-lookup"><span data-stu-id="42043-124">Name</span></span>      |<span data-ttu-id="42043-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="42043-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="42043-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="42043-126">Authorization</span></span>  | <span data-ttu-id="42043-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42043-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42043-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42043-129">Request body</span></span>
<span data-ttu-id="42043-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="42043-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42043-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="42043-131">Response</span></span>

<span data-ttu-id="42043-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [privilegedRoleSettings](../resources/privilegedrolesettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42043-132">If successful, this method returns a `200 OK` response code and [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.</span></span>

<span data-ttu-id="42043-133">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="42043-133">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="42043-134">Caso contrário, o código de status HTTP 403 Forbidden será retornado.</span><span class="sxs-lookup"><span data-stu-id="42043-134">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="42043-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42043-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42043-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42043-136">Request</span></span>
<span data-ttu-id="42043-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42043-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="42043-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="42043-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
```
# <a name="c"></a>[<span data-ttu-id="42043-139">C#</span><span class="sxs-lookup"><span data-stu-id="42043-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedrolesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42043-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42043-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedrolesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42043-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42043-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedrolesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="42043-142">Java</span><span class="sxs-lookup"><span data-stu-id="42043-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedrolesettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="42043-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="42043-143">Response</span></span>
<span data-ttu-id="42043-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42043-144">Here is an example of the response.</span></span> <span data-ttu-id="42043-145">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="42043-145">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 228

{
  "minElevationDuration": "2016-10-19T10:37:00Z",
  "maxElavationDuration": "2016-10-19T10:37:00Z",
  "elevationDuration": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
