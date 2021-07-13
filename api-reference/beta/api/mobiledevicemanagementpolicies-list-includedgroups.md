---
title: Listar includedGroups
description: Obter a lista de grupos incluídos em uma política de gerenciamento de dispositivo móvel.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 9f29a263601958820d69fe51f146d34eb5a079c6
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401453"
---
# <a name="list-includedgroups"></a><span data-ttu-id="71cb5-103">Listar includedGroups</span><span class="sxs-lookup"><span data-stu-id="71cb5-103">List includedGroups</span></span>

<span data-ttu-id="71cb5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71cb5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71cb5-105">Obter a lista de grupos incluídos em uma política de gerenciamento de dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="71cb5-105">Get the list of groups that are included in a mobile device management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="71cb5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="71cb5-106">Permissions</span></span>

<span data-ttu-id="71cb5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71cb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71cb5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71cb5-109">Permission type</span></span>|<span data-ttu-id="71cb5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="71cb5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71cb5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71cb5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="71cb5-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="71cb5-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="71cb5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71cb5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71cb5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71cb5-114">Not supported.</span></span>|
|<span data-ttu-id="71cb5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71cb5-115">Application</span></span> | <span data-ttu-id="71cb5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71cb5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71cb5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71cb5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/mobileDeviceManagementPolicies/{id}/includedGroups
```

## <a name="request-headers"></a><span data-ttu-id="71cb5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71cb5-118">Request headers</span></span>

|<span data-ttu-id="71cb5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="71cb5-119">Name</span></span>|<span data-ttu-id="71cb5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="71cb5-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="71cb5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="71cb5-121">Authorization</span></span>|<span data-ttu-id="71cb5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71cb5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71cb5-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71cb5-124">Request body</span></span>

<span data-ttu-id="71cb5-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="71cb5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71cb5-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="71cb5-126">Response</span></span>

<span data-ttu-id="71cb5-127">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [de](../resources/group.md) grupo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71cb5-127">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="71cb5-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="71cb5-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="71cb5-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71cb5-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups
```

### <a name="response"></a><span data-ttu-id="71cb5-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="71cb5-130">Response</span></span>

><span data-ttu-id="71cb5-131">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="71cb5-131">**Note:** The response object shown here might be shortened for readability.</span></span>
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
