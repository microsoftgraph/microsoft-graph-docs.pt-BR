---
title: 'user: getMemberObjects'
description: Retorna todos os grupos e funções de diretório e unidades administrativas dos quais o usuário é membro. A verificação é transitiva.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4ff151a55d5fa3cba05c34f0dfaf3827fca52371
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457811"
---
# <a name="user-getmemberobjects"></a><span data-ttu-id="9434f-104">user: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="9434f-104">user: getMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9434f-p102">Retorna todos os grupos e funções de diretório e unidades administrativas dos quais o usuário é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="9434f-p102">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="9434f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9434f-107">Permissions</span></span>
<span data-ttu-id="9434f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9434f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9434f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9434f-110">Permission type</span></span>      | <span data-ttu-id="9434f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9434f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9434f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9434f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9434f-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9434f-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9434f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9434f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9434f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9434f-115">Not supported.</span></span>    |
|<span data-ttu-id="9434f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9434f-116">Application</span></span> | <span data-ttu-id="9434f-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9434f-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9434f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9434f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="9434f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9434f-119">Request headers</span></span>
| <span data-ttu-id="9434f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9434f-120">Header</span></span>       | <span data-ttu-id="9434f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9434f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9434f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9434f-122">Authorization</span></span>  | <span data-ttu-id="9434f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9434f-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9434f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9434f-125">Content-Type</span></span>  | <span data-ttu-id="9434f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9434f-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9434f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9434f-127">Request body</span></span>
<span data-ttu-id="9434f-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9434f-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9434f-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9434f-129">Parameter</span></span>    | <span data-ttu-id="9434f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9434f-130">Type</span></span>   |<span data-ttu-id="9434f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9434f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9434f-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="9434f-132">securityEnabledOnly</span></span>|<span data-ttu-id="9434f-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="9434f-133">Boolean</span></span>|<span data-ttu-id="9434f-p105">**true** para especificar que somente grupos de segurança dos quais o usuário é membro devem ser retornados; **false** para especificar que todos os grupos dos quais o usuário é membro devem ser retornados. Observação: Definir esse parâmetro como **true** é suportado apenas ao chamar este método em um usuário.</span><span class="sxs-lookup"><span data-stu-id="9434f-p105">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="9434f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9434f-136">Response</span></span>

<span data-ttu-id="9434f-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos e das funções de diretório dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="9434f-137">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="9434f-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9434f-138">Example</span></span>
<span data-ttu-id="9434f-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="9434f-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9434f-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9434f-140">Request</span></span>
<span data-ttu-id="9434f-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9434f-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9434f-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="9434f-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="9434f-143">C#</span><span class="sxs-lookup"><span data-stu-id="9434f-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9434f-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="9434f-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9434f-145">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9434f-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9434f-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="9434f-146">Response</span></span>
<span data-ttu-id="9434f-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9434f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
