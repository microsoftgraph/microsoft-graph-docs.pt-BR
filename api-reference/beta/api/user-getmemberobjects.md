---
title: 'user: getMemberObjects'
description: Retorna todos os grupos e funções de diretório e unidades administrativas dos quais o usuário é membro. A verificação é transitiva.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: a681a4edfe244bd835d7fe07d5aac3ceeedff472
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053367"
---
# <a name="user-getmemberobjects"></a><span data-ttu-id="b2acf-104">user: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="b2acf-104">user: getMemberObjects</span></span>

<span data-ttu-id="b2acf-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2acf-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2acf-p102">Retorna todos os grupos e funções de diretório e unidades administrativas dos quais o usuário é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="b2acf-p102">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2acf-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b2acf-108">Permissions</span></span>
<span data-ttu-id="b2acf-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2acf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b2acf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2acf-111">Permission type</span></span>      | <span data-ttu-id="b2acf-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b2acf-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2acf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2acf-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b2acf-114">User.Read, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b2acf-114">User.Read, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b2acf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2acf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2acf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2acf-116">Not supported.</span></span>    |
|<span data-ttu-id="b2acf-117">Application</span><span class="sxs-lookup"><span data-stu-id="b2acf-117">Application</span></span> | <span data-ttu-id="b2acf-118">User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2acf-118">User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2acf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2acf-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="b2acf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2acf-120">Request headers</span></span>
| <span data-ttu-id="b2acf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2acf-121">Header</span></span>       | <span data-ttu-id="b2acf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b2acf-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b2acf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2acf-123">Authorization</span></span>  | <span data-ttu-id="b2acf-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2acf-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b2acf-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b2acf-126">Content-Type</span></span>  | <span data-ttu-id="b2acf-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b2acf-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b2acf-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2acf-128">Request body</span></span>
<span data-ttu-id="b2acf-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2acf-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b2acf-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b2acf-130">Parameter</span></span>    | <span data-ttu-id="b2acf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2acf-131">Type</span></span>   |<span data-ttu-id="b2acf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2acf-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2acf-133">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="b2acf-133">securityEnabledOnly</span></span>|<span data-ttu-id="b2acf-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="b2acf-134">Boolean</span></span>|<span data-ttu-id="b2acf-p105">**true** para especificar que somente grupos de segurança dos quais o usuário é membro devem ser retornados; **false** para especificar que todos os grupos dos quais o usuário é membro devem ser retornados. Observação: Definir esse parâmetro como **true** é suportado apenas ao chamar este método em um usuário.</span><span class="sxs-lookup"><span data-stu-id="b2acf-p105">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="b2acf-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2acf-137">Response</span></span>

<span data-ttu-id="b2acf-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos e das funções de diretório dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="b2acf-138">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="b2acf-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2acf-139">Example</span></span>
<span data-ttu-id="b2acf-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b2acf-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b2acf-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2acf-141">Request</span></span>
<span data-ttu-id="b2acf-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2acf-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b2acf-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2acf-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="b2acf-144">C#</span><span class="sxs-lookup"><span data-stu-id="b2acf-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2acf-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2acf-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2acf-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2acf-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b2acf-147">Java</span><span class="sxs-lookup"><span data-stu-id="b2acf-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b2acf-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2acf-148">Response</span></span>
<span data-ttu-id="b2acf-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2acf-149">Here is an example of the response.</span></span> <span data-ttu-id="b2acf-150">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b2acf-150">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "user: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


