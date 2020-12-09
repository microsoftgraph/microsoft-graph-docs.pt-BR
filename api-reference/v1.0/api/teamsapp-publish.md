---
title: Publicar teamsapp
description: 'Publicar um aplicativo no catálogo de aplicativos do Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 86a63997b9408cd4155a180d7919e54e99d8ad27
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607165"
---
# <a name="publish-teamsapp"></a><span data-ttu-id="550a6-103">Publicar teamsapp</span><span class="sxs-lookup"><span data-stu-id="550a6-103">Publish teamsapp</span></span>

<span data-ttu-id="550a6-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="550a6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="550a6-105">Publicar um [aplicativo](../resources/teamsapp.md) no catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="550a6-105">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span>
<span data-ttu-id="550a6-106">Especificamente, essa API publica o aplicativo no catálogo da sua organização (o catálogo de aplicativos do locatário); o recurso criado terá um valor de propriedade **distributionMethod** de `organization` .</span><span class="sxs-lookup"><span data-stu-id="550a6-106">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have a **distributionMethod** property value of `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="550a6-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="550a6-107">Permissions</span></span>

<span data-ttu-id="550a6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="550a6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="550a6-110">**Observação:** Somente os administradores globais podem chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="550a6-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="550a6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="550a6-111">Permission Type</span></span>                        | <span data-ttu-id="550a6-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="550a6-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="550a6-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="550a6-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="550a6-114">AppCatalog. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="550a6-114">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="550a6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="550a6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="550a6-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="550a6-116">Not supported</span></span>|
| <span data-ttu-id="550a6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="550a6-117">Application</span></span>                            | <span data-ttu-id="550a6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="550a6-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="550a6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="550a6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a><span data-ttu-id="550a6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="550a6-120">Request headers</span></span>

| <span data-ttu-id="550a6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="550a6-121">Header</span></span>        | <span data-ttu-id="550a6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="550a6-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="550a6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="550a6-123">Authorization</span></span> | <span data-ttu-id="550a6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="550a6-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="550a6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="550a6-126">Content-Type</span></span>  | <span data-ttu-id="550a6-127">Application/zip.</span><span class="sxs-lookup"><span data-stu-id="550a6-127">application/zip.</span></span> <span data-ttu-id="550a6-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="550a6-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="550a6-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="550a6-129">Request body</span></span>

<span data-ttu-id="550a6-130">No corpo da solicitação, inclua uma carga de manifesto zip do teams.</span><span class="sxs-lookup"><span data-stu-id="550a6-130">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="550a6-131">Para obter detalhes, consulte [criar um pacote de aplicativos](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="550a6-131">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

<span data-ttu-id="550a6-132">Cada aplicativo no catálogo de aplicativos deve ter uma ID de manifesto exclusiva.</span><span class="sxs-lookup"><span data-stu-id="550a6-132">Each app in the app catalog must have a unique manifest ID.</span></span>

## <a name="response"></a><span data-ttu-id="550a6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="550a6-133">Response</span></span>

<span data-ttu-id="550a6-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [teamsApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="550a6-134">If successful, this method returns a `200 OK` response code and a [teamsApp](../resources/teamsapp.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="550a6-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="550a6-135">Examples</span></span>

### <a name="example-1-publish-an-app-to-the-app-catalog"></a><span data-ttu-id="550a6-136">Exemplo 1: publicar um aplicativo no catálogo de aplicativos</span><span class="sxs-lookup"><span data-stu-id="550a6-136">Example 1: Publish an app to the app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="550a6-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="550a6-137">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="550a6-138">Para obter informações sobre como criar um arquivo zip do aplicativo do Microsoft Teams, consulte [criar um pacote de aplicativos](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="550a6-138">For information about how to create a Microsoft Teams application zip file, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

#### <a name="response"></a><span data-ttu-id="550a6-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="550a6-139">Response</span></span>

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
