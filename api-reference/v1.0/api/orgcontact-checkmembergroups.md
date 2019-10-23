---
title: 'orgContact: checkMemberGroups'
description: Verifique se há associação na lista de grupos especificada. Retorna da lista as identificações de grupo das quais o contato organizacional tem uma associação direta ou transitiva.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5694a48cb4669bbf0c81b22d48c6e90eb90b7301
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37634020"
---
# <a name="orgcontact-checkmembergroups"></a><span data-ttu-id="52847-104">orgContact: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="52847-104">orgContact: checkMemberGroups</span></span>

<span data-ttu-id="52847-105">Verifique se há associação na lista de grupos especificada.</span><span class="sxs-lookup"><span data-stu-id="52847-105">Check for membership in the specified list of groups.</span></span> <span data-ttu-id="52847-106">Retorna da lista as identificações de grupo das quais o [contato organizacional](../resources/orgcontact.md) tem uma associação direta ou transitiva.</span><span class="sxs-lookup"><span data-stu-id="52847-106">Returns from the list those group IDs of which the [organizational contact](../resources/orgcontact.md) has a direct or transitive membership.</span></span>

<span data-ttu-id="52847-107">Você pode verificar até um máximo de 20 grupos por solicitação.</span><span class="sxs-lookup"><span data-stu-id="52847-107">You can check up to a maximum of 20 groups per request.</span></span> <span data-ttu-id="52847-108">Essa função suporta o Office 365 e outros tipos de grupos provisionados no Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="52847-108">This function supports Office 365 and other types of groups provisioned in Azure Active Directory (Azure AD).</span></span>

>[!NOTE]
><span data-ttu-id="52847-109">Os grupos do Office 365 não podem conter grupos.</span><span class="sxs-lookup"><span data-stu-id="52847-109">Office 365 groups cannot contain groups.</span></span> <span data-ttu-id="52847-110">A associação a um grupo do Office 365 é sempre direta.</span><span class="sxs-lookup"><span data-stu-id="52847-110">Membership in an Office 365 group is always direct.</span></span>


## <a name="permissions"></a><span data-ttu-id="52847-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="52847-111">Permissions</span></span>
<span data-ttu-id="52847-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52847-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52847-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52847-114">Permission type</span></span>      | <span data-ttu-id="52847-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52847-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52847-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52847-116">Delegated (work or school account)</span></span> | <span data-ttu-id="52847-117">OrgContact. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="52847-117">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |
|<span data-ttu-id="52847-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52847-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52847-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52847-119">Not supported.</span></span>    |
|<span data-ttu-id="52847-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52847-120">Application</span></span> | <span data-ttu-id="52847-121">OrgContact. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="52847-121">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="52847-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52847-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="52847-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52847-123">Request headers</span></span>
| <span data-ttu-id="52847-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="52847-124">Header</span></span>       | <span data-ttu-id="52847-125">Valor</span><span class="sxs-lookup"><span data-stu-id="52847-125">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="52847-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="52847-126">Authorization</span></span>  | <span data-ttu-id="52847-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52847-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="52847-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="52847-129">Content-type</span></span>   | <span data-ttu-id="52847-p107">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52847-p107">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52847-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52847-132">Request body</span></span>
<span data-ttu-id="52847-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52847-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="52847-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="52847-134">Parameter</span></span>    | <span data-ttu-id="52847-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="52847-135">Type</span></span>   |<span data-ttu-id="52847-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="52847-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52847-137">groupIds</span><span class="sxs-lookup"><span data-stu-id="52847-137">groupIds</span></span>|<span data-ttu-id="52847-138">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="52847-138">String collection</span></span> | <span data-ttu-id="52847-139">Uma lista de IDs de grupo para verificar.</span><span class="sxs-lookup"><span data-stu-id="52847-139">A list of group IDs to check.</span></span> |

## <a name="response"></a><span data-ttu-id="52847-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="52847-140">Response</span></span>

<span data-ttu-id="52847-141">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto da coleção String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52847-141">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52847-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52847-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="52847-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52847-143">Request</span></span>
<span data-ttu-id="52847-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="52847-144">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="52847-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="52847-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/contacts/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupId-value1", "groupId-value2" 
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="52847-146">C#</span><span class="sxs-lookup"><span data-stu-id="52847-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="52847-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52847-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="52847-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52847-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="52847-149">Java</span><span class="sxs-lookup"><span data-stu-id="52847-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="52847-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="52847-150">Response</span></span>
<span data-ttu-id="52847-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="52847-151">The following is an example of the response.</span></span>
><span data-ttu-id="52847-152">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="52847-152">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
    "groupId-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
