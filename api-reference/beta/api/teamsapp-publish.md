---
title: Permissions
description: 'Publica um aplicativo para o catálogo de aplicativos do Microsoft Teams. '
ms.openlocfilehash: ae8dcf5e20da2ac18bb036ad40916496d91136f1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039565"
---
# <a name="publish-apps-to-your-organizations-app-catalog"></a><span data-ttu-id="2049e-103">Publicar aplicativos ao catálogo de aplicativos da sua organização</span><span class="sxs-lookup"><span data-stu-id="2049e-103">Publish apps to your organization's app catalog</span></span>

> <span data-ttu-id="2049e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2049e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2049e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2049e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2049e-106">Publica um [aplicativo](../resources/teamsapp.md) para o catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="2049e-106">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span> <span data-ttu-id="2049e-107">Especificamente, essa API publica o aplicativo catálogo da sua organização (o catálogo de aplicativos do inquilino); o recurso criado terá `distributionMethod`  =  `organization`.</span><span class="sxs-lookup"><span data-stu-id="2049e-107">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have `distributionMethod` = `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="2049e-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="2049e-108">Permissions</span></span>

<span data-ttu-id="2049e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="2049e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="2049e-111">**Observação:** Somente os administradores globais podem chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="2049e-111">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="2049e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2049e-112">Permission Type</span></span>                        | <span data-ttu-id="2049e-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2049e-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="2049e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2049e-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="2049e-115">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2049e-115">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="2049e-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2049e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2049e-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2049e-117">Not supported</span></span>|
| <span data-ttu-id="2049e-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2049e-118">Application</span></span>                            | <span data-ttu-id="2049e-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2049e-119">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="2049e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2049e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a><span data-ttu-id="2049e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2049e-121">Request headers</span></span>

| <span data-ttu-id="2049e-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2049e-122">Header</span></span>        | <span data-ttu-id="2049e-123">Valor</span><span class="sxs-lookup"><span data-stu-id="2049e-123">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="2049e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2049e-124">Authorization</span></span> | <span data-ttu-id="2049e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2049e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2049e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2049e-127">Content-Type</span></span>  | <span data-ttu-id="2049e-128">aplicativo/zip</span><span class="sxs-lookup"><span data-stu-id="2049e-128">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="2049e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2049e-129">Request body</span></span>

<span data-ttu-id="2049e-130">Carga de manifesto de Zip equipes.</span><span class="sxs-lookup"><span data-stu-id="2049e-130">Teams Zip Manifest Payload.</span></span> <span data-ttu-id="2049e-131">Para o aplicativo de equipes zip arquivo, [consulte Criar um pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="2049e-131">For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> <span data-ttu-id="2049e-132">Não é possível criar um aplicativo para uma organização que tem a mesma ID de manifesto do aplicativo outra organização em questão.</span><span class="sxs-lookup"><span data-stu-id="2049e-132">You can't create an app for an organization that has the same manifest ID as another app in that organization.</span></span>

## <a name="response"></a><span data-ttu-id="2049e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2049e-133">Response</span></span>

<span data-ttu-id="2049e-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="2049e-134">If successful, this method returns a `200 OK` response code and a [teamsCatalogApp](../resources/teamsapp.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="2049e-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2049e-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="2049e-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2049e-136">Request</span></span>

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="2049e-137">Para obter informações sobre como criar um arquivo do Microsoft Teams aplicativo zip, consulte [criar um pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="2049e-137">For information about how to create a Microsoft Teams application zip file, see [Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> 

### <a name="response"></a><span data-ttu-id="2049e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2049e-138">Response</span></span>

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
