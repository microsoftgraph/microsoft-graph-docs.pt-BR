---
title: 'orgContact: getMemberGroups'
description: Retorne todos os grupos dos que o contato organizacional é membro.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 7fc8f9a62656cace7a4dd3e02182a8a2bc454464
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761643"
---
# <a name="orgcontact-getmembergroups"></a><span data-ttu-id="c9291-103">orgContact: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="c9291-103">orgContact: getMemberGroups</span></span>

<span data-ttu-id="c9291-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9291-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c9291-105">Retorne todos os grupos dos que o [contato organizacional](../resources/orgcontact.md) é membro.</span><span class="sxs-lookup"><span data-stu-id="c9291-105">Return all the groups that the [organizational contact](../resources/orgcontact.md) is a member of.</span></span> <span data-ttu-id="c9291-106">A verificação é transitiva, diferentemente da leitura da propriedade de navegação **member**, que retorna somente os grupos dos quais o usuário é membro direto.</span><span class="sxs-lookup"><span data-stu-id="c9291-106">The check is transitive, unlike reading the **memberOf** navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="c9291-107">Esta função dá suporte ao Microsoft 365 e a outros tipos de grupos provisionados no Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="c9291-107">This function supports Microsoft 365 and other types of groups provisioned in Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="c9291-108">O número máximo de grupos que cada solicitação pode retornar é 2046.</span><span class="sxs-lookup"><span data-stu-id="c9291-108">The maximum number of groups each request can return is 2046.</span></span> 

>[!NOTE]
><span data-ttu-id="c9291-109">Os grupos do Microsoft 365 não podem conter grupos.</span><span class="sxs-lookup"><span data-stu-id="c9291-109">Microsoft 365 groups cannot contain groups.</span></span> <span data-ttu-id="c9291-110">A associação a um grupo do Microsoft 365 é sempre direta.</span><span class="sxs-lookup"><span data-stu-id="c9291-110">Membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9291-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="c9291-111">Permissions</span></span>
<span data-ttu-id="c9291-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9291-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9291-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9291-114">Permission type</span></span>      | <span data-ttu-id="c9291-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c9291-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9291-116">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9291-116">Delegated (work or school account)</span></span> | <span data-ttu-id="c9291-117">OrgContact.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9291-117">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |
|<span data-ttu-id="c9291-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9291-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9291-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9291-119">Not supported.</span></span>    |
|<span data-ttu-id="c9291-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9291-120">Application</span></span> | <span data-ttu-id="c9291-121">OrgContact.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9291-121">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9291-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9291-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="c9291-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9291-123">Request headers</span></span>
| <span data-ttu-id="c9291-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c9291-124">Header</span></span>       | <span data-ttu-id="c9291-125">Valor</span><span class="sxs-lookup"><span data-stu-id="c9291-125">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="c9291-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9291-126">Authorization</span></span>  |  <span data-ttu-id="c9291-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9291-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c9291-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="c9291-129">Content-type</span></span>   | <span data-ttu-id="c9291-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9291-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9291-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9291-132">Request body</span></span>
<span data-ttu-id="c9291-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9291-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c9291-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c9291-134">Parameter</span></span>    | <span data-ttu-id="c9291-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9291-135">Type</span></span>   |<span data-ttu-id="c9291-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9291-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9291-137">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="c9291-137">securityEnabledOnly</span></span>|<span data-ttu-id="c9291-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="c9291-138">Boolean</span></span>|<span data-ttu-id="c9291-139">Definir como `false` .</span><span class="sxs-lookup"><span data-stu-id="c9291-139">Set to `false`.</span></span> <span data-ttu-id="c9291-140">Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="c9291-140">Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="c9291-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9291-141">Response</span></span>

<span data-ttu-id="c9291-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9291-142">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9291-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c9291-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c9291-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9291-144">Request</span></span>
<span data-ttu-id="c9291-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9291-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c9291-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9291-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/contacts/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```
# <a name="c"></a>[<span data-ttu-id="c9291-147">C#</span><span class="sxs-lookup"><span data-stu-id="c9291-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9291-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9291-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9291-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9291-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c9291-150">Java</span><span class="sxs-lookup"><span data-stu-id="c9291-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c9291-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9291-151">Response</span></span>
<span data-ttu-id="c9291-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c9291-152">The following is an example of the response.</span></span>
><span data-ttu-id="c9291-153">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c9291-153">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
    "groupId-value1",
    "groupId-value2"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

