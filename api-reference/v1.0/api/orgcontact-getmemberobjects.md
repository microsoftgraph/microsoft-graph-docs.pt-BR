---
title: 'orgContact: getMemberObjects'
description: Retorne todos os grupos dos quais este contato organizacional é membro. A verificação é transitiva.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bbc577fe998d64a182051815124d364e9d3a7872
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37633926"
---
# <a name="orgcontact-getmemberobjects"></a><span data-ttu-id="d2b72-104">orgContact: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="d2b72-104">orgContact: getMemberObjects</span></span>

<span data-ttu-id="d2b72-105">Retorne todos os grupos dos quais este [contato organizacional](../resources/orgcontact.md) é membro.</span><span class="sxs-lookup"><span data-stu-id="d2b72-105">Return all the groups that this [organizational contact](../resources/orgcontact.md) is a member of.</span></span> <span data-ttu-id="d2b72-106">A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="d2b72-106">The check is transitive.</span></span> <span data-ttu-id="d2b72-107">Contatos organizacionais não podem ser membros de funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="d2b72-107">Organizational contacts cannot be members of directory roles.</span></span> <span data-ttu-id="d2b72-108">Nenhuma função de diretório será retornada.</span><span class="sxs-lookup"><span data-stu-id="d2b72-108">No directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2b72-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="d2b72-109">Permissions</span></span>
<span data-ttu-id="d2b72-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2b72-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2b72-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2b72-112">Permission type</span></span>      | <span data-ttu-id="d2b72-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2b72-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2b72-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2b72-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d2b72-115">OrgContact. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="d2b72-115">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="d2b72-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2b72-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2b72-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2b72-117">Not supported.</span></span>    |
|<span data-ttu-id="d2b72-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2b72-118">Application</span></span> | <span data-ttu-id="d2b72-119">OrgContact. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="d2b72-119">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2b72-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2b72-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="d2b72-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2b72-121">Request headers</span></span>
| <span data-ttu-id="d2b72-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d2b72-122">Header</span></span>       | <span data-ttu-id="d2b72-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d2b72-123">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="d2b72-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2b72-124">Authorization</span></span>  | <span data-ttu-id="d2b72-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2b72-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d2b72-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="d2b72-127">Content-type</span></span>   | <span data-ttu-id="d2b72-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2b72-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2b72-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2b72-130">Request body</span></span>
<span data-ttu-id="d2b72-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2b72-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d2b72-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d2b72-132">Parameter</span></span>    | <span data-ttu-id="d2b72-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2b72-133">Type</span></span>   |<span data-ttu-id="d2b72-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2b72-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2b72-135">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="d2b72-135">securityEnabledOnly</span></span>|<span data-ttu-id="d2b72-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="d2b72-136">Boolean</span></span>|<span data-ttu-id="d2b72-137">Definido como `false`.</span><span class="sxs-lookup"><span data-stu-id="d2b72-137">Set to `false`.</span></span> <span data-ttu-id="d2b72-138">Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="d2b72-138">Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="d2b72-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2b72-139">Response</span></span>

<span data-ttu-id="d2b72-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto da coleção String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2b72-140">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2b72-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2b72-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d2b72-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2b72-142">Request</span></span>
<span data-ttu-id="d2b72-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2b72-143">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d2b72-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2b72-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/contacts/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d2b72-145">C#</span><span class="sxs-lookup"><span data-stu-id="d2b72-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d2b72-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2b72-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d2b72-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2b72-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d2b72-148">Java</span><span class="sxs-lookup"><span data-stu-id="d2b72-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d2b72-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2b72-149">Response</span></span>
<span data-ttu-id="d2b72-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d2b72-150">The following is an example of the response.</span></span>
><span data-ttu-id="d2b72-151">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d2b72-151">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
    "groupID-value1"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
