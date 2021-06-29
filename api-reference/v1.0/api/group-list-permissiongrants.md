---
title: Listar permissionGrants de um grupo
description: Recuperar permissionGrants de um grupo.
author: akjo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1f0b26b455a004192c329bf26804631c13fed1ce
ms.sourcegitcommit: b5fbb1a715e3479bdd095ef00deb0c932eafc328
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2021
ms.locfileid: "53162179"
---
# <a name="list-permissiongrants-of-a-group"></a><span data-ttu-id="a078c-103">Listar permissionGrants de um grupo</span><span class="sxs-lookup"><span data-stu-id="a078c-103">List permissionGrants of a group</span></span>

<span data-ttu-id="a078c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a078c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a078c-p101">Listar todas [concessões de permissão específicas de recursos](../resources/resourcespecificpermissiongrant.md) no [grupo](../resources/group.md). Esta lista especifica os aplicativos Microsoft Azure Active Directory que têm acesso ao **grupo**, junto com o tipo correspondente de acesso específico de recursos que cada aplicativo tem.</span><span class="sxs-lookup"><span data-stu-id="a078c-p101">List all [resource-specific permission grants](../resources/resourcespecificpermissiongrant.md) on the [group](../resources/group.md). This list specifies the Azure AD apps that have access to the **group**, along with the corresponding kind of resource-specific access that each app has.</span></span>

## <a name="permissions"></a><span data-ttu-id="a078c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a078c-107">Permissions</span></span>

<span data-ttu-id="a078c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a078c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a078c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a078c-110">Permission Type</span></span>                        | <span data-ttu-id="a078c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a078c-111">Permissions (from least to most privileged)</span></span>                                          |
| :------------------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="a078c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a078c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a078c-113">GroupMember.Read.All, GroupMember.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a078c-113">GroupMember.Read.All, GroupMember.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="a078c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a078c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a078c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a078c-115">Not supported.</span></span>                                                                       |
| <span data-ttu-id="a078c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a078c-116">Application</span></span>                            | <span data-ttu-id="a078c-117">GroupMember.Read.All, GroupMember.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a078c-117">GroupMember.Read.All, GroupMember.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a078c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a078c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{group-id}/permissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a078c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a078c-119">Optional query parameters</span></span>

<span data-ttu-id="a078c-120">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a078c-120">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a078c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a078c-121">Request headers</span></span>

| <span data-ttu-id="a078c-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a078c-122">Header</span></span>           | <span data-ttu-id="a078c-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a078c-123">Value</span></span>                      |
| :--------------- | :------------------------- |
| <span data-ttu-id="a078c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a078c-124">Authorization</span></span>    | <span data-ttu-id="a078c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a078c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a078c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a078c-127">Request body</span></span>

<span data-ttu-id="a078c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a078c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a078c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a078c-129">Response</span></span>

<span data-ttu-id="a078c-130">Se for bem-sucedido, este método retorna um `200 OK` código de resposta e uma lista de [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) objetos no corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a078c-130">If successful, this method returns a `200 OK` response code and a list of [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a078c-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a078c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a078c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a078c-132">Request</span></span>

<span data-ttu-id="a078c-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a078c-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a078c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a078c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_list_permission_grants"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/14c981a4-dca9-4565-bae6-e13ada8861be/permissionGrants
```
# <a name="c"></a>[<span data-ttu-id="a078c-135">C#</span><span class="sxs-lookup"><span data-stu-id="a078c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-list-permission-grants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a078c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a078c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-list-permission-grants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a078c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a078c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-list-permission-grants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a078c-138">Java</span><span class="sxs-lookup"><span data-stu-id="a078c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-list-permission-grants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a078c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a078c-139">Response</span></span>

<span data-ttu-id="a078c-140">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="a078c-140">The following example shows the response.</span></span>

><span data-ttu-id="a078c-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a078c-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.resourceSpecificPermissionGrant"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#permissionGrants",
    "value": [
        {
            "id": "ZfwbxSIj9OGOBxsBmwY555mOHr_W6qN7LEbFYIIcM5A",
            "deletedDateTime": null,
            "clientId": "771b9da9-2260-41eb-a587-4d936e4aa08c",
            "clientAppId": "fdebf36e-8b3a-4b00-99fb-2e4d1da706d6",
            "resourceAppId": "00000003-0000-0000-c000-000000000000",
            "permissionType": "Application",
            "permission": "TeamMember.Read.Group"
        },
        {
            "id": "WsYCHhlwjliiK19ONpJiWq6rtFy-Tg1q8h9-f-DATto",
            "deletedDateTime": null,
            "clientId": "771b9da9-2260-41eb-a587-4d936e4aa08c",
            "clientAppId": "fdebf36e-8b3a-4b00-99fb-2e4d1da706d6",
            "resourceAppId": "00000003-0000-0000-c000-000000000000",
            "permissionType": "Application",
            "permission": "TeamsTab.Create.Group"
        },
        {
            "id": "wtAZautz7ilRA0kgHYWr2Ss2FTK3jPkf-HPhj3FS1wo",
            "deletedDateTime": null,
            "clientId": "74c92190-dc0e-485a-81c6-fdffd4aadfd8",
            "clientAppId": "69024002-35ae-4574-a219-f261183580b4",
            "resourceAppId": "00000003-0000-0000-c000-000000000000",
            "permissionType": "Application",
            "permission": "TeamMember.Read.Group"
        }
    ]
}
```
