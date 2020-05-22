---
title: Permissões
description: 'Publicar um aplicativo no catálogo de aplicativos do Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8076cc4ec988c311dd9a4cfde3b01a27a2a5d88e
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345762"
---
# <a name="publish-apps-to-your-organizations-app-catalog"></a><span data-ttu-id="20352-103">Publicar aplicativos no catálogo de aplicativos da sua organização</span><span class="sxs-lookup"><span data-stu-id="20352-103">Publish apps to your organization's app catalog</span></span>

<span data-ttu-id="20352-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20352-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="20352-105">Publicar um [aplicativo](../resources/teamsapp.md) no catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="20352-105">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span>
<span data-ttu-id="20352-106">Especificamente, essa API publica o aplicativo no catálogo da sua organização (o catálogo de aplicativos do locatário); o recurso criado terá `distributionMethod`  =  `organization` .</span><span class="sxs-lookup"><span data-stu-id="20352-106">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have `distributionMethod` = `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="20352-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="20352-107">Permissions</span></span>

<span data-ttu-id="20352-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="20352-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="20352-110">**Observação:** Somente os administradores globais podem chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="20352-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="20352-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20352-111">Permission Type</span></span>                        | <span data-ttu-id="20352-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20352-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="20352-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20352-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="20352-114">AppCatalog. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="20352-114">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="20352-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20352-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20352-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="20352-116">Not supported</span></span>|
| <span data-ttu-id="20352-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20352-117">Application</span></span>                            | <span data-ttu-id="20352-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20352-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="20352-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20352-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a><span data-ttu-id="20352-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20352-120">Request headers</span></span>

| <span data-ttu-id="20352-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="20352-121">Header</span></span>        | <span data-ttu-id="20352-122">Valor</span><span class="sxs-lookup"><span data-stu-id="20352-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="20352-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="20352-123">Authorization</span></span> | <span data-ttu-id="20352-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20352-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="20352-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="20352-126">Content-Type</span></span>  | <span data-ttu-id="20352-127">aplicativo/zip</span><span class="sxs-lookup"><span data-stu-id="20352-127">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="20352-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20352-128">Request body</span></span>

<span data-ttu-id="20352-129">Carga do manifesto zip do teams.</span><span class="sxs-lookup"><span data-stu-id="20352-129">Teams Zip Manifest Payload.</span></span>
<span data-ttu-id="20352-130">Para o arquivo zip do aplicativo do Teams, [consulte criar um pacote de aplicativos](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="20352-130">For Teams application zip file [see Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>
<span data-ttu-id="20352-131">Você não pode criar um aplicativo para uma organização que tenha a mesma ID de manifesto que outro aplicativo da organização.</span><span class="sxs-lookup"><span data-stu-id="20352-131">You can't create an app for an organization that has the same manifest ID as another app in that organization.</span></span>

## <a name="response"></a><span data-ttu-id="20352-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="20352-132">Response</span></span>

<span data-ttu-id="20352-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="20352-133">If successful, this method returns a `200 OK` response code and a [teamsCatalogApp](../resources/teamsapp.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="20352-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20352-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="20352-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20352-135">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="20352-136">Para obter informações sobre como criar um arquivo zip do aplicativo do Microsoft Teams, consulte [criar um pacote de aplicativos](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="20352-136">For information about how to create a Microsoft Teams application zip file, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

### <a name="response"></a><span data-ttu-id="20352-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="20352-137">Response</span></span>

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
