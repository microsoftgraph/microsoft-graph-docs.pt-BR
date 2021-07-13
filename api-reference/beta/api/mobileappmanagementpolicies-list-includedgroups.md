---
title: Listar includedGroups
description: Obter a lista de grupos incluídos em uma política de gerenciamento de aplicativo móvel.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 26cbec0d2fe976045a320a80fe3a69a53fbc74f6
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401663"
---
# <a name="list-includedgroups"></a><span data-ttu-id="b1526-103">Listar includedGroups</span><span class="sxs-lookup"><span data-stu-id="b1526-103">List includedGroups</span></span>

<span data-ttu-id="b1526-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1526-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1526-105">Obter a lista de grupos incluídos em uma política de gerenciamento de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="b1526-105">Get the list of groups that are included in a mobile app management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1526-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b1526-106">Permissions</span></span>

<span data-ttu-id="b1526-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1526-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1526-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1526-109">Permission type</span></span>|<span data-ttu-id="b1526-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b1526-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1526-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1526-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b1526-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="b1526-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="b1526-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1526-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1526-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1526-114">Not supported.</span></span>|
|<span data-ttu-id="b1526-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1526-115">Application</span></span> | <span data-ttu-id="b1526-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1526-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1526-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1526-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/mobileAppManagementPolicies/{id}/includedGroups
```

## <a name="request-headers"></a><span data-ttu-id="b1526-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1526-118">Request headers</span></span>

|<span data-ttu-id="b1526-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b1526-119">Name</span></span>|<span data-ttu-id="b1526-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1526-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b1526-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1526-121">Authorization</span></span>|<span data-ttu-id="b1526-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1526-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1526-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1526-124">Request body</span></span>

<span data-ttu-id="b1526-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b1526-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1526-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1526-126">Response</span></span>

<span data-ttu-id="b1526-127">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [de](../resources/group.md) grupo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1526-127">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b1526-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b1526-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b1526-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1526-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups
```

### <a name="response"></a><span data-ttu-id="b1526-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1526-130">Response</span></span>

><span data-ttu-id="b1526-131">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b1526-131">**Note:** The response object shown here might be shortened for readability.</span></span>
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
