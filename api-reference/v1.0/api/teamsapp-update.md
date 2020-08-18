---
title: Atualizar teamsApp
description: 'Atualize um aplicativo publicado anteriormente em um catálogo de aplicativos do teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 31f7b40b8f6c1f6de1fcaf6122c4311e5a65d016
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792139"
---
# <a name="update-teamsapp"></a><span data-ttu-id="13860-103">Atualizar teamsApp</span><span class="sxs-lookup"><span data-stu-id="13860-103">Update teamsApp</span></span>

<span data-ttu-id="13860-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13860-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="13860-105">Atualize um [aplicativo](../resources/teamsapp.md) publicado anteriormente no catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="13860-105">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="13860-106">Para atualizar um aplicativo, a propriedade **distributionMethod** para o aplicativo deve ser definida como `organization` .</span><span class="sxs-lookup"><span data-stu-id="13860-106">To update an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="13860-107">Essa API atualiza especificamente um aplicativo publicado no catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário).</span><span class="sxs-lookup"><span data-stu-id="13860-107">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span>

## <a name="permissions"></a><span data-ttu-id="13860-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="13860-108">Permissions</span></span>

<span data-ttu-id="13860-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13860-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="13860-111">**Observação:** Somente os administradores globais podem chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="13860-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="13860-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13860-112">Permission Type</span></span>                        | <span data-ttu-id="13860-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="13860-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="13860-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13860-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="13860-115">AppCatalog. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="13860-115">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="13860-116">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13860-116">Delegated (work or school account)</span></span> | <span data-ttu-id="13860-117">AppCatalog. Submit</span><span class="sxs-lookup"><span data-stu-id="13860-117">AppCatalog.Submit</span></span>|
| <span data-ttu-id="13860-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13860-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13860-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="13860-119">Not supported</span></span>|
| <span data-ttu-id="13860-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13860-120">Application</span></span>                            | <span data-ttu-id="13860-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13860-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="13860-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13860-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps/{id}/appDefinitions
```

## <a name="query-parameters"></a><span data-ttu-id="13860-123">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="13860-123">Query parameters</span></span>

|<span data-ttu-id="13860-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13860-124">Property</span></span>|<span data-ttu-id="13860-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="13860-125">Type</span></span>|<span data-ttu-id="13860-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="13860-126">Description</span></span>|
|----|----|----|
|<span data-ttu-id="13860-127">requiresReview</span><span class="sxs-lookup"><span data-stu-id="13860-127">requiresReview</span></span>| <span data-ttu-id="13860-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="13860-128">Boolean</span></span> | <span data-ttu-id="13860-129">Esse parâmetro de consulta opcional dispara o processo de revisão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="13860-129">This optional query parameter triggers the app review process.</span></span> <span data-ttu-id="13860-130">Os usuários com privilégios de administrador podem enviar aplicativos sem disparar uma revisão.</span><span class="sxs-lookup"><span data-stu-id="13860-130">Users with admin privileges can submit apps without triggering a review.</span></span> <span data-ttu-id="13860-131">Se os usuários desejarem solicitar uma revisão antes da publicação, eles devem  `requiresReview` ser definidos como `true` .</span><span class="sxs-lookup"><span data-stu-id="13860-131">If users want to request a review before publishing, they must set  `requiresReview` to `true`.</span></span> <span data-ttu-id="13860-132">Um usuário com privilégios de administrador pode optar por não definir `requiresReview` ou definir o valor como `false`  e o aplicativo será considerado aprovado e publicar instantaneamente.</span><span class="sxs-lookup"><span data-stu-id="13860-132">A user who has admin privileges can opt not to set `requiresReview` or set the value to `false`  and the app will be considered approved and will publish instantly.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="13860-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13860-133">Request headers</span></span>

| <span data-ttu-id="13860-134">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="13860-134">Header</span></span>        | <span data-ttu-id="13860-135">Valor</span><span class="sxs-lookup"><span data-stu-id="13860-135">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="13860-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="13860-136">Authorization</span></span> | <span data-ttu-id="13860-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13860-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="13860-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="13860-139">Content-Type</span></span>  | <span data-ttu-id="13860-140">Application/zip.</span><span class="sxs-lookup"><span data-stu-id="13860-140">application/zip.</span></span> <span data-ttu-id="13860-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13860-141">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13860-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13860-142">Request body</span></span>

<span data-ttu-id="13860-143">No corpo da solicitação, inclua uma carga de manifesto zip do teams.</span><span class="sxs-lookup"><span data-stu-id="13860-143">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="13860-144">Para obter detalhes, consulte [criar um pacote de aplicativos](/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="13860-144">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="13860-145">**Observação:** Use a ID retornada da chamada [lista de aplicativos publicados](./teamsapp-list.md) para fazer referência ao aplicativo que você deseja atualizar.</span><span class="sxs-lookup"><span data-stu-id="13860-145">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call to reference the app you'd like to update.</span></span> <span data-ttu-id="13860-146">Não use a ID do manifesto do pacote de aplicativos zip.</span><span class="sxs-lookup"><span data-stu-id="13860-146">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="13860-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="13860-147">Response</span></span>

<span data-ttu-id="13860-148">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="13860-148">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="13860-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="13860-149">Examples</span></span>

### <a name="example-1-update-an-application-previously-published-to-the-microsoft-teams-app-catalog"></a><span data-ttu-id="13860-150">Exemplo 1: atualizar um aplicativo publicado anteriormente no catálogo de aplicativos do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="13860-150">Example 1: Update an application previously published to the Microsoft Teams app catalog</span></span>

### <a name="request"></a><span data-ttu-id="13860-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13860-151">Request</span></span>

<!-- markdownlint-disable MD034 -->
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

<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="13860-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="13860-152">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-previously-reviewed-and-published-application-to-the-teams-app-catalog"></a><span data-ttu-id="13860-153">Exemplo 2: atualizar um aplicativo previamente revisado e publicado para o catálogo de aplicativos do teams</span><span class="sxs-lookup"><span data-stu-id="13860-153">Example 2: Update a previously reviewed and published application to the Teams app catalog</span></span>

### <a name="request"></a><span data-ttu-id="13860-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13860-154">Request</span></span>

<!-- markdownlint-disable MD034 -->
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

### <a name="response"></a><span data-ttu-id="13860-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="13860-155">Response</span></span>

<span data-ttu-id="13860-156">Se tiver êxito, este método retornará um `201 Created` código de resposta e o par de chave/valor `publishingState` : `submitted` no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13860-156">If successful, this method returns a `201 Created` response code and the key/value pair `publishingState`: `submitted` in the response body.</span></span> <span data-ttu-id="13860-157">Para obter detalhes, consulte [teamsAppDefinition](../resources/teamsappdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="13860-157">For details, see [teamsAppDefinition](../resources/teamsappdefinition.md).</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22/appDefinitions/MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==

{
    "@odata.context": "https://graph.microsoft.com/v1/$metadata#appDefinition",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2020-08-08 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
