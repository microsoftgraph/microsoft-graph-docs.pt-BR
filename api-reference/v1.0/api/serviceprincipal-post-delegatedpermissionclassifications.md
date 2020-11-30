---
title: Criar delegatedPermissionClassification
description: Classificar uma permissão adicionando um delegatedPermissionClassification à entidade de serviço da API.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 22512ad7a61d528d22535156c1ac882b73950f72
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377140"
---
# <a name="create-delegatedpermissionclassification"></a><span data-ttu-id="5af88-103">Criar delegatedPermissionClassification</span><span class="sxs-lookup"><span data-stu-id="5af88-103">Create delegatedPermissionClassification</span></span>

<span data-ttu-id="5af88-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5af88-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5af88-105">Classificar uma permissão delegada adicionando um [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) ao [servicePrincipalName](../resources/servicePrincipal.md) que representa a API.</span><span class="sxs-lookup"><span data-stu-id="5af88-105">Classify a delegated permission by adding a [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) to the [servicePrincipal](../resources/servicePrincipal.md) representing the API.</span></span>

## <a name="permissions"></a><span data-ttu-id="5af88-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="5af88-106">Permissions</span></span>

<span data-ttu-id="5af88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5af88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5af88-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5af88-109">Permission type</span></span>      | <span data-ttu-id="5af88-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5af88-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5af88-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5af88-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5af88-112">PermissionGrantPolicy. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5af88-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
|<span data-ttu-id="5af88-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5af88-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5af88-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5af88-114">Not supported.</span></span>    |
|<span data-ttu-id="5af88-115">Application</span><span class="sxs-lookup"><span data-stu-id="5af88-115">Application</span></span> | <span data-ttu-id="5af88-116">PermissionGrantPolicy. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5af88-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5af88-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5af88-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/delegatedPermissionClassifications
```

## <a name="request-headers"></a><span data-ttu-id="5af88-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5af88-118">Request headers</span></span>

| <span data-ttu-id="5af88-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5af88-119">Name</span></span>       | <span data-ttu-id="5af88-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5af88-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="5af88-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5af88-121">Authorization</span></span> | <span data-ttu-id="5af88-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5af88-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5af88-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="5af88-124">Content-type</span></span> | <span data-ttu-id="5af88-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5af88-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5af88-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5af88-127">Request body</span></span>

<span data-ttu-id="5af88-128">No corpo da solicitação, forneça uma representação JSON de um objeto [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) .</span><span class="sxs-lookup"><span data-stu-id="5af88-128">In the request body, supply a JSON representation of an [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5af88-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5af88-129">Response</span></span>

<span data-ttu-id="5af88-130">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5af88-130">If successful, this method returns a `201 Created` response code and an [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5af88-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5af88-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5af88-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5af88-132">Request</span></span>

<span data-ttu-id="5af88-133">No exemplo a seguir, a permissão delegada "User. Read" está sendo classificada como "Low".</span><span class="sxs-lookup"><span data-stu-id="5af88-133">In the following example, the delegated permission "User.Read" is being classified "low".</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_create_delegatedpermissionclassification"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/delegatedPermissionClassifications
Content-Type: application/json

{
  "permissionId": "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
  "permissionName": "User.Read",
  "classification": "low"
}
```

### <a name="response"></a><span data-ttu-id="5af88-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5af88-134">Response</span></span>

<span data-ttu-id="5af88-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5af88-135">The following is an example of the response.</span></span>

> <span data-ttu-id="5af88-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5af88-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
