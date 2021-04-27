---
title: Get privilegedRole
description: 'Recupere as propriedades e as relações do objeto privilegedRole. '
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 6eb4838d23ed501ee2875e9aef3484752692584f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055271"
---
# <a name="get-privilegedrole"></a><span data-ttu-id="62d43-103">Get privilegedRole</span><span class="sxs-lookup"><span data-stu-id="62d43-103">Get privilegedRole</span></span>

<span data-ttu-id="62d43-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62d43-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62d43-105">Recupere as propriedades e as relações do [objeto privilegedRole.](../resources/privilegedrole.md)</span><span class="sxs-lookup"><span data-stu-id="62d43-105">Retrieve the properties and relationships of [privilegedRole](../resources/privilegedrole.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="62d43-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="62d43-106">Permissions</span></span>
<span data-ttu-id="62d43-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62d43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="62d43-109">O solicitante precisa ter uma das seguintes funções: Administrador de Função _Privilegiada,_ _Administrador Global,_ Administrador de Segurança _ou_ Leitor de _Segurança._</span><span class="sxs-lookup"><span data-stu-id="62d43-109">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="62d43-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62d43-110">Permission type</span></span>      | <span data-ttu-id="62d43-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="62d43-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62d43-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62d43-112">Delegated (work or school account)</span></span> | <span data-ttu-id="62d43-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="62d43-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="62d43-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62d43-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62d43-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62d43-115">Not supported.</span></span>    |
|<span data-ttu-id="62d43-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62d43-116">Application</span></span> | <span data-ttu-id="62d43-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62d43-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="62d43-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62d43-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}
GET /privilegedRoleAssignments/{id}/roleInfo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="62d43-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="62d43-119">Optional query parameters</span></span>
<span data-ttu-id="62d43-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="62d43-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="62d43-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62d43-121">Request headers</span></span>
| <span data-ttu-id="62d43-122">Nome</span><span class="sxs-lookup"><span data-stu-id="62d43-122">Name</span></span>      |<span data-ttu-id="62d43-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="62d43-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="62d43-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="62d43-124">Authorization</span></span>  | <span data-ttu-id="62d43-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62d43-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62d43-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62d43-127">Request body</span></span>
<span data-ttu-id="62d43-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="62d43-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62d43-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="62d43-129">Response</span></span>

<span data-ttu-id="62d43-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [privilegedRole](../resources/privilegedrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62d43-130">If successful, this method returns a `200 OK` response code and [privilegedRole](../resources/privilegedrole.md) object in the response body.</span></span>

<span data-ttu-id="62d43-131">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="62d43-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="62d43-132">Caso contrário, o código de status HTTP 403 Forbidden será retornado.</span><span class="sxs-lookup"><span data-stu-id="62d43-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="62d43-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62d43-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="62d43-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62d43-134">Request</span></span>
<span data-ttu-id="62d43-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62d43-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="62d43-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="62d43-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedrole"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles/{id}
```
# <a name="c"></a>[<span data-ttu-id="62d43-137">C#</span><span class="sxs-lookup"><span data-stu-id="62d43-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62d43-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62d43-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62d43-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62d43-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="62d43-140">Java</span><span class="sxs-lookup"><span data-stu-id="62d43-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="62d43-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="62d43-141">Response</span></span>
<span data-ttu-id="62d43-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62d43-142">Here is an example of the response.</span></span> <span data-ttu-id="62d43-143">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="62d43-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 46

{
  "id": "id-value",
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
