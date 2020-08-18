---
title: Publicar teamsapp
description: 'Publicar um aplicativo no catálogo de aplicativos do Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8a993178cc6735449fc5ce14a8c6d5663d9e9003
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792370"
---
# <a name="publish-teamsapp"></a><span data-ttu-id="a353b-103">Publicar teamsapp</span><span class="sxs-lookup"><span data-stu-id="a353b-103">Publish teamsapp</span></span>

<span data-ttu-id="a353b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a353b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a353b-105">Publicar um [aplicativo](../resources/teamsapp.md) no catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a353b-105">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span>
<span data-ttu-id="a353b-106">Especificamente, essa API publica o aplicativo no catálogo da sua organização (o catálogo de aplicativos do locatário); o recurso criado terá um valor de propriedade **distributionMethod** de `organization` .</span><span class="sxs-lookup"><span data-stu-id="a353b-106">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have a **distributionMethod** property value of `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="a353b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a353b-107">Permissions</span></span>

<span data-ttu-id="a353b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="a353b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="a353b-110">**Observação:** Somente os administradores globais podem chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a353b-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="a353b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a353b-111">Permission Type</span></span>                        | <span data-ttu-id="a353b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a353b-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="a353b-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a353b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a353b-114">AppCatalog. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a353b-114">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="a353b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a353b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a353b-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a353b-116">Not supported</span></span>|
| <span data-ttu-id="a353b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a353b-117">Application</span></span>                            | <span data-ttu-id="a353b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a353b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a353b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a353b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```
<span data-ttu-id="a353b-120">Para publicar um aplicativo que exija uma análise:</span><span class="sxs-lookup"><span data-stu-id="a353b-120">To publish an app that requires a review:</span></span>

```http
POST /appCatalogs/teamsApps?requiresReview:{Boolean}
```

## <a name="query-parameters"></a><span data-ttu-id="a353b-121">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="a353b-121">Query parameters</span></span>

|<span data-ttu-id="a353b-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a353b-122">Property</span></span>|<span data-ttu-id="a353b-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="a353b-123">Type</span></span>|<span data-ttu-id="a353b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="a353b-124">Description</span></span>|
|----|----|----|
|<span data-ttu-id="a353b-125">requiresReview</span><span class="sxs-lookup"><span data-stu-id="a353b-125">requiresReview</span></span>| <span data-ttu-id="a353b-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="a353b-126">Boolean</span></span> | <span data-ttu-id="a353b-127">Esse parâmetro de consulta opcional dispara o processo de revisão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a353b-127">This optional query parameter triggers the app review process.</span></span> <span data-ttu-id="a353b-128">Os usuários com privilégios de administrador podem enviar aplicativos sem disparar uma revisão.</span><span class="sxs-lookup"><span data-stu-id="a353b-128">Users with admin privileges can submit apps without triggering a review.</span></span> <span data-ttu-id="a353b-129">Se os usuários desejarem solicitar uma revisão antes da publicação, eles devem  `requiresReview` ser definidos como `true` .</span><span class="sxs-lookup"><span data-stu-id="a353b-129">If users want to request a review before publishing, they must set  `requiresReview` to `true`.</span></span> <span data-ttu-id="a353b-130">Um usuário com privilégios de administrador pode optar por não definir `requiresReview` ou definir o valor como `false`  e o aplicativo será considerado aprovado e publicar instantaneamente.</span><span class="sxs-lookup"><span data-stu-id="a353b-130">A user who has admin privileges can opt not to set `requiresReview` or set the value to `false`  and the app will be considered approved and will publish instantly.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="a353b-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a353b-131">Request headers</span></span>

| <span data-ttu-id="a353b-132">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a353b-132">Header</span></span>        | <span data-ttu-id="a353b-133">Valor</span><span class="sxs-lookup"><span data-stu-id="a353b-133">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="a353b-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="a353b-134">Authorization</span></span> | <span data-ttu-id="a353b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a353b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a353b-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a353b-137">Content-Type</span></span>  | <span data-ttu-id="a353b-138">Application/zip.</span><span class="sxs-lookup"><span data-stu-id="a353b-138">application/zip.</span></span> <span data-ttu-id="a353b-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a353b-139">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a353b-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a353b-140">Request body</span></span>

<span data-ttu-id="a353b-141">No corpo da solicitação, inclua uma carga de manifesto zip do teams.</span><span class="sxs-lookup"><span data-stu-id="a353b-141">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="a353b-142">Para obter detalhes, consulte [criar um pacote de aplicativos](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="a353b-142">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

<span data-ttu-id="a353b-143">Cada aplicativo no catálogo de aplicativos deve ter uma ID de manifesto exclusiva.</span><span class="sxs-lookup"><span data-stu-id="a353b-143">Each app in the app catalog must have a unique manifest id.</span></span>

## <a name="response"></a><span data-ttu-id="a353b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a353b-144">Response</span></span>

<span data-ttu-id="a353b-145">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [teamsApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="a353b-145">If successful, this method returns a `200 OK` response code and a [teamsApp](../resources/teamsapp.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="a353b-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a353b-146">Examples</span></span>

### <a name="example-1-publish-an-app-to-the-app-catalog"></a><span data-ttu-id="a353b-147">Exemplo 1: publicar um aplicativo no catálogo de aplicativos</span><span class="sxs-lookup"><span data-stu-id="a353b-147">Example 1: Publish an app to the app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="a353b-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a353b-148">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="a353b-149">Para obter informações sobre como criar um arquivo zip do aplicativo do Microsoft Teams, consulte [criar um pacote de aplicativos](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="a353b-149">For information about how to create a Microsoft Teams application zip file, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

#### <a name="response"></a><span data-ttu-id="a353b-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="a353b-150">Response</span></span>

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
### <a name="example-2-upload-a-new-application-for-review-to-an-organizations-app-catalog"></a><span data-ttu-id="a353b-151">Exemplo 2: carregar um novo aplicativo para revisão para o catálogo de aplicativos de uma organização</span><span class="sxs-lookup"><span data-stu-id="a353b-151">Example 2: Upload a new application for review to an organization's app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="a353b-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a353b-152">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?requiresReview=true
Content-type: application/zip
Content-length: 244
```

#### <a name="response"></a><span data-ttu-id="a353b-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="a353b-153">Response</span></span>

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
