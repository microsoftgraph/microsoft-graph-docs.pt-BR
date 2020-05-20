---
title: Excluir o servicePrincipalName
description: Exclua o servicePrincipalName.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: ff4806499b2c32b88ee87f6a1e33691e25f4f25a
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291164"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="4100d-103">Excluir o servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="4100d-103">Delete servicePrincipal</span></span>

<span data-ttu-id="4100d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4100d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4100d-105">Excluir um objeto [servicePrincipalName](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="4100d-105">Delete a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4100d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4100d-106">Permissions</span></span>
<span data-ttu-id="4100d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4100d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4100d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4100d-109">Permission type</span></span>      | <span data-ttu-id="4100d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4100d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4100d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4100d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4100d-112">Application. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="4100d-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4100d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4100d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4100d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4100d-114">Not supported.</span></span>    |
|<span data-ttu-id="4100d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4100d-115">Application</span></span> | <span data-ttu-id="4100d-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4100d-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4100d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4100d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}

```
## <a name="request-headers"></a><span data-ttu-id="4100d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4100d-118">Request headers</span></span>
| <span data-ttu-id="4100d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4100d-119">Name</span></span>       | <span data-ttu-id="4100d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4100d-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="4100d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4100d-121">Authorization</span></span> | <span data-ttu-id="4100d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4100d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4100d-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="4100d-124">Content-type</span></span> | <span data-ttu-id="4100d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4100d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4100d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4100d-127">Request body</span></span>
<span data-ttu-id="4100d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4100d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4100d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4100d-129">Response</span></span>

<span data-ttu-id="4100d-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4100d-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4100d-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4100d-132">Examples</span></span>
### <a name="request"></a><span data-ttu-id="4100d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4100d-133">Request</span></span>
<span data-ttu-id="4100d-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4100d-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}
```
### <a name="response"></a><span data-ttu-id="4100d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4100d-135">Response</span></span>
<span data-ttu-id="4100d-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4100d-136">Here is an example of the response.</span></span> 
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
