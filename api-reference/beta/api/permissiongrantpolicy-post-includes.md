---
title: Criar permissionGrantConditionSet na coleção de inclusões de permissionGrantPolicy
description: Adicionar condições sob as quais um evento de concessão de permissão é incluído em uma política de concessão de permissão.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: e53acd2bb17a1082384f7c7f694aea34fc3911fc
ms.sourcegitcommit: 775b38baac6a4e7704d6144ef4589f2fc476bd61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/13/2020
ms.locfileid: "48433511"
---
# <a name="create-permissiongrantconditionset-in-includes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="6722d-103">Criar permissionGrantConditionSet na coleção de inclusões de permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="6722d-103">Create permissionGrantConditionSet in includes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="6722d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6722d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6722d-105">Adicionar condições sob as quais um evento de concessão de permissão é *incluído* em uma política de concessão de permissão.</span><span class="sxs-lookup"><span data-stu-id="6722d-105">Add conditions under which a permission grant event is *included* in a permission grant policy.</span></span> <span data-ttu-id="6722d-106">Para fazer isso, adicione um [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) à coleção de **inclusões** de um  [permissionGrantPolicy](../resources/permissionGrantPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6722d-106">You do this by adding a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) to the **includes** collection of a  [permissionGrantPolicy](../resources/permissionGrantPolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6722d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6722d-107">Permissions</span></span>

<span data-ttu-id="6722d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6722d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6722d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6722d-110">Permission type</span></span>      | <span data-ttu-id="6722d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6722d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6722d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6722d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6722d-113">Policy. ReadWrite. PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="6722d-113">Policy.ReadWrite.PermissionGrant</span></span> |
|<span data-ttu-id="6722d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6722d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6722d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6722d-115">Not supported.</span></span>    |
|<span data-ttu-id="6722d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6722d-116">Application</span></span> | <span data-ttu-id="6722d-117">Policy. ReadWrite. PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="6722d-117">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="6722d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6722d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /policies/permissionGrantPolicies/{id}/includes
```

## <a name="request-headers"></a><span data-ttu-id="6722d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6722d-119">Request headers</span></span>

| <span data-ttu-id="6722d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6722d-120">Name</span></span>       | <span data-ttu-id="6722d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6722d-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="6722d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6722d-122">Authorization</span></span> | <span data-ttu-id="6722d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6722d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6722d-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="6722d-125">Content-type</span></span> | <span data-ttu-id="6722d-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6722d-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6722d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6722d-128">Request body</span></span>

<span data-ttu-id="6722d-129">No corpo da solicitação, forneça uma representação JSON de um objeto [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) .</span><span class="sxs-lookup"><span data-stu-id="6722d-129">In the request body, supply a JSON representation of an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6722d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6722d-130">Response</span></span>

<span data-ttu-id="6722d-131">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6722d-131">If successful, this method returns a `201 Created` response code and an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6722d-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6722d-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6722d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6722d-133">Request</span></span>

<span data-ttu-id="6722d-134">Neste exemplo, *todas* as permissões delegadas para aplicativos clientes de editores verificados estão incluídas na política de concessão de permissão.</span><span class="sxs-lookup"><span data-stu-id="6722d-134">In this example, *all* delegated permissions for client apps from verified publishers are included in the permission grant policy.</span></span> <span data-ttu-id="6722d-135">Como todas as outras condições do [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) foram omitidas, elas terão seus valores padrão, o que, em cada caso, é o mais inclusivo.</span><span class="sxs-lookup"><span data-stu-id="6722d-135">Because all the other conditions from the [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) were omitted, they will take their default values, which in each case is the most-inclusive.</span></span>

<!-- {
  "blockType": "request",
  "truncated": true,
  "name": "permissiongrantpolicy_create_includes"
}-->

```http
POST https://graph.microsoft.com/beta/policies/permissionGrantPolicies/{id}/includes
Content-Type: application/json

{
  "permissionType": "delegated",
  "clientApplicationsFromVerifiedPublisherOnly": true
}
```

### <a name="response"></a><span data-ttu-id="6722d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6722d-136">Response</span></span>

<span data-ttu-id="6722d-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6722d-137">The following is an example of the response.</span></span>

> <span data-ttu-id="6722d-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6722d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantConditionSet"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "75ffda85-9314-43bc-bf19-554a7d079e96",
  "permissionClassification": "all",
  "permissionType": "delegated",
  "resourceApplication": "any",
  "permissions": ["all"],
  "clientApplicationIds": ["all"],
  "clientApplicationTenantIds": ["all"],
  "clientApplicationPublisherIds": ["all"],
  "clientApplicationsFromVerifiedPublisherOnly": false
}
```
