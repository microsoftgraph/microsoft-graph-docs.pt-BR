---
title: 'servicePrincipalName: getMemberGroups'
description: Obtenha a lista de grupos dos quais essa entidade de serviço é membro.  A verificação é transitiva.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: d9fd21012f4fe799b18ab07b85683b46ec012c8e
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219099"
---
# <a name="serviceprincipal-getmembergroups"></a><span data-ttu-id="668da-104">servicePrincipalName: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="668da-104">servicePrincipal: getMemberGroups</span></span>

<span data-ttu-id="668da-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="668da-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="668da-106">Obtenha a lista de grupos dos quais essa entidade de serviço é membro.</span><span class="sxs-lookup"><span data-stu-id="668da-106">Get the list of groups that this service principal is a member of.</span></span>  <span data-ttu-id="668da-107">A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="668da-107">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="668da-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="668da-108">Permissions</span></span>
<span data-ttu-id="668da-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="668da-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="668da-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="668da-111">Permission type</span></span>      | <span data-ttu-id="668da-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="668da-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="668da-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="668da-113">Delegated (work or school account)</span></span> | <span data-ttu-id="668da-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="668da-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="668da-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="668da-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="668da-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="668da-116">Not supported.</span></span>    |
|<span data-ttu-id="668da-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="668da-117">Application</span></span> | <span data-ttu-id="668da-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="668da-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="668da-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="668da-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="668da-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="668da-120">Request headers</span></span>
| <span data-ttu-id="668da-121">Nome</span><span class="sxs-lookup"><span data-stu-id="668da-121">Name</span></span>       | <span data-ttu-id="668da-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="668da-122">Type</span></span> | <span data-ttu-id="668da-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="668da-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="668da-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="668da-124">Authorization</span></span>  | <span data-ttu-id="668da-125">string</span><span class="sxs-lookup"><span data-stu-id="668da-125">string</span></span>  | <span data-ttu-id="668da-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="668da-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="668da-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="668da-128">Request body</span></span>
<span data-ttu-id="668da-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="668da-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="668da-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="668da-130">Parameter</span></span>    | <span data-ttu-id="668da-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="668da-131">Type</span></span>   |<span data-ttu-id="668da-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="668da-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="668da-133">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="668da-133">securityEnabledOnly</span></span>|<span data-ttu-id="668da-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="668da-134">Boolean</span></span>|<span data-ttu-id="668da-p105">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="668da-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="668da-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="668da-137">Response</span></span>

<span data-ttu-id="668da-138">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="668da-138">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="668da-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="668da-139">Example</span></span>
<span data-ttu-id="668da-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="668da-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="668da-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="668da-141">Request</span></span>
<span data-ttu-id="668da-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="668da-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="668da-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="668da-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="668da-144">C#</span><span class="sxs-lookup"><span data-stu-id="668da-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="668da-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="668da-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="668da-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="668da-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="668da-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="668da-147">Response</span></span>
<span data-ttu-id="668da-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="668da-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
