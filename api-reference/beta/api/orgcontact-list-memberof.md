---
title: 'orgContact: listar memberOf'
description: Recupere a lista de grupos e unidades administrativas dos quais o contato é membro.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 385a4d95fab9de318b5fcd9aba58a94d66fc522f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867747"
---
# <a name="orgcontact-list-memberof"></a><span data-ttu-id="b1f07-103">orgContact: listar memberOf</span><span class="sxs-lookup"><span data-stu-id="b1f07-103">orgContact: List memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1f07-104">Recupere a lista de grupos e unidades administrativas dos quais o contato é membro.</span><span class="sxs-lookup"><span data-stu-id="b1f07-104">Retrieve the list of groups and adminstrative units the contact is a member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1f07-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b1f07-105">Permissions</span></span>
<span data-ttu-id="b1f07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1f07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1f07-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1f07-108">Permission type</span></span>      | <span data-ttu-id="b1f07-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b1f07-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1f07-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1f07-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b1f07-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b1f07-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b1f07-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1f07-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1f07-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1f07-113">Not supported.</span></span>    |
|<span data-ttu-id="b1f07-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1f07-114">Application</span></span> | <span data-ttu-id="b1f07-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1f07-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="b1f07-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1f07-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b1f07-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b1f07-117">Optional query parameters</span></span>
<span data-ttu-id="b1f07-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b1f07-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b1f07-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1f07-119">Request headers</span></span>
| <span data-ttu-id="b1f07-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b1f07-120">Name</span></span>       | <span data-ttu-id="b1f07-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1f07-121">Type</span></span> | <span data-ttu-id="b1f07-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1f07-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b1f07-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1f07-123">Authorization</span></span>  | <span data-ttu-id="b1f07-124">string</span><span class="sxs-lookup"><span data-stu-id="b1f07-124">string</span></span>  | <span data-ttu-id="b1f07-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1f07-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1f07-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1f07-127">Request body</span></span>
<span data-ttu-id="b1f07-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b1f07-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1f07-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1f07-129">Response</span></span>

<span data-ttu-id="b1f07-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1f07-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b1f07-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1f07-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1f07-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1f07-132">Request</span></span>
<span data-ttu-id="b1f07-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1f07-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b1f07-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1f07-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contact_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/{id}/memberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b1f07-135">C#</span><span class="sxs-lookup"><span data-stu-id="b1f07-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contact-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b1f07-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1f07-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contact-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b1f07-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1f07-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contact-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b1f07-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1f07-138">Response</span></span>
<span data-ttu-id="b1f07-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1f07-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
