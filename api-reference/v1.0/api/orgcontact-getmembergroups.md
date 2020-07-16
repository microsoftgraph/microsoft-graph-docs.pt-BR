---
title: 'orgContact: getMemberGroups'
description: Retornar todos os grupos dos quais o contato organizacional é membro.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 431f5e01f9e74f5c9c8d5adf9b9cc2ffa8473b04
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897180"
---
# <a name="orgcontact-getmembergroups"></a><span data-ttu-id="a64e4-103">orgContact: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="a64e4-103">orgContact: getMemberGroups</span></span>

<span data-ttu-id="a64e4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a64e4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a64e4-105">Retornar todos os grupos dos quais o [contato organizacional](../resources/orgcontact.md) é membro.</span><span class="sxs-lookup"><span data-stu-id="a64e4-105">Return all the groups that the [organizational contact](../resources/orgcontact.md) is a member of.</span></span> <span data-ttu-id="a64e4-106">A verificação é transitiva, diferentemente da leitura da propriedade de navegação **member**, que retorna somente os grupos dos quais o usuário é membro direto.</span><span class="sxs-lookup"><span data-stu-id="a64e4-106">The check is transitive, unlike reading the **memberOf** navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="a64e4-107">Essa função suporta o Microsoft 365 e outros tipos de grupos provisionados no Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="a64e4-107">This function supports Microsoft 365 and other types of groups provisioned in Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="a64e4-108">O número máximo de grupos que cada solicitação pode retornar é 2046.</span><span class="sxs-lookup"><span data-stu-id="a64e4-108">The maximum number of groups each request can return is 2046.</span></span> 

>[!NOTE]
><span data-ttu-id="a64e4-109">Os grupos do Microsoft 365 não podem conter grupos.</span><span class="sxs-lookup"><span data-stu-id="a64e4-109">Microsoft 365 groups cannot contain groups.</span></span> <span data-ttu-id="a64e4-110">A associação a um grupo do Microsoft 365 é sempre direta.</span><span class="sxs-lookup"><span data-stu-id="a64e4-110">Membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="a64e4-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="a64e4-111">Permissions</span></span>
<span data-ttu-id="a64e4-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a64e4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a64e4-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a64e4-114">Permission type</span></span>      | <span data-ttu-id="a64e4-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a64e4-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a64e4-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a64e4-116">Delegated (work or school account)</span></span> | <span data-ttu-id="a64e4-117">OrgContact. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="a64e4-117">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |
|<span data-ttu-id="a64e4-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a64e4-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a64e4-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a64e4-119">Not supported.</span></span>    |
|<span data-ttu-id="a64e4-120">Application</span><span class="sxs-lookup"><span data-stu-id="a64e4-120">Application</span></span> | <span data-ttu-id="a64e4-121">OrgContact. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="a64e4-121">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a64e4-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a64e4-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="a64e4-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a64e4-123">Request headers</span></span>
| <span data-ttu-id="a64e4-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a64e4-124">Header</span></span>       | <span data-ttu-id="a64e4-125">Valor</span><span class="sxs-lookup"><span data-stu-id="a64e4-125">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="a64e4-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="a64e4-126">Authorization</span></span>  |  <span data-ttu-id="a64e4-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a64e4-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a64e4-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="a64e4-129">Content-type</span></span>   | <span data-ttu-id="a64e4-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a64e4-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a64e4-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a64e4-132">Request body</span></span>
<span data-ttu-id="a64e4-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a64e4-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a64e4-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a64e4-134">Parameter</span></span>    | <span data-ttu-id="a64e4-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="a64e4-135">Type</span></span>   |<span data-ttu-id="a64e4-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="a64e4-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a64e4-137">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="a64e4-137">securityEnabledOnly</span></span>|<span data-ttu-id="a64e4-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="a64e4-138">Boolean</span></span>|<span data-ttu-id="a64e4-139">Definido como `false` .</span><span class="sxs-lookup"><span data-stu-id="a64e4-139">Set to `false`.</span></span> <span data-ttu-id="a64e4-140">Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="a64e4-140">Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="a64e4-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a64e4-141">Response</span></span>

<span data-ttu-id="a64e4-142">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto da coleção String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a64e4-142">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a64e4-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a64e4-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a64e4-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a64e4-144">Request</span></span>
<span data-ttu-id="a64e4-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a64e4-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a64e4-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="a64e4-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a64e4-147">C#</span><span class="sxs-lookup"><span data-stu-id="a64e4-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a64e4-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a64e4-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a64e4-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a64e4-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a64e4-150">Java</span><span class="sxs-lookup"><span data-stu-id="a64e4-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a64e4-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="a64e4-151">Response</span></span>
<span data-ttu-id="a64e4-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a64e4-152">The following is an example of the response.</span></span>
><span data-ttu-id="a64e4-153">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a64e4-153">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
