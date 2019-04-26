---
title: Permissões
description: 'Remova o aplicativo do catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 49a45bbd8062aeea0de2d82cfae0032990af65e7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549010"
---
# <a name="remove-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="60b50-103">Remover um aplicativo do catálogo de aplicativos da sua organização</span><span class="sxs-lookup"><span data-stu-id="60b50-103">Remove an app from your organization's app catalog</span></span>



<span data-ttu-id="60b50-104">Remova o [aplicativo](../resources/teamsapp.md) do catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário).</span><span class="sxs-lookup"><span data-stu-id="60b50-104">Remove the [app](../resources/teamsapp.md) from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="60b50-105">Para remover o aplicativo do catálogo de aplicativos da sua organização, `organization` especifique como **DistributionMethod** no recurso [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="60b50-105">To remove your app from your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="60b50-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="60b50-106">Permissions</span></span>

<span data-ttu-id="60b50-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="60b50-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="60b50-109">**Observação:** Somente os administradores globais podem chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="60b50-109">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="60b50-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60b50-110">Permission Type</span></span>                        | <span data-ttu-id="60b50-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60b50-111">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="60b50-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60b50-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="60b50-113">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60b50-113">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="60b50-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60b50-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60b50-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="60b50-115">Not supported</span></span>|
| <span data-ttu-id="60b50-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60b50-116">Application</span></span>                            | <span data-ttu-id="60b50-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="60b50-117">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="60b50-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60b50-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="60b50-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60b50-119">Request headers</span></span>

| <span data-ttu-id="60b50-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="60b50-120">Header</span></span>        | <span data-ttu-id="60b50-121">Valor</span><span class="sxs-lookup"><span data-stu-id="60b50-121">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="60b50-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="60b50-122">Authorization</span></span> | <span data-ttu-id="60b50-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60b50-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="60b50-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60b50-125">Request body</span></span>

<span data-ttu-id="60b50-126">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="60b50-126">None.</span></span>

><span data-ttu-id="60b50-127">**Observação:** Use o ID retornado da [lista de aplicativos publicados](./teamsapp-list.md) chamada para fazer referência ao aplicativo que você deseja atualizar.</span><span class="sxs-lookup"><span data-stu-id="60b50-127">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="60b50-128">Não use a ID do manifesto do pacote de aplicativos zip.</span><span class="sxs-lookup"><span data-stu-id="60b50-128">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="60b50-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="60b50-129">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="60b50-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60b50-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="60b50-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60b50-131">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a><span data-ttu-id="60b50-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="60b50-132">Response</span></span>

```http
HTTP/1.1 204 No Content
```
