---
title: Listar permissionGrants de um chat
description: Recuperar permissionGrants de um chat.
author: akjo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2d5da4231039a88161bfb691034fbe2cab806f4e
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610687"
---
# <a name="list-permissiongrants-of-a-chat"></a><span data-ttu-id="02396-103">Listar permissionGrants de um chat</span><span class="sxs-lookup"><span data-stu-id="02396-103">List permissionGrants of a chat</span></span>

<span data-ttu-id="02396-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02396-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02396-105">Listar tudo [concessões de permissão para recursos específicos](../resources/resourcespecificpermissiongrant.md) no [chat](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="02396-105">List all [resource-specific permission grants](../resources/resourcespecificpermissiongrant.md) on the [chat](../resources/chat.md).</span></span> <span data-ttu-id="02396-106">Esta é uma lista de aplicativos do Azure AD que têm acesso ao chat junto com o tipo de acesso que cada aplicativo tem.</span><span class="sxs-lookup"><span data-stu-id="02396-106">This is a list of Azure AD apps that have access to the chat along with the kind of access that each app has.</span></span>

## <a name="permissions"></a><span data-ttu-id="02396-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="02396-107">Permissions</span></span>

<span data-ttu-id="02396-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02396-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="02396-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02396-110">Permission Type</span></span>                        | <span data-ttu-id="02396-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02396-111">Permissions (from least to most privileged)</span></span>                                                                                                                                                        |
| :------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="02396-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02396-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="02396-113">ResourceSpecificPermissionGrant.ReadForChat, TeamsAppInstallation.ReadForChat, TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="02396-113">ResourceSpecificPermissionGrant.ReadForChat, TeamsAppInstallation.ReadForChat, TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span>                                    |
| <span data-ttu-id="02396-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02396-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02396-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02396-115">Not supported.</span></span>                                                                                                                                                                                     |
| <span data-ttu-id="02396-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02396-116">Application</span></span>                            | <span data-ttu-id="02396-117">Chat.Manage.Chat\*, ResourceSpecificPermissionGrant.ReadForChat.All, TeamsAppInstallation.ReadForChat.All, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="02396-117">Chat.Manage.Chat\*, ResourceSpecificPermissionGrant.ReadForChat.All, TeamsAppInstallation.ReadForChat.All, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02396-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02396-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/permissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="02396-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="02396-119">Optional query parameters</span></span>

<span data-ttu-id="02396-120">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="02396-120">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="02396-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02396-121">Request headers</span></span>

| <span data-ttu-id="02396-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02396-122">Header</span></span>           | <span data-ttu-id="02396-123">Valor</span><span class="sxs-lookup"><span data-stu-id="02396-123">Value</span></span>                      |
| :--------------- | :------------------------- |
| <span data-ttu-id="02396-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="02396-124">Authorization</span></span>    | <span data-ttu-id="02396-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02396-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="02396-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02396-127">Request body</span></span>

<span data-ttu-id="02396-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="02396-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02396-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="02396-129">Response</span></span>

<span data-ttu-id="02396-130">Se for bem-sucedido, este método retorna um `200 OK` código de resposta e uma lista de [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) objetos no corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="02396-130">If successful, this method returns a `200 OK` response code and a list of [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="02396-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="02396-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="02396-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02396-132">Request</span></span>

<span data-ttu-id="02396-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="02396-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="02396-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="02396-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_list_permission_grants"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/19:089ac694c48647c68035aae675cf78ab@thread.v2/permissionGrants
```
# <a name="c"></a>[<span data-ttu-id="02396-135">C#</span><span class="sxs-lookup"><span data-stu-id="02396-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-list-permission-grants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02396-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02396-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-list-permission-grants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02396-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02396-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-list-permission-grants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="02396-138">Java</span><span class="sxs-lookup"><span data-stu-id="02396-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-list-permission-grants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="02396-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="02396-139">Response</span></span>

<span data-ttu-id="02396-140">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="02396-140">The following example shows the response.</span></span>

><span data-ttu-id="02396-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="02396-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.resourceSpecificPermissionGrant"
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
            "permission": "ChatSettings.ReadWrite.Chat"
        },
        {
            "id": "Y2VkZGEyMWUtYTUwZS00ZDI3LWEyZjAtOTk0MTMwMGY3Y2I1IyNUZWFtc0FwcEluc3RhbGxhdGlvbi5SZWFkLkNoYXQjI0FwcGxpY2F0aW9u",
            "clientAppId": "fdebf36e-8b3a-4b00-99fb-2e4d1da706d6",
            "resourceAppId": "00000003-0000-0000-c000-000000000000",
            "clientId": "771b9da9-2260-41eb-a587-4d936e4aa08c",
            "permissionType": "Application",
            "permission": "TeamsAppInstallation.Read.Chat"
        },
        {
            "id": "Y2VkZGEyMWUtYTUwZS00ZDI3LWEyZjAtOTk0MTMwMGY3Y2I1IyNUZWFtc1RhYi5EZWxldGUuQ2hhdCMjQXBwbGljYXRpb24=",
            "clientAppId": "fdebf36e-8b3a-4b00-99fb-2e4d1da706d6",
            "resourceAppId": "00000003-0000-0000-c000-000000000000",
            "clientId": "771b9da9-2260-41eb-a587-4d936e4aa08c",
            "permissionType": "Application",
            "permission": "TeamsTab.Delete.Chat"
        },
        {
            "id": "ZmNmMGMzNjQtMWY1ZS00MDVjLThiN2QtNjI2YmRmOWQyZjI1IyNDaGF0U2V0dGluZ3MuUmVhZC5DaGF0IyNBcHBsaWNhdGlvbg==",
            "clientAppId": "69024002-35ae-4574-a219-f261183580b4",
            "resourceAppId": "00000003-0000-0000-c000-000000000000",
            "clientId": "74c92190-dc0e-485a-81c6-fdffd4aadfd8",
            "permissionType": "Application",
            "permission": "ChatSettings.Read.Chat"
        },
    ]
}
```
