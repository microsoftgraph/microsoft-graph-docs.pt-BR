---
title: Criar accessPackageResourceRequest
description: Crie um novo accessPackageResourceRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 82b84110f7936ea8a5bfef7e7d479ecc6c4aaeea
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439461"
---
# <a name="create-accesspackageresourcerequest"></a><span data-ttu-id="89e7c-103">Criar accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="89e7c-103">Create accessPackageResourceRequest</span></span>

<span data-ttu-id="89e7c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89e7c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89e7c-105">Crie um novo [objeto accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) para solicitar a adição de um recurso a um catálogo de pacotes de acesso ou a remoção de um recurso de um catálogo.</span><span class="sxs-lookup"><span data-stu-id="89e7c-105">Create a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object to request the addition of a resource to an access package catalog, or the removal of a resource from a catalog.</span></span>

## <a name="permissions"></a><span data-ttu-id="89e7c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="89e7c-106">Permissions</span></span>

<span data-ttu-id="89e7c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89e7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="89e7c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89e7c-109">Permission type</span></span>                        | <span data-ttu-id="89e7c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="89e7c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="89e7c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89e7c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="89e7c-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89e7c-112">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="89e7c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89e7c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89e7c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89e7c-114">Not supported.</span></span> |
| <span data-ttu-id="89e7c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89e7c-115">Application</span></span>                            | <span data-ttu-id="89e7c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89e7c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="89e7c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89e7c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## <a name="request-headers"></a><span data-ttu-id="89e7c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89e7c-118">Request headers</span></span>

| <span data-ttu-id="89e7c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="89e7c-119">Name</span></span>          | <span data-ttu-id="89e7c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="89e7c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="89e7c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="89e7c-121">Authorization</span></span> | <span data-ttu-id="89e7c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89e7c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="89e7c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="89e7c-124">Content-Type</span></span>  | <span data-ttu-id="89e7c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89e7c-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="89e7c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89e7c-127">Request body</span></span>

<span data-ttu-id="89e7c-128">No corpo da solicitação, fornece uma representação JSON de um [objeto accessPackageResourceRequest.](../resources/accesspackageresourcerequest.md)</span><span class="sxs-lookup"><span data-stu-id="89e7c-128">In the request body, supply a JSON representation of an [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.</span></span> <span data-ttu-id="89e7c-129">Inclua a `accessPackageResource` relação com um objeto [accessPackageResource](../resources/accesspackageresource.md) como parte da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89e7c-129">Include the `accessPackageResource` relationship with an [accessPackageResource](../resources/accesspackageresource.md) object as part of the request.</span></span>

<span data-ttu-id="89e7c-130">Para adicionar um grupo do Azure AD como um recurso a um catálogo, de definir a **catalogId** como da ID do catálogo, **requestType** como e representando o `AdminAdd` `accessPackageResource` recurso.</span><span class="sxs-lookup"><span data-stu-id="89e7c-130">To add an Azure AD group as a resource to a catalog, set the **catalogId** to be of the ID of the catalog, **requestType** to be `AdminAdd`, and an `accessPackageResource` representing the resource.</span></span> <span data-ttu-id="89e7c-131">O valor da **propriedade originSystem** dentro do deve ser e `accessPackageResource` o valor da `AadGroup` **originId** é o identificador do grupo.</span><span class="sxs-lookup"><span data-stu-id="89e7c-131">The value of the **originSystem** property within the `accessPackageResource` should be `AadGroup` and the value of the **originId** is the identifier of the group.</span></span>

<span data-ttu-id="89e7c-132">Para remover um aplicativo do Azure AD de um catálogo, de definir **a catalogId** como da ID do catálogo, **requestType** como e o objeto de recurso a ser `AdminRemove` `accessPackageResource` removido.</span><span class="sxs-lookup"><span data-stu-id="89e7c-132">To remove an Azure AD app from a catalog, set the **catalogId** to be of the ID of the catalog, **requestType** to be `AdminRemove`, and the `accessPackageResource` the resource object to be removed.</span></span>  <span data-ttu-id="89e7c-133">O objeto resource pode ser recuperado usando [accessPackageResources](accesspackagecatalog-list-accesspackageresources.md)de lista.</span><span class="sxs-lookup"><span data-stu-id="89e7c-133">The resource object can be retrieved using [list accessPackageResources](accesspackagecatalog-list-accesspackageresources.md).</span></span>

<span data-ttu-id="89e7c-134">Para atribuir o ambiente de localização geográfica a um recurso do Sharepoint Online multilocação geográfica, inclua a relação **accessPackageResourceEnvironment** no `accessPackageResource` objeto.</span><span class="sxs-lookup"><span data-stu-id="89e7c-134">To assign the geolocation environment for a multi-geolocation Sharepoint Online resource, include the **accessPackageResourceEnvironment** relationship in the `accessPackageResource` object.</span></span> <span data-ttu-id="89e7c-135">Isso pode ser feito de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="89e7c-135">This can be done in two ways:</span></span>
+ <span data-ttu-id="89e7c-136">Use `@odata.bind` anotação para atribuir `id` o do a um `accessPackageResourceEnvironment` `accessPackageResourceEnvironment` objeto.</span><span class="sxs-lookup"><span data-stu-id="89e7c-136">Use `@odata.bind` annotation to assign the `id` of the `accessPackageResourceEnvironment` to an `accessPackageResourceEnvironment` object.</span></span>
+ <span data-ttu-id="89e7c-137">`originId`Especifique o parâmetro do em um `accessPackageResourceEnvironment` `accessPackageResourceEnvironment` objeto.</span><span class="sxs-lookup"><span data-stu-id="89e7c-137">Specify the `originId` parameter of the `accessPackageResourceEnvironment` in an `accessPackageResourceEnvironment` object.</span></span>


## <a name="response"></a><span data-ttu-id="89e7c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="89e7c-138">Response</span></span>

<span data-ttu-id="89e7c-139">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89e7c-139">If successful, this method returns a `201 Created` response code and a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="89e7c-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="89e7c-140">Examples</span></span>

### <a name="example-1-create-an-accesspackageresourcerequest"></a><span data-ttu-id="89e7c-141">Exemplo 1: Criar um accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="89e7c-141">Example 1: Create an accessPackageResourceRequest</span></span>

#### <a name="request"></a><span data-ttu-id="89e7c-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89e7c-142">Request</span></span>

<span data-ttu-id="89e7c-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="89e7c-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="89e7c-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="89e7c-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerequest_from_accesspackageresourcerequests"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-type: application/json

{
  "catalogId":"26ac0c0a-08bc-4a7b-a313-839f58044ba5",
  "requestType": "AdminAdd",
  "justification": "",
  "accessPackageResource": {
     "displayName": "Sales",
     "description": "https://contoso.sharepoint.com/sites/Sales",
     "url": "https://contoso.sharepoint.com/sites/Sales",
     "resourceType": "SharePoint Online Site",
     "originId": "https://contoso.sharepoint.com/sites/Sales",
     "originSystem": "SharePointOnline"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="89e7c-145">C#</span><span class="sxs-lookup"><span data-stu-id="89e7c-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89e7c-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89e7c-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89e7c-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89e7c-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89e7c-148">Java</span><span class="sxs-lookup"><span data-stu-id="89e7c-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="89e7c-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="89e7c-149">Response</span></span>

<span data-ttu-id="89e7c-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="89e7c-150">The following is an example of the response.</span></span>

> <span data-ttu-id="89e7c-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89e7c-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "catalogId": "26ac0c0a-08bc-4a7b-a313-839f58044ba5",
  "id": "1fe272f0-d463-42aa-a9a8-b07ab50a1c4d",
  "isValidationOnly": false,
  "justification": "",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled",
  "requestType": "AdminAdd"
}
```

### <a name="example-2-create-an-accesspackageresourcerequest-for-a-resource-and-assign-an-accesspackageresourceenvironment-using-odatabind"></a><span data-ttu-id="89e7c-153">Exemplo 2: crie um accessPackageResourceRequest para um recurso e atribua um accessPackageResourceEnvironment usando @odata.bind</span><span class="sxs-lookup"><span data-stu-id="89e7c-153">Example 2: Create an accessPackageResourceRequest for a resource and assign an accessPackageResourceEnvironment using @odata.bind</span></span>

#### <a name="request"></a><span data-ttu-id="89e7c-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89e7c-154">Request</span></span>

<span data-ttu-id="89e7c-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="89e7c-155">The following is an example of the request.</span></span> <span data-ttu-id="89e7c-156">Neste exemplo, a `@odata.bind` anotação é usada para atribuir o `id` do a um `accessPackageResourceEnvironment` `accessPackageResourceEnvironment` objeto.</span><span class="sxs-lookup"><span data-stu-id="89e7c-156">In this example, the `@odata.bind` annotation is used to assign the `id` of the `accessPackageResourceEnvironment` to an `accessPackageResourceEnvironment` object.</span></span>



# <a name="http"></a>[<span data-ttu-id="89e7c-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="89e7c-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerequest_from_accesspackageresourcerequests_with_accessPackageResourceEnvironment"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-type: application/json

{
    "catalogId": "de9315c1-272b-4905-924b-cc112ca180c7",
    "accessPackageResource": {
        "displayName": "Community Outreach",
        "description": "https://contoso.sharepoint.com/sites/CSR",
        "resourceType": "SharePoint Online Site",
        "originId": "https://contoso.sharepoint.com/sites/CSR",
        "originSystem": "SharePointOnline",
        "accessPackageResourceEnvironment@odata.bind": "accessPackageResourceEnvironments/615f2218-678f-471f-a60a-02c2f4f80c57"
    },
    "requestType": "AdminAdd"
}
```
# <a name="c"></a>[<span data-ttu-id="89e7c-158">C#</span><span class="sxs-lookup"><span data-stu-id="89e7c-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89e7c-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89e7c-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89e7c-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89e7c-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89e7c-161">Java</span><span class="sxs-lookup"><span data-stu-id="89e7c-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="89e7c-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="89e7c-162">Response</span></span>

<span data-ttu-id="89e7c-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="89e7c-163">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageResourceRequests/$entity",
    "catalogId": "de9315c1-272b-4905-924b-cc112ca180c7",
    "executeImmediately": false,
    "id": "d3f800d5-0dd6-47f3-9e90-ef562c7551dc",
    "requestType": "AdminAdd",
    "requestState": "Delivered",
    "requestStatus": "Fulfilled",
    "isValidationOnly": false,
    "expirationDateTime": null,
    "justification": null
}
```

### <a name="example-3-create-an-accesspackageresourcerequest-for-a-resource-and-assign-an-accesspackageresourceenvironment-using-originid"></a><span data-ttu-id="89e7c-164">Exemplo 3: criar um accessPackageResourceRequest para um recurso e atribuir um accessPackageResourceEnvironment usando originId</span><span class="sxs-lookup"><span data-stu-id="89e7c-164">Example 3: Create an accessPackageResourceRequest for a resource and assign an accessPackageResourceEnvironment using originId</span></span>

#### <a name="request"></a><span data-ttu-id="89e7c-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89e7c-165">Request</span></span>

<span data-ttu-id="89e7c-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="89e7c-166">The following is an example of the request.</span></span> <span data-ttu-id="89e7c-167">Neste exemplo, os parâmetros de um `accessPackageResourceEnvironment` são especificados em um `accessPackageResourceEnvironment` objeto.</span><span class="sxs-lookup"><span data-stu-id="89e7c-167">In this example, the parameters of an `accessPackageResourceEnvironment` are specified in an `accessPackageResourceEnvironment` object.</span></span>



# <a name="http"></a>[<span data-ttu-id="89e7c-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="89e7c-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerequest_from_accesspackageresourcerequests_with_accessPackageResourceEnvironment_New"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-type: application/json

{
    "catalogId": "de9315c1-272b-4905-924b-cc112ca180c7",
    "accessPackageResource": {
        "displayName": "Community Outreach",
        "description": "https://contoso.sharepoint.com/sites/CSR",
        "resourceType": "SharePoint Online Site",
        "originId": "https://contoso.sharepoint.com/sites/CSR",
        "originSystem": "SharePointOnline",
        "accessPackageResourceEnvironment": {
            "originId": "https://contoso-admin.sharepoint.com/"
        }
    },
    "requestType": "AdminAdd"
}
```
# <a name="c"></a>[<span data-ttu-id="89e7c-169">C#</span><span class="sxs-lookup"><span data-stu-id="89e7c-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89e7c-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89e7c-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89e7c-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89e7c-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89e7c-172">Java</span><span class="sxs-lookup"><span data-stu-id="89e7c-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="89e7c-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="89e7c-173">Response</span></span>

<span data-ttu-id="89e7c-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="89e7c-174">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageResourceRequests/$entity",
    "catalogId": "de9315c1-272b-4905-924b-cc112ca180c7",
    "executeImmediately": false,
    "id": "eadf3fbb-668c-4c3a-8d84-7c8bd73dc3e4",
    "requestType": "AdminAdd",
    "requestState": "Delivered",
    "requestStatus": "Fulfilled",
    "isValidationOnly": false,
    "expirationDateTime": null,
    "justification": null
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageResourceRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
