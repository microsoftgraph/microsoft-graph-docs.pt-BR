---
title: Listar teamsApp
description: 'Listar aplicativos do catálogo de aplicativos do Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b1572581cedc6e1c3fe87f4402e51c69c9b2c5dc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076646"
---
# <a name="list-teamsapp"></a><span data-ttu-id="dbe37-103">Listar teamsApp</span><span class="sxs-lookup"><span data-stu-id="dbe37-103">List teamsApp</span></span>

<span data-ttu-id="dbe37-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbe37-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbe37-105">Listar [aplicativos](../resources/teamsapp.md) do catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="dbe37-105">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="dbe37-106">Isso inclui os aplicativos do Microsoft Teams Store, bem como os aplicativos do catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário).</span><span class="sxs-lookup"><span data-stu-id="dbe37-106">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="dbe37-107">Para obter aplicativos apenas do catálogo de aplicativos da sua organização, especifique `organization` como **distributionMethod** na solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbe37-107">To get apps from your organization's app catalog only, specify `organization` as the **distributionMethod** in the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbe37-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="dbe37-108">Permissions</span></span>

<span data-ttu-id="dbe37-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbe37-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dbe37-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbe37-111">Permission Type</span></span>                        | <span data-ttu-id="dbe37-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dbe37-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="dbe37-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbe37-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="dbe37-114">AppCatalog. Read. All, AppCatalog. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="dbe37-114">AppCatalog.Read.All, AppCatalog.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="dbe37-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbe37-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbe37-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dbe37-116">Not supported</span></span>                       |
| <span data-ttu-id="dbe37-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbe37-117">Application</span></span>                            | <span data-ttu-id="dbe37-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbe37-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbe37-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbe37-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dbe37-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dbe37-120">Optional query parameters</span></span>

<span data-ttu-id="dbe37-121">Este método suporta o `$filter`, `$select`, e `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dbe37-121">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="dbe37-122">`$expand=AppDefinitions`O uso retornará mais informações sobre o estado do aplicativo, como o **publishingstate**, que reflete o status de análise de envio de aplicativos e retorna se um aplicativo foi aprovado, rejeitado ou permanece em revisão.</span><span class="sxs-lookup"><span data-stu-id="dbe37-122">Using `$expand=AppDefinitions` will return more information about the state of the app, such as the **publishingState**, which reflects the app submission review status and returns whether an app has been approved, rejected, or remains under review.</span></span> 

> <span data-ttu-id="dbe37-123">**Observação:** Você pode filtrar em qualquer um dos campos do objeto [teamsApp](../resources/teamsapp.md) para diminuir a lista de resultados.</span><span class="sxs-lookup"><span data-stu-id="dbe37-123">**Note:** You can filter on any of the fields of the [teamsApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="dbe37-124">Você pode usar qualquer uma das seguintes operações de filtro: igual, não igual, e, ou, e não.</span><span class="sxs-lookup"><span data-stu-id="dbe37-124">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dbe37-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbe37-125">Request headers</span></span>

| <span data-ttu-id="dbe37-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dbe37-126">Header</span></span>        | <span data-ttu-id="dbe37-127">Valor</span><span class="sxs-lookup"><span data-stu-id="dbe37-127">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="dbe37-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbe37-128">Authorization</span></span> | <span data-ttu-id="dbe37-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbe37-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dbe37-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbe37-131">Request body</span></span>

<span data-ttu-id="dbe37-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dbe37-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbe37-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbe37-133">Response</span></span>

<span data-ttu-id="dbe37-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma lista de objetos [teamsApp](../resources/teamsapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbe37-134">If successful, this method returns a `200 OK` response code and a list of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dbe37-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dbe37-135">Examples</span></span>

### <a name="example-1-list-all-applications-in-a-tenant"></a><span data-ttu-id="dbe37-136">Exemplo 1: listar todos os aplicativos em um locatário</span><span class="sxs-lookup"><span data-stu-id="dbe37-136">Example 1: List all applications in a tenant</span></span>

<span data-ttu-id="dbe37-137">O exemplo a seguir lista todos os aplicativos específicos do seu locatário.</span><span class="sxs-lookup"><span data-stu-id="dbe37-137">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="dbe37-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbe37-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="dbe37-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="dbe37-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```
# <a name="c"></a>[<span data-ttu-id="dbe37-140">C#</span><span class="sxs-lookup"><span data-stu-id="dbe37-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dbe37-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dbe37-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dbe37-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dbe37-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="dbe37-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbe37-143">Response</span></span>

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

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="dbe37-144">Exemplo 2: listar aplicativos com uma determinada ID</span><span class="sxs-lookup"><span data-stu-id="dbe37-144">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="dbe37-145">O exemplo a seguir lista os aplicativos com uma determinada ID.</span><span class="sxs-lookup"><span data-stu-id="dbe37-145">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="dbe37-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbe37-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="dbe37-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="dbe37-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```
# <a name="c"></a>[<span data-ttu-id="dbe37-148">C#</span><span class="sxs-lookup"><span data-stu-id="dbe37-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dbe37-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dbe37-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dbe37-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dbe37-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dbe37-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbe37-151">Response</span></span>

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

### <a name="example-3-list-applications-with-a-given-id-and-return-the-submission-review-state"></a><span data-ttu-id="dbe37-152">Exemplo 3: listar aplicativos com uma determinada ID e retornar o estado de revisão de envio</span><span class="sxs-lookup"><span data-stu-id="dbe37-152">Example 3: List applications with a given ID, and return the submission review state</span></span>

<span data-ttu-id="dbe37-153">O exemplo a seguir lista os aplicativos com uma determinada ID e expande **appDefinitions** para retornar o **publishingstate**, que reflete o estado de análise de envio do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dbe37-153">The following example lists applications with a given ID, and expands **appDefinitions** to return the **publishingState**, which reflects the app's submission review state.</span></span> <span data-ttu-id="dbe37-154">`Submitted` significa que a revisão está pendente, `published` significa que o aplicativo foi aprovado pelo administrador e `rejected` significa que o aplicativo foi rejeitado pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="dbe37-154">`Submitted` means the review is pending, `published` means the app was approved by the admin, and `rejected` means the app was rejected by the admin.</span></span>

#### <a name="request"></a><span data-ttu-id="dbe37-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbe37-155">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="dbe37-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="dbe37-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```msgraph-interactive
GET  https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id eq '876df28f-2e78-423b-94a5-44181bd0e225'&$expand=appDefinitions
```
# <a name="c"></a>[<span data-ttu-id="dbe37-157">C#</span><span class="sxs-lookup"><span data-stu-id="dbe37-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dbe37-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dbe37-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dbe37-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dbe37-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dbe37-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbe37-160">Response</span></span>

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


