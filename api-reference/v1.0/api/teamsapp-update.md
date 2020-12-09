---
title: Atualizar teamsApp
description: 'Atualize um aplicativo publicado anteriormente em um catálogo de aplicativos do teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0ca82b7d1f46722896529a53a0c12ced726a6525
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607158"
---
# <a name="update-teamsapp"></a><span data-ttu-id="082a6-103">Atualizar teamsApp</span><span class="sxs-lookup"><span data-stu-id="082a6-103">Update teamsApp</span></span>

<span data-ttu-id="082a6-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="082a6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="082a6-105">Atualize um [aplicativo](../resources/teamsapp.md) publicado anteriormente no catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="082a6-105">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="082a6-106">Para atualizar um aplicativo, a propriedade **distributionMethod** para o aplicativo deve ser definida como `organization` .</span><span class="sxs-lookup"><span data-stu-id="082a6-106">To update an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="082a6-107">Essa API atualiza especificamente um aplicativo publicado no catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário).</span><span class="sxs-lookup"><span data-stu-id="082a6-107">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span>

## <a name="permissions"></a><span data-ttu-id="082a6-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="082a6-108">Permissions</span></span>

<span data-ttu-id="082a6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="082a6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="082a6-111">**Observação:** Somente os administradores globais podem chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="082a6-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="082a6-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="082a6-112">Permission Type</span></span>                        | <span data-ttu-id="082a6-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="082a6-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="082a6-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="082a6-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="082a6-115">AppCatalog. Submit, AppCatalog. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="082a6-115">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="082a6-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="082a6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="082a6-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="082a6-117">Not supported</span></span>|
| <span data-ttu-id="082a6-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="082a6-118">Application</span></span>                            | <span data-ttu-id="082a6-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="082a6-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="082a6-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="082a6-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps/{id}/appDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="082a6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="082a6-121">Request headers</span></span>

| <span data-ttu-id="082a6-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="082a6-122">Header</span></span>        | <span data-ttu-id="082a6-123">Valor</span><span class="sxs-lookup"><span data-stu-id="082a6-123">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="082a6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="082a6-124">Authorization</span></span> | <span data-ttu-id="082a6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="082a6-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="082a6-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="082a6-127">Content-Type</span></span>  | <span data-ttu-id="082a6-128">Application/zip.</span><span class="sxs-lookup"><span data-stu-id="082a6-128">application/zip.</span></span> <span data-ttu-id="082a6-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="082a6-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="082a6-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="082a6-130">Request body</span></span>

<span data-ttu-id="082a6-131">No corpo da solicitação, inclua uma carga de manifesto zip do teams.</span><span class="sxs-lookup"><span data-stu-id="082a6-131">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="082a6-132">Para obter detalhes, consulte [criar um pacote de aplicativos](/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="082a6-132">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="082a6-133">**Observação:** Use a ID retornada da chamada [lista de aplicativos publicados](./appcatalogs-list-teamsapps.md) para fazer referência ao aplicativo que você deseja atualizar.</span><span class="sxs-lookup"><span data-stu-id="082a6-133">**Note:** Use the ID returned from the [List published apps](./appcatalogs-list-teamsapps.md) call to reference the app you'd like to update.</span></span> <span data-ttu-id="082a6-134">Não use a ID do manifesto do pacote de aplicativos zip.</span><span class="sxs-lookup"><span data-stu-id="082a6-134">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="082a6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="082a6-135">Response</span></span>

<span data-ttu-id="082a6-136">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="082a6-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="082a6-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="082a6-137">Examples</span></span>

### <a name="example-1-update-an-application-previously-published-to-the-microsoft-teams-app-catalog"></a><span data-ttu-id="082a6-138">Exemplo 1: atualizar um aplicativo publicado anteriormente no catálogo de aplicativos do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="082a6-138">Example 1: Update an application previously published to the Microsoft Teams app catalog</span></span>

### <a name="request"></a><span data-ttu-id="082a6-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="082a6-139">Request</span></span>

<!-- markdownlint-disable MD034 -->

# <a name="http"></a>[<span data-ttu-id="082a6-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="082a6-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="082a6-141">C#</span><span class="sxs-lookup"><span data-stu-id="082a6-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="082a6-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="082a6-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="082a6-143">Java</span><span class="sxs-lookup"><span data-stu-id="082a6-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="082a6-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="082a6-144">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
