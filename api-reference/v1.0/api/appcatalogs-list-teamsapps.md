---
title: Listar teamsApp
description: Listar aplicativos do teams publicados no catálogo de aplicativos do locatário.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fa54d1ac1eec5dfc0a6995f85ced9f46fa8d47ae
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607307"
---
# <a name="list-teamsapp"></a><span data-ttu-id="409a1-103">Listar teamsApp</span><span class="sxs-lookup"><span data-stu-id="409a1-103">List teamsApp</span></span>

<span data-ttu-id="409a1-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="409a1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="409a1-105">Listar [aplicativos](../resources/teamsapp.md) publicados no catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="409a1-105">List [apps](../resources/teamsapp.md) published in the Microsoft Teams app catalog.</span></span> <span data-ttu-id="409a1-106">Isso inclui os aplicativos do Microsoft Teams Store, bem como os aplicativos do catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário).</span><span class="sxs-lookup"><span data-stu-id="409a1-106">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="409a1-107">Para obter aplicativos apenas do catálogo de aplicativos da sua organização, especifique `organization` como **distributionMethod** na solicitação.</span><span class="sxs-lookup"><span data-stu-id="409a1-107">To get apps from your organization's app catalog only, specify `organization` as the **distributionMethod** in the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="409a1-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="409a1-108">Permissions</span></span>

<span data-ttu-id="409a1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="409a1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> <span data-ttu-id="409a1-111">**Observação:** Somente os administradores globais podem chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="409a1-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="409a1-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="409a1-112">Permission Type</span></span>                        | <span data-ttu-id="409a1-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="409a1-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="409a1-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="409a1-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="409a1-115">AppCatalog. Read. All, AppCatalog. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="409a1-115">AppCatalog.Read.All, AppCatalog.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="409a1-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="409a1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="409a1-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="409a1-117">Not supported</span></span>                       |
| <span data-ttu-id="409a1-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="409a1-118">Application</span></span>                            | <span data-ttu-id="409a1-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="409a1-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="409a1-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="409a1-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="409a1-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="409a1-121">Optional query parameters</span></span>

<span data-ttu-id="409a1-122">Este método suporta o `$filter`, `$select`, e `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="409a1-122">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="409a1-123">O uso `$expand=AppDefinitions` retornará mais informações sobre o estado do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="409a1-123">Using `$expand=AppDefinitions` will return more information about the state of the app.</span></span> 

> <span data-ttu-id="409a1-124">**Observação:** Você pode filtrar em qualquer um dos campos do objeto [teamsApp](../resources/teamsapp.md) para diminuir a lista de resultados.</span><span class="sxs-lookup"><span data-stu-id="409a1-124">**Note:** You can filter on any of the fields of the [teamsApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="409a1-125">Você pode usar qualquer uma das seguintes operações de filtro: igual, não igual, e, ou, e não.</span><span class="sxs-lookup"><span data-stu-id="409a1-125">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="request-headers"></a><span data-ttu-id="409a1-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="409a1-126">Request headers</span></span>

| <span data-ttu-id="409a1-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="409a1-127">Header</span></span>        | <span data-ttu-id="409a1-128">Valor</span><span class="sxs-lookup"><span data-stu-id="409a1-128">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="409a1-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="409a1-129">Authorization</span></span> | <span data-ttu-id="409a1-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="409a1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="409a1-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="409a1-132">Request body</span></span>

<span data-ttu-id="409a1-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="409a1-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="409a1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="409a1-134">Response</span></span>

<span data-ttu-id="409a1-135">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma lista de objetos [teamsApp](../resources/teamsapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="409a1-135">If successful, this method returns a `200 OK` response code and a list of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="409a1-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="409a1-136">Examples</span></span>

### <a name="example-1-list-all-applications-specific-to-the-tenant"></a><span data-ttu-id="409a1-137">Exemplo 1: listar todos os aplicativos específicos para o locatário</span><span class="sxs-lookup"><span data-stu-id="409a1-137">Example 1: List all applications specific to the tenant</span></span>

<span data-ttu-id="409a1-138">O exemplo a seguir lista todos os aplicativos específicos do seu locatário.</span><span class="sxs-lookup"><span data-stu-id="409a1-138">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="409a1-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="409a1-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_teamsapps_filter_distributionMethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```



<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="409a1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="409a1-140">Response</span></span>

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

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="409a1-141">Exemplo 2: listar aplicativos com uma determinada ID</span><span class="sxs-lookup"><span data-stu-id="409a1-141">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="409a1-142">O exemplo a seguir lista os aplicativos com uma determinada ID.</span><span class="sxs-lookup"><span data-stu-id="409a1-142">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="409a1-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="409a1-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_teamsapp_filter_id"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="409a1-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="409a1-144">Response</span></span>

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
### <a name="example-3-find-application-based-on-the-teams-app-manifest-id"></a><span data-ttu-id="409a1-145">Exemplo 3: localizar o aplicativo com base na ID de manifesto do aplicativo Teams.</span><span class="sxs-lookup"><span data-stu-id="409a1-145">Example 3: Find application based on the Teams app manifest ID.</span></span>

<span data-ttu-id="409a1-146">O exemplo a seguir lista os aplicativos que correspondem ao ' ID ' especificado no manifesto do aplicativo Teams.</span><span class="sxs-lookup"><span data-stu-id="409a1-146">The following example lists applications that match the 'id' specified in the Teams app manifest.</span></span> <span data-ttu-id="409a1-147">No exemplo, a ID de manifesto do aplicativo Teams é ' cf1ba4c7-f94e-4d80-ba90-5594b641a8ee '.</span><span class="sxs-lookup"><span data-stu-id="409a1-147">In the example, the manifest ID of the Teams app is 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'.</span></span>

#### <a name="request"></a><span data-ttu-id="409a1-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="409a1-148">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_teamsapp_filter_externalid"
}-->

```msgraph-interactive
GET  https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'
```

#### <a name="response"></a><span data-ttu-id="409a1-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="409a1-149">Response</span></span>

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

## <a name="see-also"></a><span data-ttu-id="409a1-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="409a1-150">See also</span></span>

- [<span data-ttu-id="409a1-151">Listar aplicativos instalados em uma equipe</span><span class="sxs-lookup"><span data-stu-id="409a1-151">List apps installed in a team</span></span>](team-list-installedapps.md)
- [<span data-ttu-id="409a1-152">Listar aplicativos instalados no escopo pessoal de um usuário</span><span class="sxs-lookup"><span data-stu-id="409a1-152">List apps installed in the personal scope of a user</span></span>](userteamwork-list-installedapps.md)

