---
title: 'servicePrincipalName: getMemberGroups'
description: Obtenha a lista de grupos dos quais essa entidade de serviço é membro.  A verificação é transitiva.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 40fa4162a5aea180507c0cbc04bbe095de466f3e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453461"
---
# <a name="serviceprincipal-getmembergroups"></a><span data-ttu-id="80d34-104">servicePrincipalName: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="80d34-104">servicePrincipal: getMemberGroups</span></span>

<span data-ttu-id="80d34-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="80d34-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80d34-106">Obtenha a lista de grupos dos quais essa entidade de serviço é membro.</span><span class="sxs-lookup"><span data-stu-id="80d34-106">Get the list of groups that this service principal is a member of.</span></span>  <span data-ttu-id="80d34-107">A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="80d34-107">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="80d34-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="80d34-108">Permissions</span></span>
<span data-ttu-id="80d34-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80d34-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="80d34-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80d34-111">Permission type</span></span>      | <span data-ttu-id="80d34-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="80d34-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80d34-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80d34-113">Delegated (work or school account)</span></span> | <span data-ttu-id="80d34-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="80d34-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="80d34-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80d34-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80d34-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80d34-116">Not supported.</span></span>    |
|<span data-ttu-id="80d34-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80d34-117">Application</span></span> | <span data-ttu-id="80d34-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80d34-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="80d34-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80d34-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="80d34-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80d34-120">Request headers</span></span>
| <span data-ttu-id="80d34-121">Nome</span><span class="sxs-lookup"><span data-stu-id="80d34-121">Name</span></span>       | <span data-ttu-id="80d34-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="80d34-122">Type</span></span> | <span data-ttu-id="80d34-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="80d34-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="80d34-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="80d34-124">Authorization</span></span>  | <span data-ttu-id="80d34-125">string</span><span class="sxs-lookup"><span data-stu-id="80d34-125">string</span></span>  | <span data-ttu-id="80d34-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80d34-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80d34-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80d34-128">Request body</span></span>
<span data-ttu-id="80d34-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="80d34-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="80d34-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="80d34-130">Parameter</span></span>    | <span data-ttu-id="80d34-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="80d34-131">Type</span></span>   |<span data-ttu-id="80d34-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="80d34-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80d34-133">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="80d34-133">securityEnabledOnly</span></span>|<span data-ttu-id="80d34-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="80d34-134">Boolean</span></span>|<span data-ttu-id="80d34-p105">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="80d34-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="80d34-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="80d34-137">Response</span></span>

<span data-ttu-id="80d34-138">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80d34-138">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80d34-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80d34-139">Example</span></span>
<span data-ttu-id="80d34-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="80d34-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="80d34-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80d34-141">Request</span></span>
<span data-ttu-id="80d34-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="80d34-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="80d34-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="80d34-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="80d34-144">C#</span><span class="sxs-lookup"><span data-stu-id="80d34-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="80d34-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80d34-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80d34-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80d34-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="80d34-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="80d34-147">Response</span></span>
<span data-ttu-id="80d34-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80d34-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "servicePrincipal: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
