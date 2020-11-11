---
title: Publicar teamsapp
description: Publicar um aplicativo no catálogo de aplicativos do Microsoft Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 78ff984bfec1e72a5fd480a9dd61d268beea7689
ms.sourcegitcommit: a9720ab80625a4692f7d2450164717853535d0b0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/11/2020
ms.locfileid: "48993970"
---
# <a name="publish-teamsapp"></a><span data-ttu-id="11c41-103">Publicar teamsApp</span><span class="sxs-lookup"><span data-stu-id="11c41-103">Publish teamsApp</span></span>

<span data-ttu-id="11c41-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11c41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11c41-105">Publicar um [aplicativo](../resources/teamsapp.md) no catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="11c41-105">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="11c41-106">Especificamente, essa API publica o aplicativo no catálogo da sua organização (o catálogo de aplicativos do locatário); o recurso criado terá um valor de propriedade **distributionMethod** de `organization` .</span><span class="sxs-lookup"><span data-stu-id="11c41-106">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have a **distributionMethod** property value of `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="11c41-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="11c41-107">Permissions</span></span>

<span data-ttu-id="11c41-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11c41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11c41-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11c41-110">Permission Type</span></span>                        | <span data-ttu-id="11c41-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11c41-111">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="11c41-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11c41-112">Delegated (work or school account)</span></span> | <span data-ttu-id="11c41-113">AppCatalog. Submit, AppCatalog. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="11c41-113">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="11c41-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11c41-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11c41-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="11c41-115">Not supported</span></span>|
| <span data-ttu-id="11c41-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11c41-116">Application</span></span>                            | <span data-ttu-id="11c41-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11c41-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="11c41-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11c41-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps
```

<span data-ttu-id="11c41-119">Para publicar um aplicativo que exija uma análise:</span><span class="sxs-lookup"><span data-stu-id="11c41-119">To publish an app that requires a review:</span></span>

```http
POST /appCatalogs/teamsApps?requiresReview:{Boolean}
```

## <a name="query-parameters"></a><span data-ttu-id="11c41-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="11c41-120">Query parameters</span></span>

|<span data-ttu-id="11c41-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11c41-121">Property</span></span>|<span data-ttu-id="11c41-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="11c41-122">Type</span></span>|<span data-ttu-id="11c41-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="11c41-123">Description</span></span>|
|----|----|----|
|<span data-ttu-id="11c41-124">requiresReview</span><span class="sxs-lookup"><span data-stu-id="11c41-124">requiresReview</span></span>| <span data-ttu-id="11c41-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="11c41-125">Boolean</span></span> | <span data-ttu-id="11c41-126">Esse parâmetro de consulta opcional dispara o processo de revisão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="11c41-126">This optional query parameter triggers the app review process.</span></span> <span data-ttu-id="11c41-127">Os usuários com privilégios de administrador podem enviar aplicativos sem disparar uma revisão.</span><span class="sxs-lookup"><span data-stu-id="11c41-127">Users with admin privileges can submit apps without triggering a review.</span></span> <span data-ttu-id="11c41-128">Se os usuários desejarem solicitar uma revisão antes da publicação, eles devem  `requiresReview` ser definidos como `true` .</span><span class="sxs-lookup"><span data-stu-id="11c41-128">If users want to request a review before publishing, they must set  `requiresReview` to `true`.</span></span> <span data-ttu-id="11c41-129">Um usuário com privilégios de administrador pode optar por não definir `requiresReview` ou definir o valor como `false`  e o aplicativo será considerado aprovado e publicar instantaneamente.</span><span class="sxs-lookup"><span data-stu-id="11c41-129">A user who has admin privileges can opt not to set `requiresReview` or set the value to `false`  and the app will be considered approved and will publish instantly.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="11c41-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11c41-130">Request headers</span></span>

| <span data-ttu-id="11c41-131">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="11c41-131">Header</span></span>        | <span data-ttu-id="11c41-132">Valor</span><span class="sxs-lookup"><span data-stu-id="11c41-132">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="11c41-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="11c41-133">Authorization</span></span> | <span data-ttu-id="11c41-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11c41-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="11c41-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="11c41-136">Content-Type</span></span>  | <span data-ttu-id="11c41-137">Application/zip.</span><span class="sxs-lookup"><span data-stu-id="11c41-137">application/zip.</span></span> <span data-ttu-id="11c41-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11c41-138">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11c41-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11c41-139">Request body</span></span>

<span data-ttu-id="11c41-140">No corpo da solicitação, inclua uma carga de manifesto zip do teams.</span><span class="sxs-lookup"><span data-stu-id="11c41-140">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="11c41-141">Para obter detalhes, consulte [criar um pacote de aplicativos](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="11c41-141">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>  

<span data-ttu-id="11c41-142">Cada aplicativo no catálogo de aplicativos deve ter um manifesto exclusivo `id` .</span><span class="sxs-lookup"><span data-stu-id="11c41-142">Each app in the app catalog must have a unique manifest `id`.</span></span>

## <a name="response"></a><span data-ttu-id="11c41-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="11c41-143">Response</span></span>

<span data-ttu-id="11c41-144">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [teamsApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="11c41-144">If successful, this method returns a `200 OK` response code and a [teamsApp](../resources/teamsapp.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="11c41-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="11c41-145">Examples</span></span>

### <a name="example-1-publish-an-app-to-the-app-catalog"></a><span data-ttu-id="11c41-146">Exemplo 1: publicar um aplicativo no catálogo de aplicativos</span><span class="sxs-lookup"><span data-stu-id="11c41-146">Example 1: Publish an app to the app catalog</span></span>
#### <a name="request"></a><span data-ttu-id="11c41-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11c41-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="11c41-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="11c41-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```
# <a name="javascript"></a>[<span data-ttu-id="11c41-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11c41-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11c41-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11c41-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="11c41-151">Para obter informações sobre como criar um arquivo zip do aplicativo do Microsoft Teams, consulte [criar um pacote de aplicativos](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="11c41-151">For information about how to create a Microsoft Teams application zip file, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>
<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="11c41-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="11c41-152">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}
```

### <a name="example-2-upload-a-new-application-for-review-to-an-organizations-app-catalog"></a><span data-ttu-id="11c41-153">Exemplo 2: carregar um novo aplicativo para revisão para o catálogo de aplicativos de uma organização</span><span class="sxs-lookup"><span data-stu-id="11c41-153">Example 2: Upload a new application for review to an organization's app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="11c41-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11c41-154">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="11c41-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="11c41-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps?requiresReview=true
Content-type: application/zip
Content-length: 244
```
# <a name="javascript"></a>[<span data-ttu-id="11c41-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11c41-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11c41-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11c41-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="11c41-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="11c41-158">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps/$entity",
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}
```
