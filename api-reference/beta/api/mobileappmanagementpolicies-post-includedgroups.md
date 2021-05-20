---
title: Adicionar includedGroups
description: Adicione grupos a serem incluídos em uma política de gerenciamento de aplicativo móvel.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: cb589432f3ac977775af33f49f2647ad8b03be75
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547310"
---
# <a name="add-includedgroups"></a><span data-ttu-id="d1692-103">Adicionar includedGroups</span><span class="sxs-lookup"><span data-stu-id="d1692-103">Add includedGroups</span></span>

<span data-ttu-id="d1692-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1692-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1692-105">Adicione grupos a serem incluídos em uma política de gerenciamento de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="d1692-105">Add groups to be included in a mobile app management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1692-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d1692-106">Permissions</span></span>
<span data-ttu-id="d1692-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1692-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1692-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1692-109">Permission type</span></span>|<span data-ttu-id="d1692-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1692-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1692-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1692-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d1692-112">Policy.Read.All, Policy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1692-112">Policy.Read.All, Policy.ReadWrite.All</span></span>|
|<span data-ttu-id="d1692-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1692-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1692-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1692-114">Not supported.</span></span>|
|<span data-ttu-id="d1692-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1692-115">Application</span></span> | <span data-ttu-id="d1692-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1692-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1692-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1692-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /policies/mobileAppManagementPolicies/{id}/includedGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="d1692-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1692-118">Request headers</span></span>
|<span data-ttu-id="d1692-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d1692-119">Name</span></span>|<span data-ttu-id="d1692-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1692-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d1692-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1692-121">Authorization</span></span>|<span data-ttu-id="d1692-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1692-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d1692-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d1692-124">Content-Type</span></span>|<span data-ttu-id="d1692-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1692-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1692-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1692-127">Request body</span></span>
<span data-ttu-id="d1692-128">No corpo da solicitação, fornece uma representação JSON do [objeto group.](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="d1692-128">In the request body, supply a JSON representation of the [group](../resources/group.md) object.</span></span>

<span data-ttu-id="d1692-129">A tabela a seguir mostra as propriedades necessárias ao adicionar o [grupo](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="d1692-129">The following table shows the properties that are required when you add the [group](../resources/group.md).</span></span>

|<span data-ttu-id="d1692-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d1692-130">Property</span></span>|<span data-ttu-id="d1692-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1692-131">Type</span></span>|<span data-ttu-id="d1692-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1692-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1692-133">id</span><span class="sxs-lookup"><span data-stu-id="d1692-133">id</span></span>|<span data-ttu-id="d1692-134">String</span><span class="sxs-lookup"><span data-stu-id="d1692-134">String</span></span>|<span data-ttu-id="d1692-135">O identificador exclusivo do grupo.</span><span class="sxs-lookup"><span data-stu-id="d1692-135">The unique identifier for the group.</span></span>|

## <a name="response"></a><span data-ttu-id="d1692-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1692-136">Response</span></span>

<span data-ttu-id="d1692-137">Se bem-sucedido, esse método retorna um código de resposta `204 No Content` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1692-137">If successful, this method returns a `204 No Content` response code and a [group](../resources/group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d1692-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d1692-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d1692-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1692-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_group_from_groups"
}
-->

``` http
POST https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups/$ref
Content-Type: application/json

{
  "@odata.id": "https://graph.microsoft.com/odata/groups('1a9db3ab-0acf-4808-99ae-e8ed581cb2e0')"
}
```

### <a name="response"></a><span data-ttu-id="d1692-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1692-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
