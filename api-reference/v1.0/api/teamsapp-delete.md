---
title: Excluir teamsApp
description: 'Excluir um aplicativo do teams do catálogo de aplicativos de uma organização (o catálogo de aplicativos do locatário). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 110061b252110d6b78e3b52112506d5514743299
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792650"
---
# <a name="delete-teamsapp"></a><span data-ttu-id="5ea2f-103">Excluir teamsApp</span><span class="sxs-lookup"><span data-stu-id="5ea2f-103">Delete teamsApp</span></span>

<span data-ttu-id="5ea2f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ea2f-104">Namespace: microsoft.graph</span></span>

<!-- markdownlint-disable MD001 -->
### <a name="delete-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="5ea2f-105">Excluir um aplicativo do catálogo de aplicativos da sua organização</span><span class="sxs-lookup"><span data-stu-id="5ea2f-105">Delete an app from your organization's app catalog</span></span>

<span data-ttu-id="5ea2f-106">Excluir um [aplicativo](../resources/teamsapp.md) do catálogo de aplicativos de uma organização (o catálogo de aplicativos do locatário).</span><span class="sxs-lookup"><span data-stu-id="5ea2f-106">Delete an [app](../resources/teamsapp.md) from an organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="5ea2f-107">Para excluir um aplicativo, a propriedade **distributionMethod** para o aplicativo deve ser definida como `organization` .</span><span class="sxs-lookup"><span data-stu-id="5ea2f-107">To delete an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="5ea2f-108">Você também pode usar essa API para remover um aplicativo enviado do processo de revisão.</span><span class="sxs-lookup"><span data-stu-id="5ea2f-108">You can also use this API to remove a submitted app from the review process.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ea2f-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ea2f-109">Permissions</span></span>

<span data-ttu-id="5ea2f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ea2f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="5ea2f-112">**Observação:** Somente os administradores globais podem chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5ea2f-112">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="5ea2f-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ea2f-113">Permission Type</span></span>                        | <span data-ttu-id="5ea2f-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ea2f-114">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="5ea2f-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ea2f-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="5ea2f-116">AppCatalog. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5ea2f-116">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="5ea2f-117">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ea2f-117">Delegated (work or school account)</span></span> | <span data-ttu-id="5ea2f-118">AppCatalog. Submit</span><span class="sxs-lookup"><span data-stu-id="5ea2f-118">AppCatalog.Submit</span></span> |
| <span data-ttu-id="5ea2f-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ea2f-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ea2f-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5ea2f-120">Not supported</span></span>|
| <span data-ttu-id="5ea2f-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ea2f-121">Application</span></span>                            | <span data-ttu-id="5ea2f-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ea2f-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ea2f-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ea2f-123">HTTP request</span></span>

<span data-ttu-id="5ea2f-124">Para excluir um aplicativo do catálogo de aplicativos:</span><span class="sxs-lookup"><span data-stu-id="5ea2f-124">To delete an app from the app catalog:</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

<span data-ttu-id="5ea2f-125">Para excluir um aplicativo que foi enviado, mas que não foi aprovado:</span><span class="sxs-lookup"><span data-stu-id="5ea2f-125">To delete an app that has been submitted but has not been approved:</span></span>

```http
 DELETE appCatalogs/teamsApps/{appId}/appDefinitions/{appDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="5ea2f-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ea2f-126">Request headers</span></span>

| <span data-ttu-id="5ea2f-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ea2f-127">Header</span></span>        | <span data-ttu-id="5ea2f-128">Valor</span><span class="sxs-lookup"><span data-stu-id="5ea2f-128">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="5ea2f-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ea2f-129">Authorization</span></span> | <span data-ttu-id="5ea2f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ea2f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5ea2f-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ea2f-132">Request body</span></span>

<span data-ttu-id="5ea2f-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5ea2f-133">Do not supply a request body for this method.</span></span>

><span data-ttu-id="5ea2f-134">**Observação:** Use a ID retornada da chamada [lista de aplicativos publicados](./teamsapp-list.md) para fazer referência ao aplicativo que você deseja atualizar.</span><span class="sxs-lookup"><span data-stu-id="5ea2f-134">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call to reference the app you'd like to update.</span></span> <span data-ttu-id="5ea2f-135">Não use a ID do manifesto do pacote de aplicativos zip.</span><span class="sxs-lookup"><span data-stu-id="5ea2f-135">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="5ea2f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ea2f-136">Response</span></span>

<span data-ttu-id="5ea2f-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ea2f-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ea2f-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ea2f-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ea2f-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ea2f-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_teamsapp"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```
<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="5ea2f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ea2f-141">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
