---
title: Listar teamsApp
description: Listar aplicativos do teams publicados no catálogo de aplicativos do locatário.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 35a922e2ed7fd3ccd4c41d19173199d243bb3192
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690342"
---
# <a name="list-teamsapp"></a><span data-ttu-id="c89d5-103">Listar teamsApp</span><span class="sxs-lookup"><span data-stu-id="c89d5-103">List teamsApp</span></span>

<span data-ttu-id="c89d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c89d5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c89d5-105">Listar [aplicativos](../resources/teamsapp.md) publicados no catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c89d5-105">List [apps](../resources/teamsapp.md) published in the Microsoft Teams app catalog.</span></span> <span data-ttu-id="c89d5-106">Isso inclui os aplicativos do Microsoft Teams Store, bem como os aplicativos do catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário).</span><span class="sxs-lookup"><span data-stu-id="c89d5-106">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="c89d5-107">Para obter aplicativos apenas do catálogo de aplicativos da sua organização, especifique `organization` como **distributionMethod** na solicitação.</span><span class="sxs-lookup"><span data-stu-id="c89d5-107">To get apps from your organization's app catalog only, specify `organization` as the **distributionMethod** in the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="c89d5-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="c89d5-108">Permissions</span></span>

<span data-ttu-id="c89d5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c89d5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> <span data-ttu-id="c89d5-111">**Observação:** Somente os administradores globais podem chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="c89d5-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="c89d5-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c89d5-112">Permission Type</span></span>                        | <span data-ttu-id="c89d5-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c89d5-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="c89d5-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c89d5-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="c89d5-115">AppCatalog. Read. All, AppCatalog. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c89d5-115">AppCatalog.Read.All, AppCatalog.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="c89d5-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c89d5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c89d5-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c89d5-117">Not supported</span></span>                       |
| <span data-ttu-id="c89d5-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c89d5-118">Application</span></span>                            | <span data-ttu-id="c89d5-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c89d5-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c89d5-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c89d5-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c89d5-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c89d5-121">Optional query parameters</span></span>

<span data-ttu-id="c89d5-122">Este método suporta o `$filter`, `$select`, e `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c89d5-122">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="c89d5-123">O uso `$expand=AppDefinitions` retornará mais informações sobre o estado do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c89d5-123">Using `$expand=AppDefinitions` will return more information about the state of the app.</span></span> 

> <span data-ttu-id="c89d5-124">**Observação:** Você pode filtrar em qualquer um dos campos do objeto [teamsApp](../resources/teamsapp.md) para diminuir a lista de resultados.</span><span class="sxs-lookup"><span data-stu-id="c89d5-124">**Note:** You can filter on any of the fields of the [teamsApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="c89d5-125">Você pode usar qualquer uma das seguintes operações de filtro: igual, não igual, e, ou, e não.</span><span class="sxs-lookup"><span data-stu-id="c89d5-125">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c89d5-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c89d5-126">Request headers</span></span>

| <span data-ttu-id="c89d5-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c89d5-127">Header</span></span>        | <span data-ttu-id="c89d5-128">Valor</span><span class="sxs-lookup"><span data-stu-id="c89d5-128">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="c89d5-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="c89d5-129">Authorization</span></span> | <span data-ttu-id="c89d5-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c89d5-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c89d5-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c89d5-132">Request body</span></span>

<span data-ttu-id="c89d5-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c89d5-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c89d5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c89d5-134">Response</span></span>

<span data-ttu-id="c89d5-135">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma lista de objetos [teamsApp](../resources/teamsapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c89d5-135">If successful, this method returns a `200 OK` response code and a list of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c89d5-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c89d5-136">Examples</span></span>

### <a name="example-1-list-all-applications-specific-to-the-tenant"></a><span data-ttu-id="c89d5-137">Exemplo 1: listar todos os aplicativos específicos para o locatário</span><span class="sxs-lookup"><span data-stu-id="c89d5-137">Example 1: List all applications specific to the tenant</span></span>

<span data-ttu-id="c89d5-138">O exemplo a seguir lista todos os aplicativos específicos do seu locatário.</span><span class="sxs-lookup"><span data-stu-id="c89d5-138">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="c89d5-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c89d5-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c89d5-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c89d5-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapps_filter_distributionMethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```
# <a name="c"></a>[<span data-ttu-id="c89d5-141">C#</span><span class="sxs-lookup"><span data-stu-id="c89d5-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapps-filter-distributionmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c89d5-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c89d5-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapps-filter-distributionmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c89d5-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c89d5-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapps-filter-distributionmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c89d5-144">Java</span><span class="sxs-lookup"><span data-stu-id="c89d5-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapps-filter-distributionmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="c89d5-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="c89d5-145">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="c89d5-146">Exemplo 2: listar aplicativos com uma determinada ID</span><span class="sxs-lookup"><span data-stu-id="c89d5-146">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="c89d5-147">O exemplo a seguir lista os aplicativos com uma determinada ID.</span><span class="sxs-lookup"><span data-stu-id="c89d5-147">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="c89d5-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c89d5-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c89d5-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="c89d5-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp_filter_id"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```
# <a name="c"></a>[<span data-ttu-id="c89d5-150">C#</span><span class="sxs-lookup"><span data-stu-id="c89d5-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-filter-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c89d5-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c89d5-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-filter-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c89d5-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c89d5-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-filter-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c89d5-153">Java</span><span class="sxs-lookup"><span data-stu-id="c89d5-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapp-filter-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c89d5-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="c89d5-154">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```
### <a name="example-3-find-application-based-on-the-teams-app-manifest-id"></a><span data-ttu-id="c89d5-155">Exemplo 3: localizar o aplicativo com base na ID de manifesto do aplicativo Teams.</span><span class="sxs-lookup"><span data-stu-id="c89d5-155">Example 3: Find application based on the Teams app manifest ID.</span></span>

<span data-ttu-id="c89d5-156">O exemplo a seguir lista os aplicativos que correspondem ao ' ID ' especificado no manifesto do aplicativo Teams.</span><span class="sxs-lookup"><span data-stu-id="c89d5-156">The following example lists applications that match the 'id' specified in the Teams app manifest.</span></span> <span data-ttu-id="c89d5-157">No exemplo, a ID de manifesto do aplicativo Teams é 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'.</span><span class="sxs-lookup"><span data-stu-id="c89d5-157">In the example, the manifest ID of the Teams app is 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'.</span></span>

#### <a name="request"></a><span data-ttu-id="c89d5-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c89d5-158">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c89d5-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="c89d5-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp_filter_externalid"
}-->

```msgraph-interactive
GET  https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'
```
# <a name="c"></a>[<span data-ttu-id="c89d5-160">C#</span><span class="sxs-lookup"><span data-stu-id="c89d5-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-filter-externalid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c89d5-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c89d5-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-filter-externalid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c89d5-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c89d5-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-filter-externalid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c89d5-163">Java</span><span class="sxs-lookup"><span data-stu-id="c89d5-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapp-filter-externalid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c89d5-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="c89d5-164">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#appCatalogs/teamsApps",
    "value": [
        {
            "id": "22f73bbe-f67a-4dea-bd54-54cac718cb2b",
            "externalId": "cf1ba4c7-f94e-4d80-ba90-5594b641a8ee",
            "displayName": "YPA",
            "distributionMethod": "organization"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="c89d5-165">Confira também</span><span class="sxs-lookup"><span data-stu-id="c89d5-165">See also</span></span>

- [<span data-ttu-id="c89d5-166">Listar aplicativos instalados em uma equipe</span><span class="sxs-lookup"><span data-stu-id="c89d5-166">List apps installed in a team</span></span>](team-list-installedapps.md)
- [<span data-ttu-id="c89d5-167">Listar aplicativos instalados no escopo pessoal de um usuário</span><span class="sxs-lookup"><span data-stu-id="c89d5-167">List apps installed in the personal scope of a user</span></span>](userteamwork-list-installedapps.md)

