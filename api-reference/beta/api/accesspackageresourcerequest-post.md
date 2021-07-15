---
title: Criar accessPackageResourceRequest
description: Crie um novo accessPackageResourceRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 7766eb9f6468ee93ce63a034b501e17d9653541a
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439123"
---
# <a name="create-accesspackageresourcerequest"></a><span data-ttu-id="5ee04-103">Criar accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="5ee04-103">Create accessPackageResourceRequest</span></span>

<span data-ttu-id="5ee04-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ee04-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ee04-105">Crie um novo [objeto accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) para solicitar a adição de um recurso a um catálogo de pacotes de acesso ou a remoção de um recurso de um catálogo.</span><span class="sxs-lookup"><span data-stu-id="5ee04-105">Create a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object to request the addition of a resource to an access package catalog, or the removal of a resource from a catalog.</span></span>  <span data-ttu-id="5ee04-106">Um recurso deve ser incluído em um catálogo de pacotes de acesso antes que a função desse recurso possa ser adicionada a um pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="5ee04-106">A resource must be included in an access package catalog before the role of that resource can be added to an access package.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ee04-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="5ee04-107">Permissions</span></span>

<span data-ttu-id="5ee04-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ee04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5ee04-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ee04-110">Permission type</span></span>                        | <span data-ttu-id="5ee04-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ee04-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5ee04-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ee04-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5ee04-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ee04-113">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="5ee04-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ee04-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ee04-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ee04-115">Not supported.</span></span> |
| <span data-ttu-id="5ee04-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ee04-116">Application</span></span>                            | <span data-ttu-id="5ee04-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ee04-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ee04-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ee04-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## <a name="request-headers"></a><span data-ttu-id="5ee04-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee04-119">Request headers</span></span>

| <span data-ttu-id="5ee04-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5ee04-120">Name</span></span>          | <span data-ttu-id="5ee04-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ee04-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5ee04-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ee04-122">Authorization</span></span> | <span data-ttu-id="5ee04-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ee04-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5ee04-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5ee04-125">Content-Type</span></span>  | <span data-ttu-id="5ee04-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ee04-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5ee04-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee04-128">Request body</span></span>

<span data-ttu-id="5ee04-129">No corpo da solicitação, fornece uma representação JSON de um [objeto accessPackageResourceRequest.](../resources/accesspackageresourcerequest.md)</span><span class="sxs-lookup"><span data-stu-id="5ee04-129">In the request body, supply a JSON representation of an [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.</span></span> <span data-ttu-id="5ee04-130">Inclua a `accessPackageResource` relação com um objeto [accessPackageResource](../resources/accesspackageresource.md) como parte da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ee04-130">Include the `accessPackageResource` relationship with an [accessPackageResource](../resources/accesspackageresource.md) object as part of the request.</span></span>

<span data-ttu-id="5ee04-131">Para adicionar um grupo do Azure AD como um recurso a um catálogo, de definir a **catalogId** como da ID do catálogo, **requestType** como e representando o `AdminAdd` `accessPackageResource` recurso.</span><span class="sxs-lookup"><span data-stu-id="5ee04-131">To add an Azure AD group as a resource to a catalog, set the **catalogId** to be of the ID of the catalog, **requestType** to be `AdminAdd`, and an `accessPackageResource` representing the resource.</span></span> <span data-ttu-id="5ee04-132">O valor da **propriedade originSystem** dentro do deve ser e `accessPackageResource` o valor da `AadGroup` **originId** é o identificador do grupo.</span><span class="sxs-lookup"><span data-stu-id="5ee04-132">The value of the **originSystem** property within the `accessPackageResource` should be `AadGroup` and the value of the **originId** is the identifier of the group.</span></span>

<span data-ttu-id="5ee04-133">Para remover um aplicativo do Azure AD de um catálogo, de definir **a catalogId** como da ID do catálogo, **requestType** como e o objeto de recurso a ser `AdminRemove` `accessPackageResource` removido.</span><span class="sxs-lookup"><span data-stu-id="5ee04-133">To remove an Azure AD app from a catalog, set the **catalogId** to be of the ID of the catalog, **requestType** to be `AdminRemove`, and the `accessPackageResource` the resource object to be removed.</span></span>  <span data-ttu-id="5ee04-134">O objeto resource pode ser recuperado usando [accessPackageResources](accesspackagecatalog-list-accesspackageresources.md)de lista.</span><span class="sxs-lookup"><span data-stu-id="5ee04-134">The resource object can be retrieved using [list accessPackageResources](accesspackagecatalog-list-accesspackageresources.md).</span></span>

<span data-ttu-id="5ee04-135">Para atribuir o ambiente de localização geográfica a um recurso do Sharepoint Online multilocação geográfica, inclua a relação **accessPackageResourceEnvironment** no `accessPackageResource` objeto.</span><span class="sxs-lookup"><span data-stu-id="5ee04-135">To assign the geolocation environment for a multi-geolocation Sharepoint Online resource, include the **accessPackageResourceEnvironment** relationship in the `accessPackageResource` object.</span></span> <span data-ttu-id="5ee04-136">Isso pode ser feito de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="5ee04-136">This can be done in two ways:</span></span>
+ <span data-ttu-id="5ee04-137">Use `@odata.bind` anotação para atribuir `id` o do a um `accessPackageResourceEnvironment` `accessPackageResourceEnvironment` objeto.</span><span class="sxs-lookup"><span data-stu-id="5ee04-137">Use `@odata.bind` annotation to assign the `id` of the `accessPackageResourceEnvironment` to an `accessPackageResourceEnvironment` object.</span></span>
+ <span data-ttu-id="5ee04-138">`originId`Especifique o parâmetro do em um `accessPackageResourceEnvironment` `accessPackageResourceEnvironment` objeto.</span><span class="sxs-lookup"><span data-stu-id="5ee04-138">Specify the `originId` parameter of the `accessPackageResourceEnvironment` in an `accessPackageResourceEnvironment` object.</span></span>


## <a name="response"></a><span data-ttu-id="5ee04-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ee04-139">Response</span></span>

<span data-ttu-id="5ee04-140">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ee04-140">If successful, this method returns a `201 Created` response code and a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5ee04-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5ee04-141">Examples</span></span>

### <a name="example-1-create-an-accesspackageresourcerequest-for-adding-a-site-as-a-resource"></a><span data-ttu-id="5ee04-142">Exemplo 1: Criar um accessPackageResourceRequest para adicionar um site como um recurso</span><span class="sxs-lookup"><span data-stu-id="5ee04-142">Example 1: Create an accessPackageResourceRequest for adding a site as a resource</span></span>

#### <a name="request"></a><span data-ttu-id="5ee04-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee04-143">Request</span></span>

<span data-ttu-id="5ee04-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ee04-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5ee04-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ee04-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5ee04-146">C#</span><span class="sxs-lookup"><span data-stu-id="5ee04-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ee04-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ee04-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ee04-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ee04-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ee04-149">Java</span><span class="sxs-lookup"><span data-stu-id="5ee04-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5ee04-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ee04-150">Response</span></span>

<span data-ttu-id="5ee04-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5ee04-151">The following is an example of the response.</span></span>

> <span data-ttu-id="5ee04-152">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5ee04-152">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-an-accesspackageresourcerequest-for-adding-a-site-as-a-resource-and-assign-an-accesspackageresourceenvironment-using-odatabind"></a><span data-ttu-id="5ee04-153">Exemplo 2: crie um accessPackageResourceRequest para adicionar um site como um recurso e atribuir um accessPackageResourceEnvironment usando @odata.bind</span><span class="sxs-lookup"><span data-stu-id="5ee04-153">Example 2: Create an accessPackageResourceRequest for adding a site as a resource and assign an accessPackageResourceEnvironment using @odata.bind</span></span>

#### <a name="request"></a><span data-ttu-id="5ee04-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee04-154">Request</span></span>

<span data-ttu-id="5ee04-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ee04-155">The following is an example of the request.</span></span> <span data-ttu-id="5ee04-156">Neste exemplo, a `@odata.bind` anotação é usada para atribuir o `id` do a um `accessPackageResourceEnvironment` `accessPackageResourceEnvironment` objeto.</span><span class="sxs-lookup"><span data-stu-id="5ee04-156">In this example, the `@odata.bind` annotation is used to assign the `id` of the `accessPackageResourceEnvironment` to an `accessPackageResourceEnvironment` object.</span></span>



# <a name="http"></a>[<span data-ttu-id="5ee04-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ee04-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5ee04-158">C#</span><span class="sxs-lookup"><span data-stu-id="5ee04-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ee04-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ee04-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ee04-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ee04-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ee04-161">Java</span><span class="sxs-lookup"><span data-stu-id="5ee04-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5ee04-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ee04-162">Response</span></span>

<span data-ttu-id="5ee04-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5ee04-163">The following is an example of the response.</span></span>

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

### <a name="example-3-create-an-accesspackageresourcerequest-for-adding-a-site-as-a-resource-and-assign-an-accesspackageresourceenvironment-using-originid"></a><span data-ttu-id="5ee04-164">Exemplo 3: criar um accessPackageResourceRequest para adicionar um site como um recurso e atribuir um accessPackageResourceEnvironment usando originId</span><span class="sxs-lookup"><span data-stu-id="5ee04-164">Example 3: Create an accessPackageResourceRequest for adding a site as a resource and assign an accessPackageResourceEnvironment using originId</span></span>

#### <a name="request"></a><span data-ttu-id="5ee04-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee04-165">Request</span></span>

<span data-ttu-id="5ee04-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ee04-166">The following is an example of the request.</span></span> <span data-ttu-id="5ee04-167">Neste exemplo, os parâmetros de um `accessPackageResourceEnvironment` são especificados em um `accessPackageResourceEnvironment` objeto.</span><span class="sxs-lookup"><span data-stu-id="5ee04-167">In this example, the parameters of an `accessPackageResourceEnvironment` are specified in an `accessPackageResourceEnvironment` object.</span></span>



# <a name="http"></a>[<span data-ttu-id="5ee04-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ee04-168">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5ee04-169">C#</span><span class="sxs-lookup"><span data-stu-id="5ee04-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ee04-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ee04-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ee04-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ee04-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ee04-172">Java</span><span class="sxs-lookup"><span data-stu-id="5ee04-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5ee04-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ee04-173">Response</span></span>

<span data-ttu-id="5ee04-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5ee04-174">The following is an example of the response.</span></span>

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

### <a name="example-4-create-an-accesspackageresourcerequest-for-adding-a-group-as-a-resource"></a><span data-ttu-id="5ee04-175">Exemplo 4: Criar um accessPackageResourceRequest para adicionar um grupo como um recurso</span><span class="sxs-lookup"><span data-stu-id="5ee04-175">Example 4: Create an accessPackageResourceRequest for adding a group as a resource</span></span>

#### <a name="request"></a><span data-ttu-id="5ee04-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee04-176">Request</span></span>

<span data-ttu-id="5ee04-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ee04-177">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5ee04-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ee04-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerequest_from_accesspackageresourcerequests4"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-type: application/json

{

  "catalogId":"beedadfe-01d5-4025-910b-84abb9369997",
  "requestType": "AdminAdd",
  "accessPackageResource": {
     "originId": "c6294667-7348-4f5a-be73-9d2c65f574f3",
     "originSystem": "AadGroup"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="5ee04-179">C#</span><span class="sxs-lookup"><span data-stu-id="5ee04-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ee04-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ee04-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ee04-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ee04-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ee04-182">Java</span><span class="sxs-lookup"><span data-stu-id="5ee04-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5ee04-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ee04-183">Response</span></span>

<span data-ttu-id="5ee04-184">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5ee04-184">The following is an example of the response.</span></span>

> <span data-ttu-id="5ee04-185">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5ee04-185">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "catalogId": "beedadfe-01d5-4025-910b-84abb9369997",
  "id": "acc2294e-f37f-42d3-981d-4e83847ed0ce",
  "requestType": "AdminAdd",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled"
}
```

### <a name="example-5-create-an-accesspackageresourcerequest-for-removing-a-resource"></a><span data-ttu-id="5ee04-186">Exemplo 5: Criar um accessPackageResourceRequest para remover um recurso</span><span class="sxs-lookup"><span data-stu-id="5ee04-186">Example 5: Create an accessPackageResourceRequest for removing a resource</span></span>

#### <a name="request"></a><span data-ttu-id="5ee04-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee04-187">Request</span></span>

<span data-ttu-id="5ee04-188">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ee04-188">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5ee04-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ee04-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerequest_from_accesspackageresourcerequests5"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-type: application/json

{
  "catalogId": "beedadfe-01d5-4025-910b-84abb9369997",
  "requestType": "AdminRemove",
  "accessPackageResource": {
    "id": "354078e5-dbce-4894-8af4-0ab274d41662"
  }
}

```
# <a name="c"></a>[<span data-ttu-id="5ee04-190">C#</span><span class="sxs-lookup"><span data-stu-id="5ee04-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ee04-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ee04-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ee04-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ee04-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests5-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ee04-193">Java</span><span class="sxs-lookup"><span data-stu-id="5ee04-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests5-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5ee04-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ee04-194">Response</span></span>

<span data-ttu-id="5ee04-195">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5ee04-195">The following is an example of the response.</span></span>

> <span data-ttu-id="5ee04-196">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5ee04-196">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "catalogId": "beedadfe-01d5-4025-910b-84abb9369997",
  "id": "65c3340d-defb-49a9-8930-63841fda0e68",
  "requestType": "AdminRemove",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled"
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
