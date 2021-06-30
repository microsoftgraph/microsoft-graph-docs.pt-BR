---
title: Listar permissionGrants de uma equipe
description: Recuperar permissionGrants de uma equipe.
author: jecha
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: dd29d1cb777d8dd32a7cec97d24a1e152428bd77
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209643"
---
# <a name="list-permissiongrants-of-a-team"></a><span data-ttu-id="e860c-103">Listar permissionGrants de uma equipe</span><span class="sxs-lookup"><span data-stu-id="e860c-103">List permissionGrants of a team</span></span>

<span data-ttu-id="e860c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e860c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e860c-p101">Listar todas [concessões de permissão específicas de recursos](../resources/resourcespecificpermissiongrant.md) na [equipe](../resources/team.md). Esta lista especifica os aplicativos Microsoft Azure Active Directory que têm acesso à **equipe**, juntamente com o tipo correspondente de acesso específico de recursos que cada aplicativo tem.</span><span class="sxs-lookup"><span data-stu-id="e860c-p101">List all [resource-specific permission grants](../resources/resourcespecificpermissiongrant.md) on the [team](../resources/team.md). This list specifies the Azure AD apps that have access to the **team**, along with the corresponding kind of resource-specific access that each app has.</span></span>

## <a name="permissions"></a><span data-ttu-id="e860c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e860c-107">Permissions</span></span>

<span data-ttu-id="e860c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e860c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e860c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e860c-110">Permission Type</span></span>                        | <span data-ttu-id="e860c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e860c-111">Permissions (from least to most privileged)</span></span>                                                                                                                                                                                                                              |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="e860c-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e860c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e860c-113">TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadWriteForTeam</span><span class="sxs-lookup"><span data-stu-id="e860c-113">TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadWriteForTeam</span></span>                                                                     |
| <span data-ttu-id="e860c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e860c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e860c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e860c-115">Not supported.</span></span>                                                                                                                                                                                                                                                           |
| <span data-ttu-id="e860c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e860c-116">Application</span></span>                            | <span data-ttu-id="e860c-117">TeamsAppInstallation.Read.Group *, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteSelfForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, TeamsApp.Read.Group*</span><span class="sxs-lookup"><span data-stu-id="e860c-117">TeamsAppInstallation.Read.Group *, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteSelfForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, TeamsApp.Read.Group*</span></span> |

> <span data-ttu-id="e860c-118">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="e860c-118">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="e860c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e860c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/permissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e860c-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e860c-120">Optional query parameters</span></span>

<span data-ttu-id="e860c-121">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e860c-121">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e860c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e860c-122">Request headers</span></span>

| <span data-ttu-id="e860c-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e860c-123">Header</span></span>           | <span data-ttu-id="e860c-124">Valor</span><span class="sxs-lookup"><span data-stu-id="e860c-124">Value</span></span>                      |
| :--------------- | :------------------------- |
| <span data-ttu-id="e860c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e860c-125">Authorization</span></span>    | <span data-ttu-id="e860c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e860c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e860c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e860c-128">Request body</span></span>

<span data-ttu-id="e860c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e860c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e860c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e860c-130">Response</span></span>

<span data-ttu-id="e860c-131">Se for bem-sucedido, este método retorna um `200 OK` código de resposta e uma lista de [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) objetos no corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e860c-131">If successful, this method returns a `200 OK` response code and a list of [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e860c-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e860c-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e860c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e860c-133">Request</span></span>

<span data-ttu-id="e860c-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e860c-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e860c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e860c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_list_permission_grants"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/14c981a4-dca9-4565-bae6-e13ada8861be/permissionGrants
```
# <a name="c"></a>[<span data-ttu-id="e860c-136">C#</span><span class="sxs-lookup"><span data-stu-id="e860c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-list-permission-grants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e860c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e860c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-list-permission-grants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e860c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e860c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-list-permission-grants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e860c-139">Java</span><span class="sxs-lookup"><span data-stu-id="e860c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-list-permission-grants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="e860c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e860c-140">Response</span></span>

<span data-ttu-id="e860c-141">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="e860c-141">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.resourceSpecificPermissionGrant",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#permissionGrants",
    "value": [
        {
            "id": "Y2VkZGEyMWUtYTUwZS00ZDI3LWEyZjAtOTk0MTMwMGY3Y2I1IyNDaGF0U2V0dGluZ3MuUmVhZFdyaXRlLkNoYXQjI0FwcGxpY2F0aW9u",
            "clientAppId": "fdebf36e-8b3a-4b00-99fb-2e4d1da706d6",
            "resourceAppId": "00000003-0000-0000-c000-000000000000",
            "clientId": "771b9da9-2260-41eb-a587-4d936e4aa08c",
            "permissionType": "Application",
            "permission": "TeamMember.Read.Group"
        },
        {
            "id": "Y2VkZGEyMWUtYTUwZS00ZDI3LWEyZjAtOTk0MTMwMGY3Y2I1IyNUZWFtc0FwcEluc3RhbGxhdGlvbi5SZWFkLkNoYXQjI0FwcGxpY2F0aW9u",
            "clientAppId": "fdebf36e-8b3a-4b00-99fb-2e4d1da706d6",
            "resourceAppId": "00000003-0000-0000-c000-000000000000",
            "clientId": "771b9da9-2260-41eb-a587-4d936e4aa08c",
            "permissionType": "Application",
            "permission": "TeamsTab.Create.Group"
        },
        {
            "id": "ZmNmMGMzNjQtMWY1ZS00MDVjLThiN2QtNjI2YmRmOWQyZjI1IyNDaGF0U2V0dGluZ3MuUmVhZC5DaGF0IyNBcHBsaWNhdGlvbg==",
            "clientAppId": "69024002-35ae-4574-a219-f261183580b4",
            "resourceAppId": "00000003-0000-0000-c000-000000000000",
            "clientId": "74c92190-dc0e-485a-81c6-fdffd4aadfd8",
            "permissionType": "Application",
            "permission": "TeamMember.Read.Group"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="e860c-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="e860c-142">See also</span></span>
- [<span data-ttu-id="e860c-143">Listar concessões de permissão de um grupo</span><span class="sxs-lookup"><span data-stu-id="e860c-143">List permission grants of a group</span></span>](group-list-permissionGrants.md)
- [<span data-ttu-id="e860c-144">Listar concessões de permissão de um chat</span><span class="sxs-lookup"><span data-stu-id="e860c-144">List permission grants of a chat</span></span>](chat-list-permissionGrants.md)
