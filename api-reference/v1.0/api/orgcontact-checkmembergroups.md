---
title: 'orgContact: checkMemberGroups'
description: Verifique se há associação na lista de grupos especificada. Retorna da lista as identificações de grupo das quais o contato organizacional tem uma associação direta ou transitiva.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f72b0c51d5ea9f0eff824a85af41bf51ae429c10
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895955"
---
# <a name="orgcontact-checkmembergroups"></a><span data-ttu-id="04634-104">orgContact: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="04634-104">orgContact: checkMemberGroups</span></span>

<span data-ttu-id="04634-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04634-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="04634-106">Verifique se há associação na lista de grupos especificada.</span><span class="sxs-lookup"><span data-stu-id="04634-106">Check for membership in the specified list of groups.</span></span> <span data-ttu-id="04634-107">Retorna da lista as identificações de grupo das quais o [contato organizacional](../resources/orgcontact.md) tem uma associação direta ou transitiva.</span><span class="sxs-lookup"><span data-stu-id="04634-107">Returns from the list those group IDs of which the [organizational contact](../resources/orgcontact.md) has a direct or transitive membership.</span></span>

<span data-ttu-id="04634-108">Você pode verificar até um máximo de 20 grupos por solicitação.</span><span class="sxs-lookup"><span data-stu-id="04634-108">You can check up to a maximum of 20 groups per request.</span></span> <span data-ttu-id="04634-109">Essa função suporta o Microsoft 365 e outros tipos de grupos provisionados no Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="04634-109">This function supports Microsoft 365 and other types of groups provisioned in Azure Active Directory (Azure AD).</span></span>

>[!NOTE]
><span data-ttu-id="04634-110">Os grupos do Microsoft 365 não podem conter grupos.</span><span class="sxs-lookup"><span data-stu-id="04634-110">Microsoft 365 groups cannot contain groups.</span></span> <span data-ttu-id="04634-111">A associação a um grupo do Microsoft 365 é sempre direta.</span><span class="sxs-lookup"><span data-stu-id="04634-111">Membership in a Microsoft 365 group is always direct.</span></span>


## <a name="permissions"></a><span data-ttu-id="04634-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="04634-112">Permissions</span></span>
<span data-ttu-id="04634-113">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="04634-113">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="04634-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04634-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04634-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04634-115">Permission type</span></span>      | <span data-ttu-id="04634-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="04634-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04634-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04634-117">Delegated (work or school account)</span></span> | <span data-ttu-id="04634-118">OrgContact. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="04634-118">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |
|<span data-ttu-id="04634-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04634-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04634-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04634-120">Not supported.</span></span>    |
|<span data-ttu-id="04634-121">Application</span><span class="sxs-lookup"><span data-stu-id="04634-121">Application</span></span> | <span data-ttu-id="04634-122">OrgContact. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="04634-122">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04634-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04634-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="04634-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04634-124">Request headers</span></span>
| <span data-ttu-id="04634-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="04634-125">Header</span></span>       | <span data-ttu-id="04634-126">Valor</span><span class="sxs-lookup"><span data-stu-id="04634-126">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="04634-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="04634-127">Authorization</span></span>  | <span data-ttu-id="04634-128">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="04634-128">Bearer {token}.</span></span> <span data-ttu-id="04634-129">Required.</span><span class="sxs-lookup"><span data-stu-id="04634-129">Required.</span></span> |
| <span data-ttu-id="04634-130">Content-type</span><span class="sxs-lookup"><span data-stu-id="04634-130">Content-type</span></span>   | <span data-ttu-id="04634-131">application/json.</span><span class="sxs-lookup"><span data-stu-id="04634-131">application/json.</span></span> <span data-ttu-id="04634-132">Required.</span><span class="sxs-lookup"><span data-stu-id="04634-132">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04634-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04634-133">Request body</span></span>
<span data-ttu-id="04634-134">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04634-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="04634-135">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="04634-135">Parameter</span></span>    | <span data-ttu-id="04634-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="04634-136">Type</span></span>   |<span data-ttu-id="04634-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="04634-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04634-138">groupIds</span><span class="sxs-lookup"><span data-stu-id="04634-138">groupIds</span></span>|<span data-ttu-id="04634-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="04634-139">String collection</span></span> | <span data-ttu-id="04634-140">Uma lista de IDs de grupo para verificar.</span><span class="sxs-lookup"><span data-stu-id="04634-140">A list of group IDs to check.</span></span> |

## <a name="response"></a><span data-ttu-id="04634-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="04634-141">Response</span></span>

<span data-ttu-id="04634-142">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto da coleção String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04634-142">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04634-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04634-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="04634-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04634-144">Request</span></span>
<span data-ttu-id="04634-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="04634-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="04634-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="04634-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="04634-147">C#</span><span class="sxs-lookup"><span data-stu-id="04634-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04634-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04634-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04634-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04634-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="04634-150">Java</span><span class="sxs-lookup"><span data-stu-id="04634-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="04634-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="04634-151">Response</span></span>
<span data-ttu-id="04634-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="04634-152">The following is an example of the response.</span></span>
><span data-ttu-id="04634-153">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="04634-153">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
