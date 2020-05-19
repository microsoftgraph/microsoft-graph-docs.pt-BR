---
title: 'servicePrincipalName: Adicionar proprietário'
description: Adicione um proprietário para a entidade de serviço.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 31851eb6e4e653d1c97ba56fda8c7a80e6e5803f
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290009"
---
# <a name="serviceprincipal-add-owner"></a><span data-ttu-id="0e731-103">servicePrincipalName: Adicionar proprietário</span><span class="sxs-lookup"><span data-stu-id="0e731-103">servicePrincipal: Add owner</span></span>

<span data-ttu-id="0e731-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e731-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e731-105">Adicione um proprietário para o [servicePrincipalName](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="0e731-105">Add an owner for the [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0e731-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0e731-106">Permissions</span></span>
<span data-ttu-id="0e731-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e731-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e731-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e731-109">Permission type</span></span>      | <span data-ttu-id="0e731-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e731-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e731-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e731-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0e731-112">Application. ReadWrite. All e Directory. Read. All, Application. ReadWrite. All e Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="0e731-112">Application.ReadWrite.All and Directory.Read.All, Application.ReadWrite.All and Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0e731-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e731-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e731-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e731-114">Not supported.</span></span>    |
|<span data-ttu-id="0e731-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e731-115">Application</span></span> | <span data-ttu-id="0e731-116">Application. ReadWrite. OwnedBy e Directory. Read. All, Application. ReadWrite. All e Directory. Read. All, Application. ReadWrite. OwnedBy e Directory. ReadWrite. All, Application. ReadWrite. All e Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0e731-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All, Application.ReadWrite.OwnedBy and Directory.ReadWrite.All, Application.ReadWrite.All and Directory.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="0e731-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e731-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="0e731-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e731-118">Request headers</span></span>
| <span data-ttu-id="0e731-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0e731-119">Name</span></span>       | <span data-ttu-id="0e731-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e731-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="0e731-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e731-121">Authorization</span></span> | <span data-ttu-id="0e731-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e731-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0e731-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e731-124">Request body</span></span>
<span data-ttu-id="0e731-125">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryobject](../resources/directoryobject.md) .</span><span class="sxs-lookup"><span data-stu-id="0e731-125">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0e731-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e731-126">Response</span></span>

<span data-ttu-id="0e731-127">Se bem-sucedido, este método retorna um código de resposta `204 No Content` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e731-127">If successful, this method returns a `204 No Content` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0e731-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0e731-128">Examples</span></span>
### <a name="request"></a><span data-ttu-id="0e731-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e731-129">Request</span></span>
<span data-ttu-id="0e731-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e731-130">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_serviceprincipal"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

<span data-ttu-id="0e731-131">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryobject](../resources/directoryobject.md) .</span><span class="sxs-lookup"><span data-stu-id="0e731-131">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="0e731-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e731-132">Response</span></span>
<span data-ttu-id="0e731-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0e731-133">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
