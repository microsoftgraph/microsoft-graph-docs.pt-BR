---
title: Permissões
description: 'Remova o aplicativo de catálogo de aplicativos da sua organização (o catálogo de aplicativos do inquilino). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 49a45bbd8062aeea0de2d82cfae0032990af65e7
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016678"
---
# <a name="remove-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="c7719-103">Remova um aplicativo de catálogo de aplicativos da sua organização</span><span class="sxs-lookup"><span data-stu-id="c7719-103">Remove an app from your organization's app catalog</span></span>



<span data-ttu-id="c7719-104">Remova o [aplicativo](../resources/teamsapp.md) de catálogo de aplicativos da sua organização (o catálogo de aplicativos do inquilino).</span><span class="sxs-lookup"><span data-stu-id="c7719-104">Remove the [app](../resources/teamsapp.md) from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="c7719-105">Para remover o seu aplicativo de catálogo de aplicativos da sua organização, especifique `organization` como o **distributionMethod** no recurso [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="c7719-105">To remove your app from your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7719-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c7719-106">Permissions</span></span>

<span data-ttu-id="c7719-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="c7719-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="c7719-109">**Observação:** Somente os administradores globais podem chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="c7719-109">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="c7719-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7719-110">Permission Type</span></span>                        | <span data-ttu-id="c7719-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7719-111">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="c7719-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7719-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c7719-113">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7719-113">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="c7719-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7719-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7719-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c7719-115">Not supported</span></span>|
| <span data-ttu-id="c7719-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7719-116">Application</span></span>                            | <span data-ttu-id="c7719-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c7719-117">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7719-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7719-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c7719-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7719-119">Request headers</span></span>

| <span data-ttu-id="c7719-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7719-120">Header</span></span>        | <span data-ttu-id="c7719-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c7719-121">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="c7719-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7719-122">Authorization</span></span> | <span data-ttu-id="c7719-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7719-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c7719-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7719-125">Request body</span></span>

<span data-ttu-id="c7719-126">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c7719-126">None.</span></span>

><span data-ttu-id="c7719-127">**Observação:** Use a identificação retornada da chamada [lista publicada apps](./teamsapp-list.md) para referenciar o aplicativo que você gostaria de atualizar.</span><span class="sxs-lookup"><span data-stu-id="c7719-127">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="c7719-128">Não use a ID do manifesto do pacote zip app.</span><span class="sxs-lookup"><span data-stu-id="c7719-128">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="c7719-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7719-129">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="c7719-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7719-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7719-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7719-131">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a><span data-ttu-id="c7719-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7719-132">Response</span></span>

```http
HTTP/1.1 204 No Content
```
