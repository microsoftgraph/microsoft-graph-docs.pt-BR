---
title: Atualizar teamsApp
description: 'Atualize um aplicativo publicado anteriormente em um catálogo de aplicativos do teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 64a7f6a5e7602f200a6b243669e1054f167f127b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964247"
---
# <a name="update-teamsapp"></a><span data-ttu-id="62b48-103">Atualizar teamsApp</span><span class="sxs-lookup"><span data-stu-id="62b48-103">Update teamsApp</span></span>

<span data-ttu-id="62b48-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62b48-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="62b48-105">Atualize um [aplicativo](../resources/teamsapp.md) publicado anteriormente no catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="62b48-105">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="62b48-106">Para atualizar um aplicativo, a propriedade **distributionMethod** para o aplicativo deve ser definida como `organization` .</span><span class="sxs-lookup"><span data-stu-id="62b48-106">To update an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="62b48-107">Essa API atualiza especificamente um aplicativo publicado no catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário).</span><span class="sxs-lookup"><span data-stu-id="62b48-107">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span>

## <a name="permissions"></a><span data-ttu-id="62b48-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="62b48-108">Permissions</span></span>

<span data-ttu-id="62b48-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62b48-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="62b48-111">**Observação:** Somente os administradores globais podem chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="62b48-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="62b48-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62b48-112">Permission Type</span></span>                        | <span data-ttu-id="62b48-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="62b48-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="62b48-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62b48-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="62b48-115">AppCatalog. Submit, AppCatalog. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="62b48-115">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="62b48-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62b48-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62b48-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="62b48-117">Not supported</span></span>|
| <span data-ttu-id="62b48-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62b48-118">Application</span></span>                            | <span data-ttu-id="62b48-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62b48-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="62b48-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62b48-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps/{id}/appDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="62b48-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62b48-121">Request headers</span></span>

| <span data-ttu-id="62b48-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="62b48-122">Header</span></span>        | <span data-ttu-id="62b48-123">Valor</span><span class="sxs-lookup"><span data-stu-id="62b48-123">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="62b48-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="62b48-124">Authorization</span></span> | <span data-ttu-id="62b48-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62b48-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="62b48-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="62b48-127">Content-Type</span></span>  | <span data-ttu-id="62b48-128">Application/zip.</span><span class="sxs-lookup"><span data-stu-id="62b48-128">application/zip.</span></span> <span data-ttu-id="62b48-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62b48-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62b48-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62b48-130">Request body</span></span>

<span data-ttu-id="62b48-131">No corpo da solicitação, inclua uma carga de manifesto zip do teams.</span><span class="sxs-lookup"><span data-stu-id="62b48-131">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="62b48-132">Para obter detalhes, consulte [criar um pacote de aplicativos](/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="62b48-132">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="62b48-133">**Observação:** Use a ID retornada da chamada [lista de aplicativos publicados](./teamsapp-list.md) para fazer referência ao aplicativo que você deseja atualizar.</span><span class="sxs-lookup"><span data-stu-id="62b48-133">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call to reference the app you'd like to update.</span></span> <span data-ttu-id="62b48-134">Não use a ID do manifesto do pacote de aplicativos zip.</span><span class="sxs-lookup"><span data-stu-id="62b48-134">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="62b48-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="62b48-135">Response</span></span>

<span data-ttu-id="62b48-136">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="62b48-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="62b48-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="62b48-137">Examples</span></span>

### <a name="example-1-update-an-application-previously-published-to-the-microsoft-teams-app-catalog"></a><span data-ttu-id="62b48-138">Exemplo 1: atualizar um aplicativo publicado anteriormente no catálogo de aplicativos do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="62b48-138">Example 1: Update an application previously published to the Microsoft Teams app catalog</span></span>

### <a name="request"></a><span data-ttu-id="62b48-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62b48-139">Request</span></span>

<!-- markdownlint-disable MD034 -->

# <a name="http"></a>[<span data-ttu-id="62b48-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="62b48-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="62b48-141">C#</span><span class="sxs-lookup"><span data-stu-id="62b48-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62b48-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62b48-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="62b48-143">Java</span><span class="sxs-lookup"><span data-stu-id="62b48-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="62b48-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="62b48-144">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
