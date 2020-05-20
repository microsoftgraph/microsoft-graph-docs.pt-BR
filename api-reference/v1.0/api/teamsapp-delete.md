---
title: Permissões
description: 'Remova o aplicativo do catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3d224b0458a26b35ba330c508eeac65bea2b068f
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290325"
---
# <a name="remove-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="165eb-103">Remover um aplicativo do catálogo de aplicativos da sua organização</span><span class="sxs-lookup"><span data-stu-id="165eb-103">Remove an app from your organization's app catalog</span></span>

<span data-ttu-id="165eb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="165eb-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="165eb-105">Remova o [aplicativo](../resources/teamsapp.md) do catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário).</span><span class="sxs-lookup"><span data-stu-id="165eb-105">Remove the [app](../resources/teamsapp.md) from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="165eb-106">Para remover o aplicativo do catálogo de aplicativos da sua organização, especifique `organization` como **distributionMethod** no recurso [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="165eb-106">To remove your app from your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="165eb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="165eb-107">Permissions</span></span>

<span data-ttu-id="165eb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="165eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="165eb-110">**Observação:** Somente os administradores globais podem chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="165eb-110">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="165eb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="165eb-111">Permission Type</span></span>                        | <span data-ttu-id="165eb-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="165eb-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="165eb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="165eb-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="165eb-114">AppCatalog. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="165eb-114">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="165eb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="165eb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="165eb-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="165eb-116">Not supported</span></span>|
| <span data-ttu-id="165eb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="165eb-117">Application</span></span>                            | <span data-ttu-id="165eb-118">AppCatalog. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="165eb-118">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="165eb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="165eb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="165eb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="165eb-120">Request headers</span></span>

| <span data-ttu-id="165eb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="165eb-121">Header</span></span>        | <span data-ttu-id="165eb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="165eb-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="165eb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="165eb-123">Authorization</span></span> | <span data-ttu-id="165eb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="165eb-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="165eb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="165eb-126">Request body</span></span>

<span data-ttu-id="165eb-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="165eb-127">None.</span></span>

><span data-ttu-id="165eb-128">**Observação:** Use o ID retornado da [lista de aplicativos publicados](./teamsapp-list.md) chamada para fazer referência ao aplicativo que você deseja atualizar.</span><span class="sxs-lookup"><span data-stu-id="165eb-128">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="165eb-129">Não use a ID do manifesto do pacote de aplicativos zip.</span><span class="sxs-lookup"><span data-stu-id="165eb-129">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="165eb-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="165eb-130">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="165eb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="165eb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="165eb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="165eb-132">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a><span data-ttu-id="165eb-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="165eb-133">Response</span></span>

```http
HTTP/1.1 204 No Content
```
