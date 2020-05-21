---
title: 'servicePrincipalName: getMemberObjects'
description: Obtenha a lista de grupos e funções de diretório dos quais essa entidade de serviço é membro.  Essa verificação é transitiva.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 255afc7d16c1f4f663043f44dbeeca9c657297c8
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333735"
---
# <a name="serviceprincipal-getmemberobjects"></a><span data-ttu-id="3c55b-104">servicePrincipalName: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="3c55b-104">servicePrincipal: getMemberObjects</span></span>

<span data-ttu-id="3c55b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c55b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c55b-106">Obtenha a lista de grupos e funções de diretório dos quais esse [servicePrincipalName](../resources/serviceprincipal.md) é um membro.</span><span class="sxs-lookup"><span data-stu-id="3c55b-106">Get the list of groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span>  <span data-ttu-id="3c55b-107">Essa verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="3c55b-107">This check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c55b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="3c55b-108">Permissions</span></span>
<span data-ttu-id="3c55b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c55b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c55b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c55b-111">Permission type</span></span>      | <span data-ttu-id="3c55b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3c55b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c55b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c55b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3c55b-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3c55b-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3c55b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c55b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c55b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c55b-116">Not supported.</span></span>    |
|<span data-ttu-id="3c55b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c55b-117">Application</span></span> | <span data-ttu-id="3c55b-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c55b-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c55b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c55b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="3c55b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c55b-120">Request headers</span></span>
| <span data-ttu-id="3c55b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3c55b-121">Name</span></span>       | <span data-ttu-id="3c55b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c55b-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="3c55b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c55b-123">Authorization</span></span> | <span data-ttu-id="3c55b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c55b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3c55b-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="3c55b-126">Content-type</span></span> | <span data-ttu-id="3c55b-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c55b-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c55b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c55b-129">Request body</span></span>
<span data-ttu-id="3c55b-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c55b-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3c55b-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3c55b-131">Parameter</span></span>    | <span data-ttu-id="3c55b-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c55b-132">Type</span></span>   |<span data-ttu-id="3c55b-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c55b-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c55b-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="3c55b-134">securityEnabledOnly</span></span>|<span data-ttu-id="3c55b-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="3c55b-135">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="3c55b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c55b-136">Response</span></span>

<span data-ttu-id="3c55b-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto da coleção String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c55b-137">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3c55b-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3c55b-138">Examples</span></span>
<span data-ttu-id="3c55b-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="3c55b-139">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="3c55b-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c55b-140">Request</span></span>
<span data-ttu-id="3c55b-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c55b-141">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3c55b-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c55b-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="3c55b-143">C#</span><span class="sxs-lookup"><span data-stu-id="3c55b-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c55b-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c55b-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c55b-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c55b-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3c55b-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c55b-146">Response</span></span>
<span data-ttu-id="3c55b-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c55b-147">Here is an example of the response.</span></span> 
><span data-ttu-id="3c55b-p106">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c55b-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "servicePrincipal: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
