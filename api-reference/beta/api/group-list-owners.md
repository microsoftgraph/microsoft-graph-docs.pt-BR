---
title: Listar proprietários
description: Recupere uma lista dos proprietários do grupo.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 64ee4d48713518dd9b4005cf6932dfc90932195c
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681533"
---
# <a name="list-owners"></a><span data-ttu-id="fa61c-103">Listar proprietários</span><span class="sxs-lookup"><span data-stu-id="fa61c-103">List owners</span></span>

<span data-ttu-id="fa61c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa61c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa61c-105">Recupere uma lista dos proprietários do grupo.</span><span class="sxs-lookup"><span data-stu-id="fa61c-105">Retrieve a list of the group's owners.</span></span> <span data-ttu-id="fa61c-106">Os proprietários são um conjunto de usuários que têm permissão para modificar o objeto group.</span><span class="sxs-lookup"><span data-stu-id="fa61c-106">The owners are a set of users who are allowed to modify the group object.</span></span> <span data-ttu-id="fa61c-107">Os proprietários não estão atualmente disponíveis no Microsoft Graph para os grupos que foram criados no Exchange ou grupos que são sincronizados a partir de um ambiente no local.</span><span class="sxs-lookup"><span data-stu-id="fa61c-107">Owners are currently not available in Microsoft Graph for groups that were created in Exchange or groups that are synchronized from an on-premises environment.</span></span> 

## <a name="permissions"></a><span data-ttu-id="fa61c-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa61c-108">Permissions</span></span>
<span data-ttu-id="fa61c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa61c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa61c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa61c-111">Permission type</span></span>      | <span data-ttu-id="fa61c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa61c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa61c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa61c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fa61c-114">GroupMember.Read.All, Group.Read.All, Group.Member.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fa61c-114">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="fa61c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa61c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa61c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa61c-116">Not supported.</span></span>    |
|<span data-ttu-id="fa61c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa61c-117">Application</span></span> | <span data-ttu-id="fa61c-118">GroupMember.Read.All, Group.Read.All, Group.Member.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fa61c-118">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>  |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="fa61c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa61c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa61c-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fa61c-120">Optional query parameters</span></span>
<span data-ttu-id="fa61c-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fa61c-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa61c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa61c-122">Request headers</span></span>
| <span data-ttu-id="fa61c-123">Nome</span><span class="sxs-lookup"><span data-stu-id="fa61c-123">Name</span></span>       | <span data-ttu-id="fa61c-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa61c-124">Type</span></span> | <span data-ttu-id="fa61c-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa61c-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fa61c-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa61c-126">Authorization</span></span>  | <span data-ttu-id="fa61c-127">string</span><span class="sxs-lookup"><span data-stu-id="fa61c-127">string</span></span>  | <span data-ttu-id="fa61c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa61c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa61c-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa61c-130">Request body</span></span>
<span data-ttu-id="fa61c-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fa61c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa61c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa61c-132">Response</span></span>
<span data-ttu-id="fa61c-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa61c-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa61c-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa61c-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fa61c-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa61c-135">Request</span></span>
<span data-ttu-id="fa61c-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa61c-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fa61c-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa61c-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="fa61c-138">C#</span><span class="sxs-lookup"><span data-stu-id="fa61c-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fa61c-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa61c-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fa61c-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa61c-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fa61c-141">Java</span><span class="sxs-lookup"><span data-stu-id="fa61c-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fa61c-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa61c-142">Response</span></span>
<span data-ttu-id="fa61c-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fa61c-143">The following is an example of the response.</span></span>
><span data-ttu-id="fa61c-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fa61c-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


