---
title: Permissões
description: 'Publicar um aplicativo no catálogo de aplicativos do Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b528ce517bc5cd3df627c01ffc247f5aeef19015
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864933"
---
# <a name="publish-apps-to-your-organizations-app-catalog"></a><span data-ttu-id="b2738-103">Publicar aplicativos no catálogo de aplicativos da sua organização</span><span class="sxs-lookup"><span data-stu-id="b2738-103">Publish apps to your organization's app catalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2738-104">Publicar um [aplicativo](../resources/teamsapp.md) no catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="b2738-104">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span>
<span data-ttu-id="b2738-105">Especificamente, essa API publica o aplicativo no catálogo da sua organização (o catálogo de aplicativos do locatário); o recurso `distributionMethod`  =  `organization`criado terá.</span><span class="sxs-lookup"><span data-stu-id="b2738-105">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have `distributionMethod` = `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2738-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b2738-106">Permissions</span></span>

<span data-ttu-id="b2738-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="b2738-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="b2738-109">**Observação:** Somente os administradores globais podem chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b2738-109">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="b2738-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2738-110">Permission Type</span></span>                        | <span data-ttu-id="b2738-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b2738-111">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="b2738-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2738-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b2738-113">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2738-113">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="b2738-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2738-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2738-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b2738-115">Not supported</span></span>|
| <span data-ttu-id="b2738-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2738-116">Application</span></span>                            | <span data-ttu-id="b2738-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b2738-117">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2738-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2738-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a><span data-ttu-id="b2738-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2738-119">Request headers</span></span>

| <span data-ttu-id="b2738-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2738-120">Header</span></span>        | <span data-ttu-id="b2738-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b2738-121">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="b2738-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2738-122">Authorization</span></span> | <span data-ttu-id="b2738-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2738-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b2738-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b2738-125">Content-Type</span></span>  | <span data-ttu-id="b2738-126">aplicativo/zip</span><span class="sxs-lookup"><span data-stu-id="b2738-126">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2738-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2738-127">Request body</span></span>

<span data-ttu-id="b2738-128">Carga do manifesto zip do teams.</span><span class="sxs-lookup"><span data-stu-id="b2738-128">Teams Zip Manifest Payload.</span></span>
<span data-ttu-id="b2738-129">Para o arquivo zip do aplicativo do Teams, [consulte criar um pacote de aplicativos](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="b2738-129">For Teams application zip file [see Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>
<span data-ttu-id="b2738-130">Você não pode criar um aplicativo para uma organização que tenha a mesma ID de manifesto que outro aplicativo da organização.</span><span class="sxs-lookup"><span data-stu-id="b2738-130">You can't create an app for an organization that has the same manifest ID as another app in that organization.</span></span>

## <a name="response"></a><span data-ttu-id="b2738-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2738-131">Response</span></span>

<span data-ttu-id="b2738-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="b2738-132">If successful, this method returns a `200 OK` response code and a [teamsCatalogApp](../resources/teamsapp.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="b2738-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2738-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2738-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2738-134">Request</span></span>

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="b2738-135">Para obter informações sobre como criar um arquivo zip do aplicativo do Microsoft Teams, consulte [criar um pacote de aplicativos](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="b2738-135">For information about how to create a Microsoft Teams application zip file, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

### <a name="response"></a><span data-ttu-id="b2738-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2738-136">Response</span></span>

```
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
