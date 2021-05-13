---
title: 'accessPackage: filterByCurrentUser'
description: Recupere uma lista de objetos accesspackage filtrados no usuário de entrada.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 9dbc8275bceceff6fb6beb90e3bfcf5acb476baa
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474033"
---
# <a name="accesspackage-filterbycurrentuser"></a><span data-ttu-id="92eb9-103">accessPackage: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="92eb9-103">accessPackage: filterByCurrentUser</span></span>
<span data-ttu-id="92eb9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92eb9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92eb9-105">No [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md), recupere uma lista de objetos [accessPackage](../resources/accesspackage.md) filtrados no usuário de entrada.</span><span class="sxs-lookup"><span data-stu-id="92eb9-105">In [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackage](../resources/accesspackage.md) objects filtered on the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="92eb9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="92eb9-106">Permissions</span></span>
<span data-ttu-id="92eb9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92eb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92eb9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92eb9-109">Permission type</span></span>|<span data-ttu-id="92eb9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92eb9-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92eb9-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92eb9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="92eb9-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92eb9-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>|
|<span data-ttu-id="92eb9-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92eb9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92eb9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92eb9-114">Not supported.</span></span>|
|<span data-ttu-id="92eb9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92eb9-115">Application</span></span>|<span data-ttu-id="92eb9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92eb9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92eb9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92eb9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/accessPackages/filterByCurrentUser
```

## <a name="function-parameters"></a><span data-ttu-id="92eb9-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="92eb9-118">Function parameters</span></span>
<span data-ttu-id="92eb9-119">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="92eb9-119">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="92eb9-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="92eb9-120">Parameter</span></span>|<span data-ttu-id="92eb9-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="92eb9-121">Type</span></span>|<span data-ttu-id="92eb9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="92eb9-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92eb9-123">on</span><span class="sxs-lookup"><span data-stu-id="92eb9-123">on</span></span>|[<span data-ttu-id="92eb9-124">accessPackageFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="92eb9-124">accessPackageFilterByCurrentUserOptions</span></span>](../resources/accesspackage-accesspackagefilterbycurrentuseroptions.md)|<span data-ttu-id="92eb9-125">A lista de opções de usuário atuais que podem ser usadas para filtrar na lista de pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="92eb9-125">The list of current user options that can be used to filter on the access packages list.</span></span>|

- <span data-ttu-id="92eb9-126">`allowedRequestor` é usado para obter os objetos para os quais o usuário interno tem permissão `accessPackage` para enviar solicitações de acesso.</span><span class="sxs-lookup"><span data-stu-id="92eb9-126">`allowedRequestor` is used to get the `accessPackage` objects for which the signed-in user is allowed to submit access requests.</span></span> <span data-ttu-id="92eb9-127">A lista resultante inclui todos os pacotes de acesso que podem ser solicitados pelo chamador em todos os catálogos.</span><span class="sxs-lookup"><span data-stu-id="92eb9-127">The resulting list includes all access packages that can be requested by the caller across all catalogs.</span></span>

## <a name="request-headers"></a><span data-ttu-id="92eb9-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92eb9-128">Request headers</span></span>
|<span data-ttu-id="92eb9-129">Nome</span><span class="sxs-lookup"><span data-stu-id="92eb9-129">Name</span></span>|<span data-ttu-id="92eb9-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="92eb9-130">Description</span></span>|
|:---|:---|
|<span data-ttu-id="92eb9-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="92eb9-131">Authorization</span></span>|<span data-ttu-id="92eb9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92eb9-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="92eb9-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92eb9-134">Request body</span></span>
<span data-ttu-id="92eb9-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="92eb9-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92eb9-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="92eb9-136">Response</span></span>

<span data-ttu-id="92eb9-137">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção [accessPackage](../resources/accesspackage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92eb9-137">If successful, this method returns a `200 OK` response code and an [accessPackage](../resources/accesspackage.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="92eb9-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="92eb9-138">Examples</span></span>
<span data-ttu-id="92eb9-139">O exemplo a seguir obtém os pacotes de acesso que podem ser solicitados pelo usuário interno.</span><span class="sxs-lookup"><span data-stu-id="92eb9-139">The following example gets the access packages that can be requested by the signed-in user.</span></span>

### <a name="request"></a><span data-ttu-id="92eb9-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92eb9-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="92eb9-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="92eb9-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accesspackageassignmentrequest_filterByCurrentUser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/filterByCurrentUser(on='allowedRequestor')
```
# <a name="c"></a>[<span data-ttu-id="92eb9-142">C#</span><span class="sxs-lookup"><span data-stu-id="92eb9-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accesspackageassignmentrequest-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92eb9-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92eb9-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accesspackageassignmentrequest-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92eb9-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92eb9-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accesspackageassignmentrequest-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92eb9-145">Java</span><span class="sxs-lookup"><span data-stu-id="92eb9-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accesspackageassignmentrequest-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="92eb9-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="92eb9-146">Response</span></span>
> <span data-ttu-id="92eb9-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="92eb9-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignmentRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessPackage",
            "id": "d378b3b7-b42a-445a-8780-2841194f777e",
            "catalogId": "eb0f5e12-484d-4545-8ae1-fb1dfc28ab3c",
            "displayName": "Sales resources",
            "description": "Resources needed by the Sales department.",
            "isHidden": false,
            "isRoleScopesVisible": false,
            "createdBy": "TestGA@example.com",
            "createdDateTime": "2021-01-26T22:30:57.37Z",
            "modifiedBy": "TestGA@example.com",
            "modifiedDateTime": "2021-01-26T22:30:57.37Z"
        }
    ]
}
```

