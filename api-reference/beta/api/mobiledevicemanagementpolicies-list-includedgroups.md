---
title: Listar includedGroups
description: Obter a lista de grupos incluídos em uma política de gerenciamento de dispositivo móvel.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 2b83a7c797d790600aa391712e1deb70b5639cf7
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547293"
---
# <a name="list-includedgroups"></a><span data-ttu-id="b8908-103">Listar includedGroups</span><span class="sxs-lookup"><span data-stu-id="b8908-103">List includedGroups</span></span>

<span data-ttu-id="b8908-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8908-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8908-105">Obter a lista de grupos incluídos em uma política de gerenciamento de dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="b8908-105">Get the list of groups that are included in a mobile device management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8908-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8908-106">Permissions</span></span>

<span data-ttu-id="b8908-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8908-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8908-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8908-109">Permission type</span></span>|<span data-ttu-id="b8908-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8908-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8908-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8908-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b8908-112">Policy.Read.All, Policy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8908-112">Policy.Read.All, Policy.ReadWrite.All</span></span>|
|<span data-ttu-id="b8908-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8908-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8908-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8908-114">Not supported.</span></span>|
|<span data-ttu-id="b8908-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8908-115">Application</span></span> | <span data-ttu-id="b8908-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8908-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8908-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8908-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/mobileDeviceManagementPolicies/{id}/includedGroups
```

## <a name="request-headers"></a><span data-ttu-id="b8908-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8908-118">Request headers</span></span>

|<span data-ttu-id="b8908-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b8908-119">Name</span></span>|<span data-ttu-id="b8908-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8908-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b8908-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8908-121">Authorization</span></span>|<span data-ttu-id="b8908-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8908-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8908-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8908-124">Request body</span></span>

<span data-ttu-id="b8908-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8908-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8908-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8908-126">Response</span></span>

<span data-ttu-id="b8908-127">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [de](../resources/group.md) grupo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8908-127">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b8908-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b8908-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b8908-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8908-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups
```

### <a name="response"></a><span data-ttu-id="b8908-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8908-130">Response</span></span>

><span data-ttu-id="b8908-131">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b8908-131">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "id": "dc3d2ce5-7c5e-4dca-a0ef-2145bf6e53ef",
      "displayName": "Test MDM Group"
    }
  ]
}
```
