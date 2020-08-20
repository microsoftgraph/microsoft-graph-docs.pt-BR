---
title: Listar teamsApp
description: 'Listar aplicativos do catálogo de aplicativos do Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c0948dcc2545a30480188741e1ca622c9acbde35
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819979"
---
# <a name="list-teamsapp"></a><span data-ttu-id="67f8a-103">Listar teamsApp</span><span class="sxs-lookup"><span data-stu-id="67f8a-103">List teamsApp</span></span>

<span data-ttu-id="67f8a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67f8a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67f8a-105">Listar [aplicativos](../resources/teamsapp.md) do catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="67f8a-105">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="67f8a-106">Isso inclui os aplicativos do Microsoft Teams Store, bem como os aplicativos do catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário).</span><span class="sxs-lookup"><span data-stu-id="67f8a-106">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="67f8a-107">Para obter aplicativos apenas do catálogo de aplicativos da sua organização, especifique `organization` como **distributionMethod** na solicitação.</span><span class="sxs-lookup"><span data-stu-id="67f8a-107">To get apps from your organization's app catalog only, specify `organization` as the **distributionMethod** in the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="67f8a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="67f8a-108">Permissions</span></span>

<span data-ttu-id="67f8a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67f8a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="67f8a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67f8a-111">Permission Type</span></span>                        | <span data-ttu-id="67f8a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="67f8a-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="67f8a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67f8a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="67f8a-114">AppCatalog. Read. All, AppCatalog. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="67f8a-114">AppCatalog.Read.All, AppCatalog.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="67f8a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67f8a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67f8a-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="67f8a-116">Not supported</span></span>                       |
| <span data-ttu-id="67f8a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67f8a-117">Application</span></span>                            | <span data-ttu-id="67f8a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67f8a-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="67f8a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67f8a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="67f8a-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="67f8a-120">Optional query parameters</span></span>

<span data-ttu-id="67f8a-121">Este método suporta o `$filter`, `$select`, e `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="67f8a-121">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="67f8a-122">`$expand=AppDefinitions`O uso retornará mais informações sobre o estado do aplicativo, como o **publishingstate**, que reflete o status de análise de envio de aplicativos e retorna se um aplicativo foi aprovado, rejeitado ou permanece em revisão.</span><span class="sxs-lookup"><span data-stu-id="67f8a-122">Using `$expand=AppDefinitions` will return more information about the state of the app, such as the **publishingState**, which reflects the app submission review status and returns whether an app has been approved, rejected, or remains under review.</span></span> 

> <span data-ttu-id="67f8a-123">**Observação:** Você pode filtrar em qualquer um dos campos do objeto [teamsApp](../resources/teamsapp.md) para diminuir a lista de resultados.</span><span class="sxs-lookup"><span data-stu-id="67f8a-123">**Note:** You can filter on any of the fields of the [teamsApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="67f8a-124">Você pode usar qualquer uma das seguintes operações de filtro: igual, não igual, e, ou, e não.</span><span class="sxs-lookup"><span data-stu-id="67f8a-124">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="request-headers"></a><span data-ttu-id="67f8a-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67f8a-125">Request headers</span></span>

| <span data-ttu-id="67f8a-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67f8a-126">Header</span></span>        | <span data-ttu-id="67f8a-127">Valor</span><span class="sxs-lookup"><span data-stu-id="67f8a-127">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="67f8a-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="67f8a-128">Authorization</span></span> | <span data-ttu-id="67f8a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67f8a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67f8a-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67f8a-131">Request body</span></span>

<span data-ttu-id="67f8a-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="67f8a-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67f8a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="67f8a-133">Response</span></span>

<span data-ttu-id="67f8a-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma lista de objetos [teamsApp](../resources/teamsapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67f8a-134">If successful, this method returns a `200 OK` response code and a list of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="67f8a-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="67f8a-135">Examples</span></span>

### <a name="example-1-list-all-applications-in-a-tenant"></a><span data-ttu-id="67f8a-136">Exemplo 1: listar todos os aplicativos em um locatário</span><span class="sxs-lookup"><span data-stu-id="67f8a-136">Example 1: List all applications in a tenant</span></span>

<span data-ttu-id="67f8a-137">O exemplo a seguir lista todos os aplicativos específicos do seu locatário.</span><span class="sxs-lookup"><span data-stu-id="67f8a-137">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="67f8a-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67f8a-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="67f8a-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="67f8a-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```
# <a name="c"></a>[<span data-ttu-id="67f8a-140">C#</span><span class="sxs-lookup"><span data-stu-id="67f8a-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67f8a-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67f8a-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67f8a-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67f8a-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="67f8a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="67f8a-143">Response</span></span>

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

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="67f8a-144">Exemplo 2: listar aplicativos com uma determinada ID</span><span class="sxs-lookup"><span data-stu-id="67f8a-144">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="67f8a-145">O exemplo a seguir lista os aplicativos com uma determinada ID.</span><span class="sxs-lookup"><span data-stu-id="67f8a-145">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="67f8a-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67f8a-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="67f8a-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="67f8a-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```
# <a name="c"></a>[<span data-ttu-id="67f8a-148">C#</span><span class="sxs-lookup"><span data-stu-id="67f8a-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67f8a-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67f8a-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67f8a-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67f8a-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="67f8a-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="67f8a-151">Response</span></span>

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

### <a name="example-3-list-applications-with-a-given-id-and-return-the-submission-review-state"></a><span data-ttu-id="67f8a-152">Exemplo 3: listar aplicativos com uma determinada ID e retornar o estado de revisão de envio</span><span class="sxs-lookup"><span data-stu-id="67f8a-152">Example 3: List applications with a given ID, and return the submission review state</span></span>

<span data-ttu-id="67f8a-153">O exemplo a seguir lista os aplicativos com uma determinada ID e expande **appDefinitions** para retornar o **publishingstate**, que reflete o estado de análise de envio do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="67f8a-153">The following example lists applications with a given ID, and expands **appDefinitions** to return the **publishingState**, which reflects the app's submission review state.</span></span> <span data-ttu-id="67f8a-154">`Submitted` significa que a revisão está pendente, `published` significa que o aplicativo foi aprovado pelo administrador e `rejected` significa que o aplicativo foi rejeitado pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="67f8a-154">`Submitted` means the review is pending, `published` means the app was approved by the admin, and `rejected` means the app was rejected by the admin.</span></span>

#### <a name="request"></a><span data-ttu-id="67f8a-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67f8a-155">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="67f8a-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="67f8a-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```msgraph-interactive
GET  https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id eq '876df28f-2e78-423b-94a5-44181bd0e225'&$expand=appDefinitions
```
# <a name="c"></a>[<span data-ttu-id="67f8a-157">C#</span><span class="sxs-lookup"><span data-stu-id="67f8a-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67f8a-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67f8a-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67f8a-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67f8a-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="67f8a-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="67f8a-160">Response</span></span>

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
      "id": "876df28f-2e78-423b-94a5-44181bd0e225",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization",
      "appDefinitions": [
                {

                    "id": "NGQyMGNiNDUtZWViYS00ZTEyLWE3YzktMGQ0NDgzYjYxNzU2IyMxLjAuMA==",

                    "teamsAppId": "876df28f-2e78-423b-94a5-44181bd0e225",

                    "azureADAppId": null,

                    "displayName": "Test App",

                    "version": "1.0.1",

                    "requiredResourceSpecificApplicationPermissions": [],

                    "publishingState": "published"

                  }
            ]
      }
    ]
  }
```
