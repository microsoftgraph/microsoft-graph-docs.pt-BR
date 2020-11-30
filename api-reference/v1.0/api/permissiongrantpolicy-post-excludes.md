---
title: Criar permissionGrantConditionSet na coleção Excludes de permissionGrantPolicy
description: Adicionar condições sob as quais um evento de concessão de permissão é excluído em uma política de concessão de permissão.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 9011d194e0de5f0efea0d5a483219896b0f71073
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377121"
---
# <a name="create-permissiongrantconditionset-in-excludes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="1734b-103">Criar permissionGrantConditionSet na coleção Excludes de permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="1734b-103">Create permissionGrantConditionSet in excludes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="1734b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1734b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1734b-105">Adicionar condições sob as quais um evento de concessão de permissão é *excluído* em uma política de concessão de permissão.</span><span class="sxs-lookup"><span data-stu-id="1734b-105">Add conditions under which a permission grant event is *excluded* in a permission grant policy.</span></span> <span data-ttu-id="1734b-106">Para fazer isso, adicione um [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) à coleção **Excludes** de um  [permissionGrantPolicy](../resources/permissionGrantPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1734b-106">You do this by adding a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) to the **excludes** collection of a  [permissionGrantPolicy](../resources/permissionGrantPolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1734b-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="1734b-107">Permissions</span></span>

<span data-ttu-id="1734b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1734b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1734b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1734b-110">Permission type</span></span>      | <span data-ttu-id="1734b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1734b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1734b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1734b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1734b-113">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="1734b-113">Policy.ReadWrite.PermissionGrant</span></span> |
|<span data-ttu-id="1734b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1734b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1734b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1734b-115">Not supported.</span></span>    |
|<span data-ttu-id="1734b-116">Application</span><span class="sxs-lookup"><span data-stu-id="1734b-116">Application</span></span> | <span data-ttu-id="1734b-117">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="1734b-117">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="1734b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1734b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /policies/permissionGrantPolicies/{id}/excludes
```

## <a name="request-headers"></a><span data-ttu-id="1734b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1734b-119">Request headers</span></span>

| <span data-ttu-id="1734b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1734b-120">Name</span></span>       | <span data-ttu-id="1734b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1734b-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="1734b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1734b-122">Authorization</span></span> | <span data-ttu-id="1734b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1734b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1734b-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="1734b-125">Content-type</span></span> | <span data-ttu-id="1734b-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1734b-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1734b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1734b-128">Request body</span></span>

<span data-ttu-id="1734b-129">No corpo da solicitação, forneça uma representação JSON de um objeto [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) .</span><span class="sxs-lookup"><span data-stu-id="1734b-129">In the request body, supply a JSON representation of an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1734b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1734b-130">Response</span></span>

<span data-ttu-id="1734b-131">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1734b-131">If successful, this method returns a `201 Created` response code and an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1734b-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1734b-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1734b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1734b-133">Request</span></span>

<span data-ttu-id="1734b-134">Neste exemplo, *todas* as permissões delegadas para o Microsoft Graph (**AppID** 00000003-0000-0000-C000-000000000000) são excluídas da política de concessão de permissão.</span><span class="sxs-lookup"><span data-stu-id="1734b-134">In this example, *all* delegated permissions for Microsoft Graph (**appId** 00000003-0000-0000-c000-000000000000) are excluded from the permission grant policy.</span></span>

<!-- {
  "blockType": "request",
  "truncated": true,
  "name": "permissiongrantpolicy_create_excludes"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/my-custom-consent-policy/excludes
Content-Type: application/json

{
  "permissionType": "delegated",
  "resourceApplication": "00000003-0000-0000-c000-000000000000"
}
```

### <a name="response"></a><span data-ttu-id="1734b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1734b-135">Response</span></span>

<span data-ttu-id="1734b-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1734b-136">The following is an example of the response.</span></span>

> <span data-ttu-id="1734b-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1734b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantConditionSet"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "9a532f49-e646-405d-8c7c-d4c8e8a4d294",
  "permissionClassification": "all",
  "permissionType": "delegated",
  "resourceApplication": "00000003-0000-0000-c000-000000000000",
  "permissions": ["all"],
  "clientApplicationIds": ["all"],
  "clientApplicationTenantIds": ["all"],
  "clientApplicationPublisherIds": ["all"],
  "clientApplicationsFromVerifiedPublisherOnly": false
}
```
