---
title: Atualizar teamsApp
description: 'Atualize um aplicativo publicado anteriormente em um catálogo de aplicativos do teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e69a43182b0d96b146b080e7326560dc11ac3ed1
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223539"
---
# <a name="update-teamsapp"></a><span data-ttu-id="762ab-103">Atualizar teamsApp</span><span class="sxs-lookup"><span data-stu-id="762ab-103">Update teamsApp</span></span>

<span data-ttu-id="762ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="762ab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="762ab-105">Atualize um [aplicativo](../resources/teamsapp.md) publicado anteriormente no catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="762ab-105">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="762ab-106">Para atualizar um aplicativo, a propriedade **distributionMethod** para o aplicativo deve ser definida como `organization` .</span><span class="sxs-lookup"><span data-stu-id="762ab-106">To update an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="762ab-107">Essa API atualiza especificamente um aplicativo publicado no catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário).</span><span class="sxs-lookup"><span data-stu-id="762ab-107">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span>

## <a name="permissions"></a><span data-ttu-id="762ab-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="762ab-108">Permissions</span></span>

<span data-ttu-id="762ab-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="762ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="762ab-111">**Observação:** Somente os administradores globais podem chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="762ab-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="762ab-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="762ab-112">Permission Type</span></span>                        | <span data-ttu-id="762ab-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="762ab-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="762ab-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="762ab-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="762ab-115">AppCatalog. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="762ab-115">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="762ab-116">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="762ab-116">Delegated (work or school account)</span></span> | <span data-ttu-id="762ab-117">AppCatalog.Submit</span><span class="sxs-lookup"><span data-stu-id="762ab-117">AppCatalog.Submit</span></span>|
| <span data-ttu-id="762ab-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="762ab-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="762ab-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="762ab-119">Not supported</span></span>|
| <span data-ttu-id="762ab-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="762ab-120">Application</span></span>                            | <span data-ttu-id="762ab-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="762ab-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="762ab-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="762ab-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps/{id}/appDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="762ab-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="762ab-123">Request headers</span></span>

| <span data-ttu-id="762ab-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="762ab-124">Header</span></span>        | <span data-ttu-id="762ab-125">Valor</span><span class="sxs-lookup"><span data-stu-id="762ab-125">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="762ab-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="762ab-126">Authorization</span></span> | <span data-ttu-id="762ab-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="762ab-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="762ab-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="762ab-129">Content-Type</span></span>  | <span data-ttu-id="762ab-130">Application/zip.</span><span class="sxs-lookup"><span data-stu-id="762ab-130">application/zip.</span></span> <span data-ttu-id="762ab-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="762ab-131">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="762ab-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="762ab-132">Request body</span></span>

<span data-ttu-id="762ab-133">No corpo da solicitação, inclua uma carga de manifesto zip do teams.</span><span class="sxs-lookup"><span data-stu-id="762ab-133">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="762ab-134">Para obter detalhes, consulte [criar um pacote de aplicativos](/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="762ab-134">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="762ab-135">**Observação:** Use a ID retornada da chamada [lista de aplicativos publicados](./teamsapp-list.md) para fazer referência ao aplicativo que você deseja atualizar.</span><span class="sxs-lookup"><span data-stu-id="762ab-135">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call to reference the app you'd like to update.</span></span> <span data-ttu-id="762ab-136">Não use a ID do manifesto do pacote de aplicativos zip.</span><span class="sxs-lookup"><span data-stu-id="762ab-136">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="762ab-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="762ab-137">Response</span></span>

<span data-ttu-id="762ab-138">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="762ab-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="762ab-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="762ab-139">Examples</span></span>

### <a name="example-1-update-an-application-previously-published-to-the-microsoft-teams-app-catalog"></a><span data-ttu-id="762ab-140">Exemplo 1: atualizar um aplicativo publicado anteriormente no catálogo de aplicativos do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="762ab-140">Example 1: Update an application previously published to the Microsoft Teams app catalog</span></span>

### <a name="request"></a><span data-ttu-id="762ab-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="762ab-141">Request</span></span>

<!-- markdownlint-disable MD034 -->

# <a name="http"></a>[<span data-ttu-id="762ab-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="762ab-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_teamsapp"
}-->

```http
PUT https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```
# <a name="c"></a>[<span data-ttu-id="762ab-143">C#</span><span class="sxs-lookup"><span data-stu-id="762ab-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="762ab-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="762ab-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="762ab-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="762ab-145">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
