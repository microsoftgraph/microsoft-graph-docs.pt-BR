---
title: 'orgContact: getMemberGroups'
description: Retornar todos os grupos dos quais o contato organizacional é membro.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bfff689d075fc874c3ce31b2992cf90286af3049
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37633965"
---
# <a name="orgcontact-getmembergroups"></a><span data-ttu-id="5f92d-103">orgContact: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="5f92d-103">orgContact: getMemberGroups</span></span>

<span data-ttu-id="5f92d-104">Retornar todos os grupos dos quais o [contato organizacional](../resources/orgcontact.md) é membro.</span><span class="sxs-lookup"><span data-stu-id="5f92d-104">Return all the groups that the [organizational contact](../resources/orgcontact.md) is a member of.</span></span> <span data-ttu-id="5f92d-105">A verificação é transitiva, diferentemente da leitura da propriedade de navegação **member**, que retorna somente os grupos dos quais o usuário é membro direto.</span><span class="sxs-lookup"><span data-stu-id="5f92d-105">The check is transitive, unlike reading the **memberOf** navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="5f92d-106">Essa função suporta o Office 365 e outros tipos de grupos provisionados no Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="5f92d-106">This function supports Office 365 and other types of groups provisioned in Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="5f92d-107">O número máximo de grupos que cada solicitação pode retornar é 2046.</span><span class="sxs-lookup"><span data-stu-id="5f92d-107">The maximum number of groups each request can return is 2046.</span></span> 

>[!NOTE]
><span data-ttu-id="5f92d-108">Os grupos do Office 365 não podem conter grupos.</span><span class="sxs-lookup"><span data-stu-id="5f92d-108">Office 365 groups cannot contain groups.</span></span> <span data-ttu-id="5f92d-109">A associação a um grupo do Office 365 é sempre direta.</span><span class="sxs-lookup"><span data-stu-id="5f92d-109">Membership in an Office 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f92d-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="5f92d-110">Permissions</span></span>
<span data-ttu-id="5f92d-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f92d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f92d-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f92d-113">Permission type</span></span>      | <span data-ttu-id="5f92d-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5f92d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f92d-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f92d-115">Delegated (work or school account)</span></span> | <span data-ttu-id="5f92d-116">OrgContact. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="5f92d-116">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |
|<span data-ttu-id="5f92d-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f92d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f92d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f92d-118">Not supported.</span></span>    |
|<span data-ttu-id="5f92d-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f92d-119">Application</span></span> | <span data-ttu-id="5f92d-120">OrgContact. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="5f92d-120">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f92d-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f92d-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="5f92d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f92d-122">Request headers</span></span>
| <span data-ttu-id="5f92d-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5f92d-123">Header</span></span>       | <span data-ttu-id="5f92d-124">Valor</span><span class="sxs-lookup"><span data-stu-id="5f92d-124">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="5f92d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f92d-125">Authorization</span></span>  |  <span data-ttu-id="5f92d-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f92d-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5f92d-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="5f92d-128">Content-type</span></span>   | <span data-ttu-id="5f92d-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f92d-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f92d-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f92d-131">Request body</span></span>
<span data-ttu-id="5f92d-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f92d-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5f92d-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5f92d-133">Parameter</span></span>    | <span data-ttu-id="5f92d-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f92d-134">Type</span></span>   |<span data-ttu-id="5f92d-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f92d-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f92d-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="5f92d-136">securityEnabledOnly</span></span>|<span data-ttu-id="5f92d-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="5f92d-137">Boolean</span></span>|<span data-ttu-id="5f92d-138">Definido como `false`.</span><span class="sxs-lookup"><span data-stu-id="5f92d-138">Set to `false`.</span></span> <span data-ttu-id="5f92d-139">Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="5f92d-139">Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="5f92d-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f92d-140">Response</span></span>

<span data-ttu-id="5f92d-141">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto da coleção String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f92d-141">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f92d-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f92d-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5f92d-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f92d-143">Request</span></span>
<span data-ttu-id="5f92d-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f92d-144">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5f92d-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f92d-145">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="5f92d-146">C#</span><span class="sxs-lookup"><span data-stu-id="5f92d-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5f92d-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f92d-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5f92d-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f92d-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5f92d-149">Java</span><span class="sxs-lookup"><span data-stu-id="5f92d-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5f92d-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f92d-150">Response</span></span>
<span data-ttu-id="5f92d-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5f92d-151">The following is an example of the response.</span></span>
><span data-ttu-id="5f92d-152">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5f92d-152">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
