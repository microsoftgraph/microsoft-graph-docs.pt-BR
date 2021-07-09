---
title: Listar includedGroups
description: Obter a lista de grupos incluídos em uma política de gerenciamento de aplicativo móvel.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d69156b2614b17037a6eba473d00e7d333868d6c
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351066"
---
# <a name="list-includedgroups"></a><span data-ttu-id="6c2df-103">Listar includedGroups</span><span class="sxs-lookup"><span data-stu-id="6c2df-103">List includedGroups</span></span>

<span data-ttu-id="6c2df-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c2df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c2df-105">Obter a lista de grupos incluídos em uma política de gerenciamento de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="6c2df-105">Get the list of groups that are included in a mobile app management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c2df-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6c2df-106">Permissions</span></span>

<span data-ttu-id="6c2df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c2df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c2df-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c2df-109">Permission type</span></span>|<span data-ttu-id="6c2df-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6c2df-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c2df-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c2df-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6c2df-112">Policy.Read.All, Policy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c2df-112">Policy.Read.All, Policy.ReadWrite.All</span></span>|
|<span data-ttu-id="6c2df-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c2df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c2df-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c2df-114">Not supported.</span></span>|
|<span data-ttu-id="6c2df-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c2df-115">Application</span></span> | <span data-ttu-id="6c2df-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c2df-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c2df-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c2df-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/mobileAppManagementPolicies/{id}/includedGroups
```

## <a name="request-headers"></a><span data-ttu-id="6c2df-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c2df-118">Request headers</span></span>

|<span data-ttu-id="6c2df-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6c2df-119">Name</span></span>|<span data-ttu-id="6c2df-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c2df-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6c2df-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c2df-121">Authorization</span></span>|<span data-ttu-id="6c2df-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c2df-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c2df-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c2df-124">Request body</span></span>

<span data-ttu-id="6c2df-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6c2df-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c2df-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c2df-126">Response</span></span>

<span data-ttu-id="6c2df-127">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [de](../resources/group.md) grupo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c2df-127">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6c2df-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6c2df-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6c2df-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c2df-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups
```

### <a name="response"></a><span data-ttu-id="6c2df-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c2df-130">Response</span></span>

><span data-ttu-id="6c2df-131">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6c2df-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.group)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "800c583d-cc3d-4361-8e4a-3fbf668f27f4",
      "displayName": "Test Group"
    }
  ]
}
```
