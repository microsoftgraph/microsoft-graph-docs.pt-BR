---
title: 'orgContact: checkMemberGroups'
description: Verifique se há associação na lista de grupos especificada. Retorna da lista as IDs de grupo das quais o contato organizacional tem uma associação direta ou transitiva.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5bdafc5ecaf7e2f95017267bf35ff140994bfb1d
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761357"
---
# <a name="orgcontact-checkmembergroups"></a><span data-ttu-id="d4724-104">orgContact: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="d4724-104">orgContact: checkMemberGroups</span></span>

<span data-ttu-id="d4724-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4724-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d4724-106">Verifique se há associação na lista de grupos especificada.</span><span class="sxs-lookup"><span data-stu-id="d4724-106">Check for membership in the specified list of groups.</span></span> <span data-ttu-id="d4724-107">Retorna da lista as IDs de grupo das quais o contato [organizacional](../resources/orgcontact.md) tem uma associação direta ou transitiva.</span><span class="sxs-lookup"><span data-stu-id="d4724-107">Returns from the list those group IDs of which the [organizational contact](../resources/orgcontact.md) has a direct or transitive membership.</span></span>

<span data-ttu-id="d4724-108">Você pode fazer check-up de no máximo 20 grupos por solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4724-108">You can check up to a maximum of 20 groups per request.</span></span> <span data-ttu-id="d4724-109">Esta função dá suporte ao Microsoft 365 e a outros tipos de grupos provisionados no Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="d4724-109">This function supports Microsoft 365 and other types of groups provisioned in Azure Active Directory (Azure AD).</span></span>

>[!NOTE]
><span data-ttu-id="d4724-110">Os grupos do Microsoft 365 não podem conter grupos.</span><span class="sxs-lookup"><span data-stu-id="d4724-110">Microsoft 365 groups cannot contain groups.</span></span> <span data-ttu-id="d4724-111">A associação a um grupo do Microsoft 365 é sempre direta.</span><span class="sxs-lookup"><span data-stu-id="d4724-111">Membership in a Microsoft 365 group is always direct.</span></span>


## <a name="permissions"></a><span data-ttu-id="d4724-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="d4724-112">Permissions</span></span>
<span data-ttu-id="d4724-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4724-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4724-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4724-115">Permission type</span></span>      | <span data-ttu-id="d4724-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d4724-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4724-117">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4724-117">Delegated (work or school account)</span></span> | <span data-ttu-id="d4724-118">OrgContact.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4724-118">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |
|<span data-ttu-id="d4724-119">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4724-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4724-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4724-120">Not supported.</span></span>    |
|<span data-ttu-id="d4724-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4724-121">Application</span></span> | <span data-ttu-id="d4724-122">OrgContact.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4724-122">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4724-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4724-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="d4724-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4724-124">Request headers</span></span>
| <span data-ttu-id="d4724-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d4724-125">Header</span></span>       | <span data-ttu-id="d4724-126">Valor</span><span class="sxs-lookup"><span data-stu-id="d4724-126">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="d4724-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4724-127">Authorization</span></span>  | <span data-ttu-id="d4724-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4724-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d4724-130">Content-type</span><span class="sxs-lookup"><span data-stu-id="d4724-130">Content-type</span></span>   | <span data-ttu-id="d4724-p107">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4724-p107">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4724-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4724-133">Request body</span></span>
<span data-ttu-id="d4724-134">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4724-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d4724-135">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d4724-135">Parameter</span></span>    | <span data-ttu-id="d4724-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4724-136">Type</span></span>   |<span data-ttu-id="d4724-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4724-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4724-138">groupIds</span><span class="sxs-lookup"><span data-stu-id="d4724-138">groupIds</span></span>|<span data-ttu-id="d4724-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4724-139">String collection</span></span> | <span data-ttu-id="d4724-140">Uma lista de IDs de grupo a verificar.</span><span class="sxs-lookup"><span data-stu-id="d4724-140">A list of group IDs to check.</span></span> |

## <a name="response"></a><span data-ttu-id="d4724-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4724-141">Response</span></span>

<span data-ttu-id="d4724-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4724-142">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4724-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4724-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d4724-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4724-144">Request</span></span>
<span data-ttu-id="d4724-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4724-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d4724-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4724-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d4724-147">C#</span><span class="sxs-lookup"><span data-stu-id="d4724-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d4724-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4724-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4724-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4724-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d4724-150">Java</span><span class="sxs-lookup"><span data-stu-id="d4724-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d4724-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4724-151">Response</span></span>
<span data-ttu-id="d4724-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d4724-152">The following is an example of the response.</span></span>
><span data-ttu-id="d4724-153">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d4724-153">**Note**: The response object shown here might be shortened for readability.</span></span> 
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

