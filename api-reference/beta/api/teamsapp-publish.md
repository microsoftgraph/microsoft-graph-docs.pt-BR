---
title: Publicar teamsapp
description: Publicar um aplicativo no catálogo de aplicativos do Microsoft Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7694f51ff8f42f27e58fca04ec0ae87ad74e526e
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563475"
---
# <a name="publish-teamsapp"></a><span data-ttu-id="8b2ca-103">Publicar teamsApp</span><span class="sxs-lookup"><span data-stu-id="8b2ca-103">Publish teamsApp</span></span>

<span data-ttu-id="8b2ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b2ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b2ca-105">Publicar um [aplicativo](../resources/teamsapp.md) no catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="8b2ca-105">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="8b2ca-106">Especificamente, essa API publica o aplicativo no catálogo da sua organização (o catálogo de aplicativos do locatário); o recurso criado terá um valor de propriedade **distributionMethod** de `organization` .</span><span class="sxs-lookup"><span data-stu-id="8b2ca-106">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have a **distributionMethod** property value of `organization`.</span></span>

<span data-ttu-id="8b2ca-107">A propriedade **requiresReview** permite que qualquer usuário envie um aplicativo para revisão por um administrador.</span><span class="sxs-lookup"><span data-stu-id="8b2ca-107">The **requiresReview** property allows any user to submit an app for review by an administrator.</span></span> <span data-ttu-id="8b2ca-108">Os administradores podem aprovar ou rejeitar esses aplicativos por meio desta API ou do centro de administração do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="8b2ca-108">Admins can approve or reject these apps via this API or the Microsoft Teams admin center.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b2ca-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="8b2ca-109">Permissions</span></span>

<span data-ttu-id="8b2ca-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b2ca-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b2ca-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b2ca-112">Permission Type</span></span>                        | <span data-ttu-id="8b2ca-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8b2ca-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="8b2ca-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b2ca-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8b2ca-115">AppCatalog. Submit, AppCatalog. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8b2ca-115">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="8b2ca-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b2ca-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b2ca-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8b2ca-117">Not supported</span></span>|
| <span data-ttu-id="8b2ca-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b2ca-118">Application</span></span>                            | <span data-ttu-id="8b2ca-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b2ca-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b2ca-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b2ca-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps
```

<span data-ttu-id="8b2ca-121">Para publicar um aplicativo que exija uma análise:</span><span class="sxs-lookup"><span data-stu-id="8b2ca-121">To publish an app that requires a review:</span></span>

```http
POST /appCatalogs/teamsApps?requiresReview:{Boolean}
```

## <a name="query-parameters"></a><span data-ttu-id="8b2ca-122">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="8b2ca-122">Query parameters</span></span>

|<span data-ttu-id="8b2ca-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b2ca-123">Property</span></span>|<span data-ttu-id="8b2ca-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b2ca-124">Type</span></span>|<span data-ttu-id="8b2ca-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b2ca-125">Description</span></span>|
|----|----|----|
|<span data-ttu-id="8b2ca-126">requiresReview</span><span class="sxs-lookup"><span data-stu-id="8b2ca-126">requiresReview</span></span>| <span data-ttu-id="8b2ca-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b2ca-127">Boolean</span></span> | <span data-ttu-id="8b2ca-128">Esse parâmetro de consulta opcional dispara o processo de revisão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8b2ca-128">This optional query parameter triggers the app review process.</span></span> <span data-ttu-id="8b2ca-129">Os usuários com privilégios de administrador podem enviar aplicativos sem disparar uma revisão.</span><span class="sxs-lookup"><span data-stu-id="8b2ca-129">Users with admin privileges can submit apps without triggering a review.</span></span> <span data-ttu-id="8b2ca-130">Se os usuários desejarem solicitar uma revisão antes da publicação, eles devem  `requiresReview` ser definidos como `true` .</span><span class="sxs-lookup"><span data-stu-id="8b2ca-130">If users want to request a review before publishing, they must set  `requiresReview` to `true`.</span></span> <span data-ttu-id="8b2ca-131">Um usuário com privilégios de administrador pode optar por não definir `requiresReview` ou definir o valor como `false`  e o aplicativo será considerado aprovado e publicar instantaneamente.</span><span class="sxs-lookup"><span data-stu-id="8b2ca-131">A user who has admin privileges can opt not to set `requiresReview` or set the value to `false`  and the app will be considered approved and will publish instantly.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="8b2ca-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b2ca-132">Request headers</span></span>

| <span data-ttu-id="8b2ca-133">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8b2ca-133">Header</span></span>        | <span data-ttu-id="8b2ca-134">Valor</span><span class="sxs-lookup"><span data-stu-id="8b2ca-134">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="8b2ca-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b2ca-135">Authorization</span></span> | <span data-ttu-id="8b2ca-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b2ca-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8b2ca-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8b2ca-138">Content-Type</span></span>  | <span data-ttu-id="8b2ca-139">Application/zip.</span><span class="sxs-lookup"><span data-stu-id="8b2ca-139">application/zip.</span></span> <span data-ttu-id="8b2ca-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b2ca-140">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b2ca-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b2ca-141">Request body</span></span>

<span data-ttu-id="8b2ca-142">No corpo da solicitação, inclua uma carga de manifesto zip do teams.</span><span class="sxs-lookup"><span data-stu-id="8b2ca-142">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="8b2ca-143">Para obter detalhes, consulte [criar um pacote de aplicativos](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="8b2ca-143">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>  

<span data-ttu-id="8b2ca-144">Cada aplicativo no catálogo de aplicativos deve ter um manifesto exclusivo `id` .</span><span class="sxs-lookup"><span data-stu-id="8b2ca-144">Each app in the app catalog must have a unique manifest `id`.</span></span>

## <a name="response"></a><span data-ttu-id="8b2ca-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b2ca-145">Response</span></span>

<span data-ttu-id="8b2ca-146">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [teamsApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="8b2ca-146">If successful, this method returns a `200 OK` response code and a [teamsApp](../resources/teamsapp.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="8b2ca-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8b2ca-147">Examples</span></span>

### <a name="example-1-publish-an-app-to-the-app-catalog"></a><span data-ttu-id="8b2ca-148">Exemplo 1: publicar um aplicativo no catálogo de aplicativos</span><span class="sxs-lookup"><span data-stu-id="8b2ca-148">Example 1: Publish an app to the app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="8b2ca-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b2ca-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8b2ca-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b2ca-150">HTTP</span></span>](#tab/http)
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

# <a name="javascript"></a>[<span data-ttu-id="8b2ca-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b2ca-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b2ca-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b2ca-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="8b2ca-153">Para obter informações sobre como criar um arquivo zip do aplicativo do Microsoft Teams, consulte [criar um pacote de aplicativos](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="8b2ca-153">For information about how to create a Microsoft Teams application zip file, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>
<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="8b2ca-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b2ca-154">Response</span></span>

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

### <a name="example-2-upload-a-new-application-for-review-to-an-organizations-app-catalog"></a><span data-ttu-id="8b2ca-155">Exemplo 2: carregar um novo aplicativo para revisão para o catálogo de aplicativos de uma organização</span><span class="sxs-lookup"><span data-stu-id="8b2ca-155">Example 2: Upload a new application for review to an organization's app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="8b2ca-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b2ca-156">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8b2ca-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b2ca-157">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps?requiresReview=true
Content-type: application/zip
Content-length: 244
```

# <a name="javascript"></a>[<span data-ttu-id="8b2ca-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b2ca-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b2ca-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b2ca-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8b2ca-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b2ca-160">Response</span></span>

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

### <a name="example-3-approve-or-reject-an-app-pending-review"></a><span data-ttu-id="8b2ca-161">Exemplo 3: aprovar ou rejeitar uma revisão pendente do aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b2ca-161">Example 3: Approve or reject an app pending review</span></span>

#### <a name="request"></a><span data-ttu-id="8b2ca-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b2ca-162">Request</span></span>

<span data-ttu-id="8b2ca-163">**HTTP**</span><span class="sxs-lookup"><span data-stu-id="8b2ca-163">**HTTP**</span></span>
<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
PATCH https://graph.microsoft.com/beta/appCatalogs/teamsApps/a761ad07-22ef-4a53-9feb-2837c8ad4a84/appDefinitions/YTc2MWFkMDctMjJlZi00YTUzLTlmZWItMjgzN2M4YWQ0YTg0IyMxLjEuOCMjU3VibWl0dGVk
Content-type: application/json
If-Match: InFtSStsNVJHVWdzWUJRU2ZVWGp4RWc9PSI=

{
   "Body":{
      "publishingState":"published"
   }
}
```

---

#### <a name="response"></a><span data-ttu-id="8b2ca-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b2ca-164">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps('a761ad07-22ef-4a53-9feb-2837c8ad4a84')/appDefinitions/$entity",
    "id": "YTc2MWFkMDctMjJlZi00YTUzLTlmZWItMjgzN2M4YWQ0YTg0IyMxLjEuOCMjUHVibGlzaGVk",
    "teamsAppId": "a761ad07-22ef-4a53-9feb-2837c8ad4a84",
    "azureADAppId": null,
    "displayName": "Ducks",
    "version": "1.1.8",
    "requiredResourceSpecificApplicationPermissions": [],
    "publishingState": "published",
    "shortdescription": "quaerat quasi magnam. slight change. 5",
    "description": "Aliquid placeat animi debitis accusamus. Non perferendis ullam. Quis est consequuntur vitae provident. Sunt laudantium id aut. slight change 5",
    "lastModifiedDateTime": null,
    "createdBy": null
}
```
