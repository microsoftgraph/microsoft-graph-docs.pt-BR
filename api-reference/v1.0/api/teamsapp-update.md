---
title: Atualizar teamsApp
description: 'Atualize um aplicativo publicado anteriormente em um catálogo de aplicativos do Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8610c51922989d96f455073ea824c258d6d454ba
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774796"
---
# <a name="update-teamsapp"></a><span data-ttu-id="11e60-103">Atualizar teamsApp</span><span class="sxs-lookup"><span data-stu-id="11e60-103">Update teamsApp</span></span>

<span data-ttu-id="11e60-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11e60-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="11e60-105">Atualize [um aplicativo](../resources/teamsapp.md) publicado anteriormente no catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="11e60-105">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="11e60-106">Para atualizar um aplicativo, a **propriedade distributionMethod** para o aplicativo deve ser definida como `organization` .</span><span class="sxs-lookup"><span data-stu-id="11e60-106">To update an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="11e60-107">Essa API atualiza especificamente um aplicativo publicado no catálogo de aplicativos da sua organização (o catálogo de aplicativos de locatário).</span><span class="sxs-lookup"><span data-stu-id="11e60-107">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span>

## <a name="permissions"></a><span data-ttu-id="11e60-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="11e60-108">Permissions</span></span>

<span data-ttu-id="11e60-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11e60-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="11e60-111">**Observação:** Somente administradores globais podem chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="11e60-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="11e60-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11e60-112">Permission Type</span></span>                        | <span data-ttu-id="11e60-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11e60-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="11e60-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11e60-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="11e60-115">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11e60-115">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="11e60-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11e60-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11e60-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="11e60-117">Not supported</span></span>|
| <span data-ttu-id="11e60-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11e60-118">Application</span></span>                            | <span data-ttu-id="11e60-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11e60-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="11e60-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11e60-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps/{id}/appDefinitions
```

## <a name="query-parameters"></a><span data-ttu-id="11e60-121">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="11e60-121">Query parameters</span></span>

|<span data-ttu-id="11e60-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11e60-122">Property</span></span>|<span data-ttu-id="11e60-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="11e60-123">Type</span></span>|<span data-ttu-id="11e60-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="11e60-124">Description</span></span>|
|----|----|----|
|<span data-ttu-id="11e60-125">requiresReview</span><span class="sxs-lookup"><span data-stu-id="11e60-125">requiresReview</span></span>| <span data-ttu-id="11e60-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="11e60-126">Boolean</span></span> | <span data-ttu-id="11e60-127">Esse parâmetro de consulta opcional aciona o processo de revisão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="11e60-127">This optional query parameter triggers the app review process.</span></span> <span data-ttu-id="11e60-128">Os usuários com privilégios de administrador podem enviar aplicativos sem disparar uma revisão.</span><span class="sxs-lookup"><span data-stu-id="11e60-128">Users with admin privileges can submit apps without triggering a review.</span></span> <span data-ttu-id="11e60-129">Se os usuários quiserem solicitar uma revisão antes da publicação, eles deverão definir  `requiresReview` como `true` .</span><span class="sxs-lookup"><span data-stu-id="11e60-129">If users want to request a review before publishing, they must set  `requiresReview` to `true`.</span></span> <span data-ttu-id="11e60-130">Um usuário com privilégios de administrador pode optar por não definir ou definir o valor como e o aplicativo será considerado aprovado e `requiresReview` `false`  publicará instantaneamente.</span><span class="sxs-lookup"><span data-stu-id="11e60-130">A user who has admin privileges can opt not to set `requiresReview` or set the value to `false`  and the app will be considered approved and will publish instantly.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="11e60-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11e60-131">Request headers</span></span>

| <span data-ttu-id="11e60-132">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="11e60-132">Header</span></span>        | <span data-ttu-id="11e60-133">Valor</span><span class="sxs-lookup"><span data-stu-id="11e60-133">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="11e60-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="11e60-134">Authorization</span></span> | <span data-ttu-id="11e60-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11e60-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="11e60-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="11e60-137">Content-Type</span></span>  | <span data-ttu-id="11e60-138">application/zip.</span><span class="sxs-lookup"><span data-stu-id="11e60-138">application/zip.</span></span> <span data-ttu-id="11e60-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11e60-139">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11e60-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11e60-140">Request body</span></span>

<span data-ttu-id="11e60-141">No corpo da solicitação, inclua uma carga de manifesto zip do Teams.</span><span class="sxs-lookup"><span data-stu-id="11e60-141">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="11e60-142">Para obter detalhes, consulte [Create an app package](/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="11e60-142">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="11e60-143">**Observação:** Use a ID retornada da chamada Lista [de](./appcatalogs-list-teamsapps.md) aplicativos publicados para fazer referência ao aplicativo que você gostaria de atualizar.</span><span class="sxs-lookup"><span data-stu-id="11e60-143">**Note:** Use the ID returned from the [List published apps](./appcatalogs-list-teamsapps.md) call to reference the app you'd like to update.</span></span> <span data-ttu-id="11e60-144">Não use a ID do manifesto do pacote do aplicativo zip.</span><span class="sxs-lookup"><span data-stu-id="11e60-144">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="11e60-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="11e60-145">Response</span></span>

<span data-ttu-id="11e60-146">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="11e60-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="11e60-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="11e60-147">Examples</span></span>

### <a name="example-1-update-an-application-previously-published-to-the-microsoft-teams-app-catalog"></a><span data-ttu-id="11e60-148">Exemplo 1: atualizar um aplicativo publicado anteriormente no catálogo de aplicativos do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="11e60-148">Example 1: Update an application previously published to the Microsoft Teams app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="11e60-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11e60-149">Request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8/appDefinitions
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="11e60-150">Para obter detalhes sobre o arquivo zip do aplicativo Teams, consulte [Create app package](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="11e60-150">For details about the Teams application zip file, see [Create app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>
<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="11e60-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="11e60-151">Response</span></span>

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-new-version-of-an-existing-app-for-admin-review-prior-to-publication-in-the-current-tenant-catalog"></a><span data-ttu-id="11e60-152">Exemplo 2: atualizar uma nova versão de um aplicativo existente para revisão de administrador antes da publicação no catálogo de locatários atual</span><span class="sxs-lookup"><span data-stu-id="11e60-152">Example 2: Update a new version of an existing app for admin review prior to publication in the current tenant catalog</span></span>

#### <a name="request"></a><span data-ttu-id="11e60-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11e60-153">Request</span></span>

<!-- markdownlint-disable MD034 -->


# <a name="http"></a>[<span data-ttu-id="11e60-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="11e60-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_teamsapp"
}-->

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22/appDefinitions?requiresReview=true
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```
# <a name="javascript"></a>[<span data-ttu-id="11e60-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11e60-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="11e60-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="11e60-156">Response</span></span>

<span data-ttu-id="11e60-157">Se tiver êxito, este método retornará um código de resposta e o par `201 Created` chave/valor `publishingState` : no corpo da `submitted` resposta.</span><span class="sxs-lookup"><span data-stu-id="11e60-157">If successful, this method returns a `201 Created` response code and the key/value pair `publishingState`: `submitted` in the response body.</span></span> <span data-ttu-id="11e60-158">*Consulte* [teamsappdefinition](../resources/teamsappdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="11e60-158">*See* [teamsappdefinition](../resources/teamsappdefinition.md).</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22/appDefinitions/MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#appDefinition",
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
