---
title: Permissões
description: 'Remova o aplicativo do catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b34e571112235e8d0f099f3ff7e69a1fa2180aa3
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345811"
---
# <a name="remove-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="2a92e-103">Remover um aplicativo do catálogo de aplicativos da sua organização</span><span class="sxs-lookup"><span data-stu-id="2a92e-103">Remove an app from your organization's app catalog</span></span>

<span data-ttu-id="2a92e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a92e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a92e-105">Remova o [aplicativo](../resources/teamsapp.md) do catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário).</span><span class="sxs-lookup"><span data-stu-id="2a92e-105">Remove the [app](../resources/teamsapp.md) from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="2a92e-106">Para remover o aplicativo do catálogo de aplicativos da sua organização, especifique `organization` como **distributionMethod** no recurso [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="2a92e-106">To remove your app from your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a92e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2a92e-107">Permissions</span></span>

<span data-ttu-id="2a92e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="2a92e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="2a92e-110">**Observação:** Somente os administradores globais podem chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2a92e-110">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="2a92e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a92e-111">Permission Type</span></span>                        | <span data-ttu-id="2a92e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2a92e-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="2a92e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a92e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="2a92e-114">AppCatalog. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2a92e-114">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="2a92e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a92e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a92e-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2a92e-116">Not supported</span></span>|
| <span data-ttu-id="2a92e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a92e-117">Application</span></span>                            | <span data-ttu-id="2a92e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a92e-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a92e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a92e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2a92e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a92e-120">Request headers</span></span>

| <span data-ttu-id="2a92e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2a92e-121">Header</span></span>        | <span data-ttu-id="2a92e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2a92e-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="2a92e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a92e-123">Authorization</span></span> | <span data-ttu-id="2a92e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a92e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2a92e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a92e-126">Request body</span></span>

<span data-ttu-id="2a92e-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2a92e-127">None.</span></span>

><span data-ttu-id="2a92e-128">**Observação:** Use o ID retornado da [lista de aplicativos publicados](./teamsapp-list.md) chamada para fazer referência ao aplicativo que você deseja atualizar.</span><span class="sxs-lookup"><span data-stu-id="2a92e-128">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="2a92e-129">Não use a ID do manifesto do pacote de aplicativos zip.</span><span class="sxs-lookup"><span data-stu-id="2a92e-129">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="2a92e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a92e-130">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="2a92e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a92e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a92e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a92e-132">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a><span data-ttu-id="2a92e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a92e-133">Response</span></span>

```http
HTTP/1.1 204 No Content
```
