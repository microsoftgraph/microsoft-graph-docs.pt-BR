---
title: Criar delegatedPermissionClassification
description: Classificar uma permissão adicionando um delegatedPermissionClassification à entidade de serviço da API.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 79e5b3985e8bffab1613cbe0cc4b81eb27d49d6a
ms.sourcegitcommit: 775b38baac6a4e7704d6144ef4589f2fc476bd61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/13/2020
ms.locfileid: "48433491"
---
# <a name="create-delegatedpermissionclassification"></a><span data-ttu-id="c9d77-103">Criar delegatedPermissionClassification</span><span class="sxs-lookup"><span data-stu-id="c9d77-103">Create delegatedPermissionClassification</span></span>

<span data-ttu-id="c9d77-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9d77-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9d77-105">Classificar uma permissão delegada adicionando um [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) ao [servicePrincipalName](../resources/servicePrincipal.md) que representa a API.</span><span class="sxs-lookup"><span data-stu-id="c9d77-105">Classify a delegated permission by adding a [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) to the [servicePrincipal](../resources/servicePrincipal.md) representing the API.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9d77-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c9d77-106">Permissions</span></span>

<span data-ttu-id="c9d77-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9d77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9d77-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9d77-109">Permission type</span></span>      | <span data-ttu-id="c9d77-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c9d77-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9d77-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9d77-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c9d77-112">PermissionGrantPolicy. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c9d77-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
|<span data-ttu-id="c9d77-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9d77-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9d77-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9d77-114">Not supported.</span></span>    |
|<span data-ttu-id="c9d77-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9d77-115">Application</span></span> | <span data-ttu-id="c9d77-116">PermissionGrantPolicy. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c9d77-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9d77-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9d77-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/delegatedPermissionClassifications
```

## <a name="request-headers"></a><span data-ttu-id="c9d77-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9d77-118">Request headers</span></span>

| <span data-ttu-id="c9d77-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c9d77-119">Name</span></span>       | <span data-ttu-id="c9d77-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9d77-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="c9d77-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9d77-121">Authorization</span></span> | <span data-ttu-id="c9d77-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9d77-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c9d77-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="c9d77-124">Content-type</span></span> | <span data-ttu-id="c9d77-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9d77-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9d77-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9d77-127">Request body</span></span>

<span data-ttu-id="c9d77-128">No corpo da solicitação, forneça uma representação JSON de um objeto [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) .</span><span class="sxs-lookup"><span data-stu-id="c9d77-128">In the request body, supply a JSON representation of an [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c9d77-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9d77-129">Response</span></span>

<span data-ttu-id="c9d77-130">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9d77-130">If successful, this method returns a `201 Created` response code and an [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c9d77-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c9d77-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c9d77-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9d77-132">Request</span></span>

<span data-ttu-id="c9d77-133">No exemplo a seguir, a permissão delegada "User. Read" está sendo classificada como "Low".</span><span class="sxs-lookup"><span data-stu-id="c9d77-133">In the following example, the delegated permission "User.Read" is being classified "low".</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_create_delegatedpermissionclassification"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/delegatedPermissionClassifications
Content-Type: application/json

{
  "permissionId": "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
  "permissionName": "User.Read",
  "classification": "low"
}
```

### <a name="response"></a><span data-ttu-id="c9d77-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9d77-134">Response</span></span>

<span data-ttu-id="c9d77-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c9d77-135">The following is an example of the response.</span></span>

> <span data-ttu-id="c9d77-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c9d77-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.delegatedPermissionClassification"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "2G3-4TG6YU2J54hjnaRoPQE",
  "permissionId": "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
  "permissionName": "User.Read",
  "classification": "low"
}
```
