---
title: Permissões
description: 'Remova o aplicativo do catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4b3565e88e229c1909e189ea9eee9ce53d257066
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290718"
---
# <a name="remove-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="7fddf-103">Remover um aplicativo do catálogo de aplicativos da sua organização</span><span class="sxs-lookup"><span data-stu-id="7fddf-103">Remove an app from your organization's app catalog</span></span>

<span data-ttu-id="7fddf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fddf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7fddf-105">Remova o [aplicativo](../resources/teamsapp.md) do catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário).</span><span class="sxs-lookup"><span data-stu-id="7fddf-105">Remove the [app](../resources/teamsapp.md) from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="7fddf-106">Para remover o aplicativo do catálogo de aplicativos da sua organização, especifique `organization` como **distributionMethod** no recurso [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="7fddf-106">To remove your app from your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="7fddf-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7fddf-107">Permissions</span></span>

<span data-ttu-id="7fddf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="7fddf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="7fddf-110">**Observação:** Somente os administradores globais podem chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7fddf-110">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="7fddf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7fddf-111">Permission Type</span></span>                        | <span data-ttu-id="7fddf-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7fddf-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="7fddf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7fddf-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7fddf-114">AppCatalog. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7fddf-114">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="7fddf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7fddf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fddf-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7fddf-116">Not supported</span></span>|
| <span data-ttu-id="7fddf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7fddf-117">Application</span></span>                            | <span data-ttu-id="7fddf-118">Directory. ReadWrite. All, AppCatalog. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7fddf-118">Directory.ReadWrite.All, AppCatalog.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fddf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7fddf-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7fddf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7fddf-120">Request headers</span></span>

| <span data-ttu-id="7fddf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7fddf-121">Header</span></span>        | <span data-ttu-id="7fddf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7fddf-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="7fddf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7fddf-123">Authorization</span></span> | <span data-ttu-id="7fddf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7fddf-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7fddf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7fddf-126">Request body</span></span>

<span data-ttu-id="7fddf-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7fddf-127">None.</span></span>

><span data-ttu-id="7fddf-128">**Observação:** Use o ID retornado da [lista de aplicativos publicados](./teamsapp-list.md) chamada para fazer referência ao aplicativo que você deseja atualizar.</span><span class="sxs-lookup"><span data-stu-id="7fddf-128">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="7fddf-129">Não use a ID do manifesto do pacote de aplicativos zip.</span><span class="sxs-lookup"><span data-stu-id="7fddf-129">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="7fddf-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fddf-130">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="7fddf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7fddf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7fddf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7fddf-132">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a><span data-ttu-id="7fddf-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fddf-133">Response</span></span>

```http
HTTP/1.1 204 No Content
```
