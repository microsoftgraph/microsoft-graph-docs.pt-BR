---
title: 'servicePrincipal: getMemberObjects'
description: Obtenha a lista de grupos dos quais essa entidade de serviço é membro.  A verificação é transitiva.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 66298b90fb794fc4453de5b983b1213a8486cc23
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134446"
---
# <a name="serviceprincipal-getmembergroups"></a><span data-ttu-id="56c5d-104">servicePrincipal: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="56c5d-104">servicePrincipal: getMemberGroups</span></span>

<span data-ttu-id="56c5d-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56c5d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56c5d-106">Obtenha a lista de grupos dos quais [servicePrincipal](../resources/serviceprincipal.md) é membro.</span><span class="sxs-lookup"><span data-stu-id="56c5d-106">Get the list of groups that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span>  <span data-ttu-id="56c5d-107">A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="56c5d-107">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="56c5d-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="56c5d-108">Permissions</span></span>
<span data-ttu-id="56c5d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56c5d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="56c5d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56c5d-111">Permission type</span></span>      | <span data-ttu-id="56c5d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56c5d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56c5d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56c5d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="56c5d-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="56c5d-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="56c5d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56c5d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56c5d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56c5d-116">Not supported.</span></span>    |
|<span data-ttu-id="56c5d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56c5d-117">Application</span></span> | <span data-ttu-id="56c5d-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56c5d-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="56c5d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56c5d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="56c5d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56c5d-120">Request headers</span></span>
| <span data-ttu-id="56c5d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="56c5d-121">Name</span></span>       | <span data-ttu-id="56c5d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="56c5d-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="56c5d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="56c5d-123">Authorization</span></span> | <span data-ttu-id="56c5d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56c5d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="56c5d-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="56c5d-126">Content-type</span></span> | <span data-ttu-id="56c5d-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56c5d-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56c5d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56c5d-129">Request body</span></span>
<span data-ttu-id="56c5d-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56c5d-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="56c5d-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="56c5d-131">Parameter</span></span>    | <span data-ttu-id="56c5d-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="56c5d-132">Type</span></span>   |<span data-ttu-id="56c5d-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="56c5d-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56c5d-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="56c5d-134">securityEnabledOnly</span></span>|<span data-ttu-id="56c5d-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="56c5d-135">Boolean</span></span>|<span data-ttu-id="56c5d-p106">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="56c5d-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="56c5d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="56c5d-138">Response</span></span>

<span data-ttu-id="56c5d-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56c5d-139">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="56c5d-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="56c5d-140">Examples</span></span>
<span data-ttu-id="56c5d-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="56c5d-141">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="56c5d-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56c5d-142">Request</span></span>
<span data-ttu-id="56c5d-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56c5d-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="56c5d-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="56c5d-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="56c5d-145">C#</span><span class="sxs-lookup"><span data-stu-id="56c5d-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56c5d-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56c5d-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56c5d-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56c5d-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="56c5d-148">Java</span><span class="sxs-lookup"><span data-stu-id="56c5d-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="56c5d-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="56c5d-149">Response</span></span>
<span data-ttu-id="56c5d-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56c5d-150">Here is an example of the response.</span></span> 
><span data-ttu-id="56c5d-p107">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56c5d-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



