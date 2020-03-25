---
title: 'group: getMemberObjects'
description: 'Retorne todos os grupos dos quais este grupo é um membro. A verificação é transitiva. Observação: Grupos não podem ser membros de funções de diretório, então nenhuma função de diretório retornará.'
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ab08cd3d4abcaef15b27db676fa5d4bc9d0495ed
ms.sourcegitcommit: d0f88dcb7f4c72196c45a00cccbb9fc30b715637
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42927015"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="48e49-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="48e49-105">group: getMemberObjects</span></span>

<span data-ttu-id="48e49-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48e49-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="48e49-p102">Retorne todos os grupos dos quais este grupo é um membro. A verificação é transitiva. Observação: Grupos não podem ser membros de funções de diretório, então nenhuma função de diretório retornará.</span><span class="sxs-lookup"><span data-stu-id="48e49-p102">Return all of the groups that this group is a member of. The check is transitive. Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="48e49-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="48e49-110">Permissions</span></span>
<span data-ttu-id="48e49-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48e49-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48e49-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48e49-113">Permission type</span></span>      | <span data-ttu-id="48e49-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="48e49-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48e49-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48e49-115">Delegated (work or school account)</span></span> | <span data-ttu-id="48e49-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="48e49-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="48e49-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48e49-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48e49-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48e49-118">Not supported.</span></span>    |
|<span data-ttu-id="48e49-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48e49-119">Application</span></span> | <span data-ttu-id="48e49-120">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48e49-120">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="48e49-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48e49-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="48e49-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48e49-122">Request headers</span></span>
| <span data-ttu-id="48e49-123">Nome</span><span class="sxs-lookup"><span data-stu-id="48e49-123">Name</span></span>       | <span data-ttu-id="48e49-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="48e49-124">Type</span></span> | <span data-ttu-id="48e49-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="48e49-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="48e49-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="48e49-126">Authorization</span></span>  | <span data-ttu-id="48e49-127">string</span><span class="sxs-lookup"><span data-stu-id="48e49-127">string</span></span>  | <span data-ttu-id="48e49-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48e49-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48e49-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48e49-130">Request body</span></span>
<span data-ttu-id="48e49-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="48e49-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="48e49-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="48e49-132">Parameter</span></span>    | <span data-ttu-id="48e49-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="48e49-133">Type</span></span>   |<span data-ttu-id="48e49-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="48e49-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48e49-135">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="48e49-135">securityEnabledOnly</span></span>|<span data-ttu-id="48e49-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="48e49-136">Boolean</span></span>| <span data-ttu-id="48e49-p105">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="48e49-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="48e49-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="48e49-139">Response</span></span>
<span data-ttu-id="48e49-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="48e49-140">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="48e49-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48e49-141">Example</span></span>
#### <a name="request"></a><span data-ttu-id="48e49-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48e49-142">Request</span></span>
<span data-ttu-id="48e49-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="48e49-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="48e49-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="48e49-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```
# <a name="c"></a>[<span data-ttu-id="48e49-145">C#</span><span class="sxs-lookup"><span data-stu-id="48e49-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="48e49-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48e49-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="48e49-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48e49-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="48e49-148">Java</span><span class="sxs-lookup"><span data-stu-id="48e49-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="48e49-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="48e49-149">Response</span></span>
<span data-ttu-id="48e49-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="48e49-150">The following is an example of the response.</span></span>
><span data-ttu-id="48e49-151">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="48e49-151">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="48e49-152">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="48e49-152">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
