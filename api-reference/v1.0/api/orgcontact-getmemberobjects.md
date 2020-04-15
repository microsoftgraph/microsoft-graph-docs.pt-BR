---
title: 'orgContact: getMemberObjects'
description: Retorne todos os grupos dos quais este contato organizacional é membro. A verificação é transitiva.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2d3f283eaaaed217596c8cdaa200b3bc0a1c2f06
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451684"
---
# <a name="orgcontact-getmemberobjects"></a><span data-ttu-id="2eb87-104">orgContact: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="2eb87-104">orgContact: getMemberObjects</span></span>

<span data-ttu-id="2eb87-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2eb87-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2eb87-106">Retorne todos os grupos dos quais este [contato organizacional](../resources/orgcontact.md) é membro.</span><span class="sxs-lookup"><span data-stu-id="2eb87-106">Return all the groups that this [organizational contact](../resources/orgcontact.md) is a member of.</span></span> <span data-ttu-id="2eb87-107">A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="2eb87-107">The check is transitive.</span></span> <span data-ttu-id="2eb87-108">Contatos organizacionais não podem ser membros de funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="2eb87-108">Organizational contacts cannot be members of directory roles.</span></span> <span data-ttu-id="2eb87-109">Nenhuma função de diretório será retornada.</span><span class="sxs-lookup"><span data-stu-id="2eb87-109">No directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="2eb87-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="2eb87-110">Permissions</span></span>
<span data-ttu-id="2eb87-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2eb87-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2eb87-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2eb87-113">Permission type</span></span>      | <span data-ttu-id="2eb87-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2eb87-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2eb87-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2eb87-115">Delegated (work or school account)</span></span> | <span data-ttu-id="2eb87-116">OrgContact. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="2eb87-116">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="2eb87-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2eb87-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2eb87-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2eb87-118">Not supported.</span></span>    |
|<span data-ttu-id="2eb87-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2eb87-119">Application</span></span> | <span data-ttu-id="2eb87-120">OrgContact. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="2eb87-120">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2eb87-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2eb87-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="2eb87-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2eb87-122">Request headers</span></span>
| <span data-ttu-id="2eb87-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2eb87-123">Header</span></span>       | <span data-ttu-id="2eb87-124">Valor</span><span class="sxs-lookup"><span data-stu-id="2eb87-124">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="2eb87-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="2eb87-125">Authorization</span></span>  | <span data-ttu-id="2eb87-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2eb87-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2eb87-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="2eb87-128">Content-type</span></span>   | <span data-ttu-id="2eb87-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2eb87-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2eb87-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2eb87-131">Request body</span></span>
<span data-ttu-id="2eb87-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2eb87-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2eb87-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2eb87-133">Parameter</span></span>    | <span data-ttu-id="2eb87-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="2eb87-134">Type</span></span>   |<span data-ttu-id="2eb87-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="2eb87-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2eb87-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="2eb87-136">securityEnabledOnly</span></span>|<span data-ttu-id="2eb87-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="2eb87-137">Boolean</span></span>|<span data-ttu-id="2eb87-138">Definido como `false`.</span><span class="sxs-lookup"><span data-stu-id="2eb87-138">Set to `false`.</span></span> <span data-ttu-id="2eb87-139">Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="2eb87-139">Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="2eb87-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="2eb87-140">Response</span></span>

<span data-ttu-id="2eb87-141">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto da coleção String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2eb87-141">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2eb87-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2eb87-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2eb87-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2eb87-143">Request</span></span>
<span data-ttu-id="2eb87-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2eb87-144">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2eb87-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="2eb87-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2eb87-146">C#</span><span class="sxs-lookup"><span data-stu-id="2eb87-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2eb87-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2eb87-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2eb87-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2eb87-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2eb87-149">Java</span><span class="sxs-lookup"><span data-stu-id="2eb87-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2eb87-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="2eb87-150">Response</span></span>
<span data-ttu-id="2eb87-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2eb87-151">The following is an example of the response.</span></span>
><span data-ttu-id="2eb87-152">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2eb87-152">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
