---
title: 'orgContact: listar memberOf'
description: Recupere a lista de grupos e unidades administrativas dos quais o contato é membro.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2f35e63b739fdab47f4f4b256eac78e1e474797c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456261"
---
# <a name="orgcontact-list-memberof"></a><span data-ttu-id="87b54-103">orgContact: listar memberOf</span><span class="sxs-lookup"><span data-stu-id="87b54-103">orgContact: List memberOf</span></span>

<span data-ttu-id="87b54-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="87b54-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87b54-105">Recupere a lista de grupos e unidades administrativas dos quais o contato é membro.</span><span class="sxs-lookup"><span data-stu-id="87b54-105">Retrieve the list of groups and adminstrative units the contact is a member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="87b54-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="87b54-106">Permissions</span></span>
<span data-ttu-id="87b54-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87b54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87b54-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87b54-109">Permission type</span></span>      | <span data-ttu-id="87b54-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="87b54-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87b54-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87b54-111">Delegated (work or school account)</span></span> | <span data-ttu-id="87b54-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="87b54-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="87b54-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87b54-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87b54-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87b54-114">Not supported.</span></span>    |
|<span data-ttu-id="87b54-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87b54-115">Application</span></span> | <span data-ttu-id="87b54-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87b54-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="87b54-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87b54-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="87b54-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="87b54-118">Optional query parameters</span></span>
<span data-ttu-id="87b54-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="87b54-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87b54-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87b54-120">Request headers</span></span>
| <span data-ttu-id="87b54-121">Nome</span><span class="sxs-lookup"><span data-stu-id="87b54-121">Name</span></span>       | <span data-ttu-id="87b54-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="87b54-122">Type</span></span> | <span data-ttu-id="87b54-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="87b54-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="87b54-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="87b54-124">Authorization</span></span>  | <span data-ttu-id="87b54-125">string</span><span class="sxs-lookup"><span data-stu-id="87b54-125">string</span></span>  | <span data-ttu-id="87b54-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87b54-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87b54-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87b54-128">Request body</span></span>
<span data-ttu-id="87b54-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="87b54-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87b54-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="87b54-130">Response</span></span>

<span data-ttu-id="87b54-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87b54-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="87b54-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87b54-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="87b54-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87b54-133">Request</span></span>
<span data-ttu-id="87b54-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87b54-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="87b54-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="87b54-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contact_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="87b54-136">C#</span><span class="sxs-lookup"><span data-stu-id="87b54-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contact-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="87b54-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87b54-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contact-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="87b54-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87b54-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contact-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="87b54-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="87b54-139">Response</span></span>
<span data-ttu-id="87b54-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87b54-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
