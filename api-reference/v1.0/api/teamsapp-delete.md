---
title: Permissões
description: 'Remova o aplicativo do catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7fa273be1265c4e0a236688cc4af4a3f695a1477
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021131"
---
# <a name="remove-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="9f2fb-103">Remover um aplicativo do catálogo de aplicativos da sua organização</span><span class="sxs-lookup"><span data-stu-id="9f2fb-103">Remove an app from your organization's app catalog</span></span>



<span data-ttu-id="9f2fb-104">Remova o [aplicativo](../resources/teamsapp.md) do catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário).</span><span class="sxs-lookup"><span data-stu-id="9f2fb-104">Remove the [app](../resources/teamsapp.md) from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="9f2fb-105">Para remover o aplicativo do catálogo de aplicativos da sua organização, `organization` especifique como **DistributionMethod** no recurso [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="9f2fb-105">To remove your app from your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f2fb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9f2fb-106">Permissions</span></span>

<span data-ttu-id="9f2fb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="9f2fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="9f2fb-109">**Observação:** Somente os administradores globais podem chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="9f2fb-109">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="9f2fb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f2fb-110">Permission Type</span></span>                        | <span data-ttu-id="9f2fb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9f2fb-111">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="9f2fb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f2fb-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f2fb-113">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f2fb-113">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="9f2fb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f2fb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f2fb-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9f2fb-115">Not supported</span></span>|
| <span data-ttu-id="9f2fb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f2fb-116">Application</span></span>                            | <span data-ttu-id="9f2fb-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9f2fb-117">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f2fb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f2fb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9f2fb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f2fb-119">Request headers</span></span>

| <span data-ttu-id="9f2fb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9f2fb-120">Header</span></span>        | <span data-ttu-id="9f2fb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9f2fb-121">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="9f2fb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f2fb-122">Authorization</span></span> | <span data-ttu-id="9f2fb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f2fb-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9f2fb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f2fb-125">Request body</span></span>

<span data-ttu-id="9f2fb-126">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9f2fb-126">None.</span></span>

><span data-ttu-id="9f2fb-127">**Observação:** Use o ID retornado da [lista de aplicativos publicados](./teamsapp-list.md) chamada para fazer referência ao aplicativo que você deseja atualizar.</span><span class="sxs-lookup"><span data-stu-id="9f2fb-127">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="9f2fb-128">Não use a ID do manifesto do pacote de aplicativos zip.</span><span class="sxs-lookup"><span data-stu-id="9f2fb-128">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="9f2fb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f2fb-129">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="9f2fb-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9f2fb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f2fb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f2fb-131">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a><span data-ttu-id="9f2fb-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f2fb-132">Response</span></span>

```http
HTTP/1.1 204 No Content
```
