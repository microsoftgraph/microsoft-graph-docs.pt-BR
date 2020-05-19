---
title: Excluir o servicePrincipalName
description: Exclua o servicePrincipalName.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 2731a23dea3de57d588ceec304a1155a6c09a34d
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291283"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="c88ec-103">Excluir o servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="c88ec-103">Delete servicePrincipal</span></span>

<span data-ttu-id="c88ec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c88ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c88ec-105">Excluir um objeto [servicePrincipalName](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="c88ec-105">Delete a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c88ec-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c88ec-106">Permissions</span></span>
<span data-ttu-id="c88ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c88ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c88ec-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c88ec-109">Permission type</span></span>      | <span data-ttu-id="c88ec-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c88ec-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c88ec-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c88ec-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c88ec-112">Application. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="c88ec-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="c88ec-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c88ec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c88ec-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c88ec-114">Not supported.</span></span>    |
|<span data-ttu-id="c88ec-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c88ec-115">Application</span></span> | <span data-ttu-id="c88ec-116">Application. ReadWrite. OwnedBy, Application. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c88ec-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c88ec-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c88ec-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}

```
## <a name="request-headers"></a><span data-ttu-id="c88ec-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c88ec-118">Request headers</span></span>
| <span data-ttu-id="c88ec-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c88ec-119">Name</span></span>       | <span data-ttu-id="c88ec-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="c88ec-120">Type</span></span> | <span data-ttu-id="c88ec-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c88ec-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c88ec-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c88ec-122">Authorization</span></span>  | <span data-ttu-id="c88ec-123">string</span><span class="sxs-lookup"><span data-stu-id="c88ec-123">string</span></span>  | <span data-ttu-id="c88ec-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c88ec-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c88ec-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c88ec-126">Request body</span></span>
<span data-ttu-id="c88ec-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c88ec-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c88ec-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c88ec-128">Response</span></span>

<span data-ttu-id="c88ec-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c88ec-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c88ec-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c88ec-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="c88ec-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c88ec-132">Request</span></span>
<span data-ttu-id="c88ec-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c88ec-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}
```
### <a name="response"></a><span data-ttu-id="c88ec-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c88ec-134">Response</span></span>
<span data-ttu-id="c88ec-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c88ec-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
