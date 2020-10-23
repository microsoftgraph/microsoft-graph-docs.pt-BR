---
title: Publicar teamsapp
description: Publicar um aplicativo no catálogo de aplicativos do Microsoft Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cf5dde98d9f21249a23d6806b4f79dd6ae824572
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2020
ms.locfileid: "48741933"
---
# <a name="publish-teamsapp"></a><span data-ttu-id="fe20b-103">Publicar teamsApp</span><span class="sxs-lookup"><span data-stu-id="fe20b-103">Publish teamsApp</span></span>

<span data-ttu-id="fe20b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe20b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe20b-105">Publicar um [aplicativo](../resources/teamsapp.md) no catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="fe20b-105">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="fe20b-106">Especificamente, essa API publica o aplicativo no catálogo da sua organização (o catálogo de aplicativos do locatário); o recurso criado terá um valor de propriedade **distributionMethod** de `organization` .</span><span class="sxs-lookup"><span data-stu-id="fe20b-106">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have a **distributionMethod** property value of `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe20b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fe20b-107">Permissions</span></span>

<span data-ttu-id="fe20b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe20b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="fe20b-110">**Observação:** Somente os administradores globais podem chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="fe20b-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="fe20b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe20b-111">Permission Type</span></span>                        | <span data-ttu-id="fe20b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe20b-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="fe20b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe20b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="fe20b-114">AppCatalog. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="fe20b-114">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="fe20b-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe20b-115">Delegated (work or school account)</span></span> | <span data-ttu-id="fe20b-116">AppCatalog.Submit</span><span class="sxs-lookup"><span data-stu-id="fe20b-116">AppCatalog.Submit</span></span>|
| <span data-ttu-id="fe20b-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe20b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe20b-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="fe20b-118">Not supported</span></span>|
| <span data-ttu-id="fe20b-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe20b-119">Application</span></span>                            | <span data-ttu-id="fe20b-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe20b-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe20b-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe20b-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps
```

<span data-ttu-id="fe20b-122">Para publicar um aplicativo que exija uma análise:</span><span class="sxs-lookup"><span data-stu-id="fe20b-122">To publish an app that requires a review:</span></span>

```http
POST /appCatalogs/teamsApps?requiresReview:{Boolean}
```

## <a name="query-parameters"></a><span data-ttu-id="fe20b-123">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="fe20b-123">Query parameters</span></span>

|<span data-ttu-id="fe20b-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe20b-124">Property</span></span>|<span data-ttu-id="fe20b-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe20b-125">Type</span></span>|<span data-ttu-id="fe20b-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe20b-126">Description</span></span>|
|----|----|----|
|<span data-ttu-id="fe20b-127">requiresReview</span><span class="sxs-lookup"><span data-stu-id="fe20b-127">requiresReview</span></span>| <span data-ttu-id="fe20b-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="fe20b-128">Boolean</span></span> | <span data-ttu-id="fe20b-129">Esse parâmetro de consulta opcional dispara o processo de revisão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fe20b-129">This optional query parameter triggers the app review process.</span></span> <span data-ttu-id="fe20b-130">Os usuários com privilégios de administrador podem enviar aplicativos sem disparar uma revisão.</span><span class="sxs-lookup"><span data-stu-id="fe20b-130">Users with admin privileges can submit apps without triggering a review.</span></span> <span data-ttu-id="fe20b-131">Se os usuários desejarem solicitar uma revisão antes da publicação, eles devem  `requiresReview` ser definidos como `true` .</span><span class="sxs-lookup"><span data-stu-id="fe20b-131">If users want to request a review before publishing, they must set  `requiresReview` to `true`.</span></span> <span data-ttu-id="fe20b-132">Um usuário com privilégios de administrador pode optar por não definir `requiresReview` ou definir o valor como `false`  e o aplicativo será considerado aprovado e publicar instantaneamente.</span><span class="sxs-lookup"><span data-stu-id="fe20b-132">A user who has admin privileges can opt not to set `requiresReview` or set the value to `false`  and the app will be considered approved and will publish instantly.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="fe20b-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe20b-133">Request headers</span></span>

| <span data-ttu-id="fe20b-134">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fe20b-134">Header</span></span>        | <span data-ttu-id="fe20b-135">Valor</span><span class="sxs-lookup"><span data-stu-id="fe20b-135">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="fe20b-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe20b-136">Authorization</span></span> | <span data-ttu-id="fe20b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe20b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fe20b-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe20b-139">Content-Type</span></span>  | <span data-ttu-id="fe20b-140">Application/zip.</span><span class="sxs-lookup"><span data-stu-id="fe20b-140">application/zip.</span></span> <span data-ttu-id="fe20b-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe20b-141">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe20b-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe20b-142">Request body</span></span>

<span data-ttu-id="fe20b-143">No corpo da solicitação, inclua uma carga de manifesto zip do teams.</span><span class="sxs-lookup"><span data-stu-id="fe20b-143">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="fe20b-144">Para obter detalhes, consulte [criar um pacote de aplicativos](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="fe20b-144">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>  

<span data-ttu-id="fe20b-145">Cada aplicativo no catálogo de aplicativos deve ter um manifesto exclusivo `id` .</span><span class="sxs-lookup"><span data-stu-id="fe20b-145">Each app in the app catalog must have a unique manifest `id`.</span></span>

## <a name="response"></a><span data-ttu-id="fe20b-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe20b-146">Response</span></span>

<span data-ttu-id="fe20b-147">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [teamsApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="fe20b-147">If successful, this method returns a `200 OK` response code and a [teamsApp](../resources/teamsapp.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="fe20b-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fe20b-148">Examples</span></span>

### <a name="example-1-publish-an-app-to-the-app-catalog"></a><span data-ttu-id="fe20b-149">Exemplo 1: publicar um aplicativo no catálogo de aplicativos</span><span class="sxs-lookup"><span data-stu-id="fe20b-149">Example 1: Publish an app to the app catalog</span></span>
#### <a name="request"></a><span data-ttu-id="fe20b-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe20b-150">Request</span></span>

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

<span data-ttu-id="fe20b-151">Para obter informações sobre como criar um arquivo zip do aplicativo do Microsoft Teams, consulte [criar um pacote de aplicativos](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="fe20b-151">For information about how to create a Microsoft Teams application zip file, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>
<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="fe20b-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe20b-152">Response</span></span>

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

### <a name="example-2-upload-a-new-application-for-review-to-an-organizations-app-catalog"></a><span data-ttu-id="fe20b-153">Exemplo 2: carregar um novo aplicativo para revisão para o catálogo de aplicativos de uma organização</span><span class="sxs-lookup"><span data-stu-id="fe20b-153">Example 2: Upload a new application for review to an organization's app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="fe20b-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe20b-154">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps?requiresReview=true
Content-type: application/zip
Content-length: 244
```

#### <a name="response"></a><span data-ttu-id="fe20b-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe20b-155">Response</span></span>

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
