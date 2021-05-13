---
title: 'accessPackageAssignmentRequest: filterByCurrentUser'
description: Recupere uma lista de objetos accesspackageassignmentrequest filtrados no usuário de entrada.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f65ca1c94f2702245b1765e904bb3c559cab6685
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52473945"
---
# <a name="accesspackageassignmentrequest-filterbycurrentuser"></a><span data-ttu-id="231ec-103">accessPackageAssignmentRequest: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="231ec-103">accessPackageAssignmentRequest: filterByCurrentUser</span></span>
<span data-ttu-id="231ec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="231ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="231ec-105">No [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md), recupere uma lista de objetos [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) filtrados no usuário de entrada.</span><span class="sxs-lookup"><span data-stu-id="231ec-105">In [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects filtered on the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="231ec-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="231ec-106">Permissions</span></span>
<span data-ttu-id="231ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="231ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="231ec-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="231ec-109">Permission type</span></span>|<span data-ttu-id="231ec-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="231ec-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="231ec-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="231ec-111">Delegated (work or school account)</span></span>|<span data-ttu-id="231ec-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="231ec-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>|
|<span data-ttu-id="231ec-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="231ec-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="231ec-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="231ec-114">Not supported.</span></span>|
|<span data-ttu-id="231ec-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="231ec-115">Application</span></span>|<span data-ttu-id="231ec-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="231ec-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="231ec-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="231ec-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/filterByCurrentUser
```

## <a name="function-parameters"></a><span data-ttu-id="231ec-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="231ec-118">Function parameters</span></span>
<span data-ttu-id="231ec-119">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="231ec-119">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="231ec-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="231ec-120">Parameter</span></span>|<span data-ttu-id="231ec-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="231ec-121">Type</span></span>|<span data-ttu-id="231ec-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="231ec-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="231ec-123">on</span><span class="sxs-lookup"><span data-stu-id="231ec-123">on</span></span>|[<span data-ttu-id="231ec-124">accessPackageAssignmentRequestFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="231ec-124">accessPackageAssignmentRequestFilterByCurrentUserOptions</span></span>](../resources/accesspackageassignmentrequest-accesspackageassignmentrequestfilterbycurrentuseroptions.md)|<span data-ttu-id="231ec-125">A lista de opções de usuário atuais que podem ser usadas para filtrar na lista de solicitações de atribuição de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="231ec-125">The list of current user options that can be used to filter on the access package assignment requests list.</span></span>|

- <span data-ttu-id="231ec-126">`target` é usado para obter os `accessPackageAssignmentRequest` objetos em que o usuário inscreva é o destino.</span><span class="sxs-lookup"><span data-stu-id="231ec-126">`target` is used to get the `accessPackageAssignmentRequest` objects where the signed-in user is the target.</span></span> <span data-ttu-id="231ec-127">A lista resultante inclui todas as solicitações de atribuição, atuais e expiradas, que foram solicitadas pelo chamador ou pelo chamador, em todos os catálogos e pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="231ec-127">The resulting list includes all the assignment requests, current and expired, that were requested by the caller or for the caller, across all catalogs and access packages.</span></span>

- <span data-ttu-id="231ec-128">`createdBy` é usado para obter `accessPackageAssignmentRequest` os objetos criados pelo usuário in-locar.</span><span class="sxs-lookup"><span data-stu-id="231ec-128">`createdBy` is used to get the `accessPackageAssignmentRequest` objects created by the signed-in user.</span></span> <span data-ttu-id="231ec-129">A lista resultante inclui todas as solicitações de atribuição que o chamador criou para si ou em nome de outras pessoas, como no caso de atribuição direta do administrador, em todos os catálogos e pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="231ec-129">The resulting list includes all of the assignment requests that the caller has created for themselves or on behalf of others, such as in case of admin direct assignment, across all catalogs and access packages.</span></span>

- <span data-ttu-id="231ec-130">`approver` é usado para obter os objetos em que o usuário inscreve é um aprovador permitido `accessPackageAssignmentRequest` em qualquer contido ( ou `accessPackageAssignment/accessPackageAssignmentPolicy/requestApprovalSettings/approvalStages` `primaryApprovers` `escalationApprovers` ).</span><span class="sxs-lookup"><span data-stu-id="231ec-130">`approver` is used to get the `accessPackageAssignmentRequest` objects where the signed-in user is an allowed approver in any contained `accessPackageAssignment/accessPackageAssignmentPolicy/requestApprovalSettings/approvalStages` (`primaryApprovers` or `escalationApprovers`).</span></span> <span data-ttu-id="231ec-131">A lista resultante inclui as  solicitações de atribuição em estado pendente, em todos os catálogos e pacotes de acesso e que precisam de uma decisão do chamador.</span><span class="sxs-lookup"><span data-stu-id="231ec-131">The resulting list includes the assignment requests in *pending* state, across all catalogs and access packages and that need a decision from the caller.</span></span> <span data-ttu-id="231ec-132">A lista resultante inclui as solicitações de atribuição em um estado, em todos os catálogos e pacotes de acesso e que precisam de uma decisão `pending` do chamador.</span><span class="sxs-lookup"><span data-stu-id="231ec-132">The resulting list includes the assignment requests in a `pending` state, across all catalogs and access packages and that need a decision from the caller.</span></span>

## <a name="request-headers"></a><span data-ttu-id="231ec-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="231ec-133">Request headers</span></span>
|<span data-ttu-id="231ec-134">Nome</span><span class="sxs-lookup"><span data-stu-id="231ec-134">Name</span></span>|<span data-ttu-id="231ec-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="231ec-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="231ec-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="231ec-136">Authorization</span></span>|<span data-ttu-id="231ec-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="231ec-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="231ec-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="231ec-139">Request body</span></span>
<span data-ttu-id="231ec-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="231ec-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="231ec-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="231ec-141">Response</span></span>

<span data-ttu-id="231ec-142">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` [coleção accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="231ec-142">If successful, this method returns a `200 OK` response code and an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="231ec-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="231ec-143">Examples</span></span>

<span data-ttu-id="231ec-144">O exemplo a seguir obtém o status das solicitações de atribuição de pacote de acesso direcionadas para o usuário de entrada.</span><span class="sxs-lookup"><span data-stu-id="231ec-144">The following example gets the status of access package assignment requests targeted for the signed-in user.</span></span>

### <a name="request"></a><span data-ttu-id="231ec-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="231ec-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="231ec-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="231ec-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accesspackageassignmentrequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/filterByCurrentUser(on='target')
```
# <a name="c"></a>[<span data-ttu-id="231ec-147">C#</span><span class="sxs-lookup"><span data-stu-id="231ec-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accesspackageassignmentrequest-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="231ec-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="231ec-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accesspackageassignmentrequest-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="231ec-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="231ec-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accesspackageassignmentrequest-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="231ec-150">Java</span><span class="sxs-lookup"><span data-stu-id="231ec-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accesspackageassignmentrequest-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="231ec-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="231ec-151">Response</span></span>
> <span data-ttu-id="231ec-152">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="231ec-152">**Note:** The response object shown here might be shortened for readability.</span></span>
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
            "@odata.type": "#microsoft.graph.accessPackageAssignmentRequest",
            "createdDateTime": "2021-01-19T20:02:23.907Z",
            "completedDate": "2021-01-19T20:02:40.97Z",
            "id": "46c1410d-ef96-44c5-ae9c-a577d014fe0e",
            "requestType": "AdminAdd",
            "requestState": "Delivered",
            "requestStatus": "Fulfilled",
            "isValidationOnly": false,
            "expirationDateTime": null,
            "justification": null,
            "answers": [],
            "schedule": {
                "startDateTime": "2021-01-19T20:01:57.643Z",
                "recurrence": null,
                "expiration": {
                    "endDateTime": null,
                    "duration": null,
                    "type": "noExpiration"
                }
            }
        }
    ]
}
```

