---
title: Atualizar teamsApp
description: 'Atualize um aplicativo publicado anteriormente no catálogo de aplicativos do Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c1eb3382053c20e210bd87f96a2bb1bc688f90c2
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848392"
---
# <a name="update-teamsapp"></a><span data-ttu-id="33df1-103">Atualizar teamsApp</span><span class="sxs-lookup"><span data-stu-id="33df1-103">Update teamsApp</span></span>

<span data-ttu-id="33df1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33df1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33df1-105">Atualize um [aplicativo](../resources/teamsapp.md) publicado anteriormente no catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="33df1-105">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="33df1-106">Para atualizar um aplicativo, a propriedade **distributionMethod** para o aplicativo deve ser definida como `organization` .</span><span class="sxs-lookup"><span data-stu-id="33df1-106">To update an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="33df1-107">Essa API atualiza especificamente um aplicativo publicado no catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário).</span><span class="sxs-lookup"><span data-stu-id="33df1-107">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span>  

## <a name="permissions"></a><span data-ttu-id="33df1-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="33df1-108">Permissions</span></span>

<span data-ttu-id="33df1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33df1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="33df1-111">**Observação:** Somente os administradores globais podem chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="33df1-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="33df1-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33df1-112">Permission Type</span></span>                        | <span data-ttu-id="33df1-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="33df1-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="33df1-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33df1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="33df1-115">AppCatalog. Submit, AppCatalog. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="33df1-115">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="33df1-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33df1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33df1-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="33df1-117">Not supported</span></span>|
| <span data-ttu-id="33df1-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33df1-118">Application</span></span>                            | <span data-ttu-id="33df1-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33df1-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="33df1-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33df1-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps/{id}/appDefinitions
```

## <a name="query-parameters"></a><span data-ttu-id="33df1-121">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="33df1-121">Query parameters</span></span>

|<span data-ttu-id="33df1-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33df1-122">Property</span></span>|<span data-ttu-id="33df1-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="33df1-123">Type</span></span>|<span data-ttu-id="33df1-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="33df1-124">Description</span></span>|
|----|----|----|
|<span data-ttu-id="33df1-125">requiresReview</span><span class="sxs-lookup"><span data-stu-id="33df1-125">requiresReview</span></span>| <span data-ttu-id="33df1-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="33df1-126">Boolean</span></span> | <span data-ttu-id="33df1-127">Esse parâmetro de consulta opcional dispara o processo de revisão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="33df1-127">This optional query parameter triggers the app review process.</span></span> <span data-ttu-id="33df1-128">Os usuários com privilégios de administrador podem enviar aplicativos sem disparar uma revisão.</span><span class="sxs-lookup"><span data-stu-id="33df1-128">Users with admin privileges can submit apps without triggering a review.</span></span> <span data-ttu-id="33df1-129">Se os usuários desejarem solicitar uma revisão antes da publicação, eles devem  `requiresReview` ser definidos como `true` .</span><span class="sxs-lookup"><span data-stu-id="33df1-129">If users want to request a review before publishing, they must set  `requiresReview` to `true`.</span></span> <span data-ttu-id="33df1-130">Um usuário com privilégios de administrador pode optar por não definir `requiresReview` ou definir o valor como `false`  e o aplicativo será considerado aprovado e publicar instantaneamente.</span><span class="sxs-lookup"><span data-stu-id="33df1-130">A user who has admin privileges can opt not to set `requiresReview` or set the value to `false`  and the app will be considered approved and will publish instantly.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="33df1-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33df1-131">Request headers</span></span>

| <span data-ttu-id="33df1-132">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="33df1-132">Header</span></span>        | <span data-ttu-id="33df1-133">Valor</span><span class="sxs-lookup"><span data-stu-id="33df1-133">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="33df1-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="33df1-134">Authorization</span></span> | <span data-ttu-id="33df1-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33df1-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="33df1-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="33df1-137">Content-Type</span></span>  | <span data-ttu-id="33df1-138">Application/zip.</span><span class="sxs-lookup"><span data-stu-id="33df1-138">application/zip.</span></span> <span data-ttu-id="33df1-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33df1-139">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33df1-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33df1-140">Request body</span></span>

<span data-ttu-id="33df1-141">No corpo da solicitação, inclua uma carga de manifesto zip do teams.</span><span class="sxs-lookup"><span data-stu-id="33df1-141">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="33df1-142">Para obter detalhes, consulte [criar um pacote de aplicativos](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="33df1-142">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

><span data-ttu-id="33df1-143">**Observação:** Use o ID retornado da [lista de aplicativos publicados](./teamsapp-list.md) chamada para fazer referência ao aplicativo que você deseja atualizar.</span><span class="sxs-lookup"><span data-stu-id="33df1-143">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="33df1-144">Não use a ID do manifesto do pacote de aplicativos zip.</span><span class="sxs-lookup"><span data-stu-id="33df1-144">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="33df1-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="33df1-145">Response</span></span>

<span data-ttu-id="33df1-146">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="33df1-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="33df1-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="33df1-147">Examples</span></span>

### <a name="example-1-update-an-application-previously-published-to-the-microsoft-teams-app-catalog"></a><span data-ttu-id="33df1-148">Exemplo 1: atualizar um aplicativo publicado anteriormente no catálogo de aplicativos do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="33df1-148">Example 1: Update an application previously published to the Microsoft Teams app catalog</span></span>

### <a name="request"></a><span data-ttu-id="33df1-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33df1-149">Request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8/appDefinitions
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="33df1-150">Para obter detalhes sobre o arquivo zip do aplicativo do Teams, consulte [create app Package](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="33df1-150">For details about the Teams application zip file, see [Create app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>
<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="33df1-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="33df1-151">Response</span></span>

<span data-ttu-id="33df1-152">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="33df1-152">If successful, this method returns a `204 No Content` response code.</span></span>

### <a name="example-2-update-a-new-version-of-an-existing-app-for-admin-review-prior-to-publication-in-the-current-tenant-catalog"></a><span data-ttu-id="33df1-153">Exemplo 2: atualizar uma nova versão de um aplicativo existente para revisão de administrador antes da publicação no catálogo de locatários atual</span><span class="sxs-lookup"><span data-stu-id="33df1-153">Example 2: Update a new version of an existing app for admin review prior to publication in the current tenant catalog</span></span>

### <a name="request"></a><span data-ttu-id="33df1-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33df1-154">Request</span></span>

<!-- markdownlint-disable MD034 -->

# <a name="http"></a>[<span data-ttu-id="33df1-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="33df1-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_teamsapp"
}-->

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22/appDefinitions?requiresReview=true
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```
# <a name="javascript"></a>[<span data-ttu-id="33df1-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33df1-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="33df1-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="33df1-157">Response</span></span>

<span data-ttu-id="33df1-158">Se tiver êxito, este método retornará um `201 Created` código de resposta e o par de chave/valor `publishingState` : `submitted` no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33df1-158">If successful, this method returns a `201 Created` response code and the key/value pair `publishingState`: `submitted` in the response body.</span></span> <span data-ttu-id="33df1-159">*Consulte* [teamsappdefinition](../resources/teamsappdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="33df1-159">*See* [teamsappdefinition](../resources/teamsappdefinition.md).</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22/appDefinitions/MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appDefinition",
    "@odata.etag": "158749010",
    "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
    "teamsAppId": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
    "displayName": "Test app",
    "version": "1.0.11",
    "azureADAppId": "a651cc7d-ec54-4fb2-9d0e-2c58dc830b0b",
    "requiredResourceSpecificApplicationPermissions":[
         "ChannelMessage.Read.Group",
         "Channel.Create.Group",
         "Tab.ReadWrite.Group",
         "Member.Read.Group"
    ],
    "publishingState": "submitted",
    "lastModifiedDateTime": "2020-02-10 22:48:33.841",
}
```
