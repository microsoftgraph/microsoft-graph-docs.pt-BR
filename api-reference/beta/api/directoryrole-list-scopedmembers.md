---
title: Listar scopedMembers para uma função de diretório
description: Recupere uma lista de objetos scopedRoleMembership para uma função de diretório.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d5f915debcdecba1effdf96bae6ae36da0331783
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207691"
---
# <a name="list-scopedmembers-for-a-directory-role"></a><span data-ttu-id="8bb1f-103">Listar scopedMembers para uma função de diretório</span><span class="sxs-lookup"><span data-stu-id="8bb1f-103">List scopedMembers for a directory role</span></span>

<span data-ttu-id="8bb1f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bb1f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bb1f-105">Recupere uma lista de [objetos scopedRoleMembership](../resources/scopedrolemembership.md) para uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="8bb1f-105">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) objects for a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="8bb1f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8bb1f-106">Permissions</span></span>
<span data-ttu-id="8bb1f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bb1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bb1f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8bb1f-109">Permission type</span></span>      | <span data-ttu-id="8bb1f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8bb1f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8bb1f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8bb1f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8bb1f-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8bb1f-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8bb1f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8bb1f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bb1f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8bb1f-114">Not supported.</span></span>    |
|<span data-ttu-id="8bb1f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8bb1f-115">Application</span></span> | <span data-ttu-id="8bb1f-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bb1f-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bb1f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8bb1f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryroles/{role-id}/scopedMembers
GET /directoryroles/roleTemplateId={roleTemplateId}/scopedMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8bb1f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8bb1f-118">Optional query parameters</span></span>
<span data-ttu-id="8bb1f-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8bb1f-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8bb1f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8bb1f-120">Request headers</span></span>
| <span data-ttu-id="8bb1f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8bb1f-121">Name</span></span>      |<span data-ttu-id="8bb1f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bb1f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8bb1f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8bb1f-123">Authorization</span></span>  | <span data-ttu-id="8bb1f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8bb1f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8bb1f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8bb1f-126">Request body</span></span>
<span data-ttu-id="8bb1f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8bb1f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8bb1f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bb1f-128">Response</span></span>

<span data-ttu-id="8bb1f-129">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos scopedRoleMembership](../resources/scopedrolemembership.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8bb1f-129">If successful, this method returns a `200 OK` response code and a collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="8bb1f-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8bb1f-130">Examples</span></span>

### <a name="example-1--get-the-scoped-members-of-a-directory-role-using-role-id"></a><span data-ttu-id="8bb1f-131">Exemplo 1: Obter os membros com escopo de uma função de diretório usando a id de função</span><span class="sxs-lookup"><span data-stu-id="8bb1f-131">Example 1:  Get the scoped members of a directory role using role id</span></span>

#### <a name="request"></a><span data-ttu-id="8bb1f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8bb1f-132">Request</span></span>
<span data-ttu-id="8bb1f-133">A seguir está um exemplo de uma solicitação para uma **id** de função de `41d12a2f-caa8-4e3e-ba14-05e5102ce085` diretório.</span><span class="sxs-lookup"><span data-stu-id="8bb1f-133">The following is an example of a request for a directory role **id** `41d12a2f-caa8-4e3e-ba14-05e5102ce085`.</span></span>

# <a name="http"></a>[<span data-ttu-id="8bb1f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8bb1f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedmembers_directoryrole"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/41d12a2f-caa8-4e3e-ba14-05e5102ce085/scopedMembers
```
# <a name="c"></a>[<span data-ttu-id="8bb1f-135">C#</span><span class="sxs-lookup"><span data-stu-id="8bb1f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedmembers-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8bb1f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8bb1f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedmembers-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8bb1f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8bb1f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedmembers-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8bb1f-138">Java</span><span class="sxs-lookup"><span data-stu-id="8bb1f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedmembers-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8bb1f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bb1f-139">Response</span></span>
<span data-ttu-id="8bb1f-140">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="8bb1f-140">The following example shows the response.</span></span> 
><span data-ttu-id="8bb1f-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8bb1f-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#scopedRoleMemberships",
    "value": [
        {
            "id": "LyrRQajKPk66FAXlECzghXFuYtw3SOtAvkq8KdiKEXiTwZeOU-r8RIHrq2vQ4F1wU",
            "roleId": "41d12a2f-caa8-4e3e-ba14-05e5102ce085",
            "administrativeUnitId": "dc626e71-4837-40eb-be4a-bc29d88a1178",
            "roleMemberInfo": {
                "id": "8e97c193-ea53-44fc-81eb-ab6bd0e05d70",
                "displayName": "Adele Vance"
            }
        }
    ]
}
```

### <a name="example-2--get-the-scoped-members-of-a-directory-role-using-roletemplateid"></a><span data-ttu-id="8bb1f-142">Exemplo 2: Obter os membros com escopo de uma função de diretório usando roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="8bb1f-142">Example 2:  Get the scoped members of a directory role using roleTemplateId</span></span>

#### <a name="request"></a><span data-ttu-id="8bb1f-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8bb1f-143">Request</span></span>
<span data-ttu-id="8bb1f-144">A seguir está um exemplo de uma solicitação para uma função de diretório com **roleTemplateId** `fdd7a751-b60b-444a-984c-02652fe8fa1c` .</span><span class="sxs-lookup"><span data-stu-id="8bb1f-144">The following is an example of a request for a directory role with **roleTemplateId** `fdd7a751-b60b-444a-984c-02652fe8fa1c`.</span></span>


# <a name="http"></a>[<span data-ttu-id="8bb1f-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="8bb1f-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedmembers_directoryrole_templateId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/roleTemplateId=fdd7a751-b60b-444a-984c-02652fe8fa1c/scopedMembers
```
# <a name="c"></a>[<span data-ttu-id="8bb1f-146">C#</span><span class="sxs-lookup"><span data-stu-id="8bb1f-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedmembers-directoryrole-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8bb1f-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8bb1f-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedmembers-directoryrole-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8bb1f-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8bb1f-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedmembers-directoryrole-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8bb1f-149">Java</span><span class="sxs-lookup"><span data-stu-id="8bb1f-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedmembers-directoryrole-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8bb1f-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bb1f-150">Response</span></span>
<span data-ttu-id="8bb1f-151">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="8bb1f-151">The following example shows the response.</span></span> 
><span data-ttu-id="8bb1f-152">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8bb1f-152">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#scopedRoleMemberships",
    "value": [
        {
            "id": "LyrRQajKPk66FAXlECzghXFuYtw3SOtAvkq8KdiKEXiTwZeOU-r8RIHrq2vQ4F1wU",
            "roleId": "41d12a2f-caa8-4e3e-ba14-05e5102ce085",
            "administrativeUnitId": "dc626e71-4837-40eb-be4a-bc29d88a1178",
            "roleMemberInfo": {
                "id": "8e97c193-ea53-44fc-81eb-ab6bd0e05d70",
                "displayName": "Adele Vance"
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedmembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
