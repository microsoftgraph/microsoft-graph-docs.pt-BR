---
title: Adicionar um membro
description: Use essa API para adicionar um membro (usuário ou grupo) a uma unidade administrativa.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 9f3aca05107b73232b11e42ed70a9e737c65a45b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942937"
---
# <a name="add-a-member"></a><span data-ttu-id="e7de7-103">Adicionar um membro</span><span class="sxs-lookup"><span data-stu-id="e7de7-103">Add a member</span></span>

<span data-ttu-id="e7de7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7de7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7de7-105">Use essa API para adicionar um membro (usuário ou grupo) a uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="e7de7-105">Use this API to add a member (user or group) to an administrative unit.</span></span>

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a><span data-ttu-id="e7de7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e7de7-106">Permissions</span></span>
<span data-ttu-id="e7de7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7de7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e7de7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7de7-109">Permission type</span></span>      | <span data-ttu-id="e7de7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e7de7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7de7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7de7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e7de7-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e7de7-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e7de7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7de7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7de7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7de7-114">Not supported.</span></span>    |
|<span data-ttu-id="e7de7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7de7-115">Application</span></span> | <span data-ttu-id="e7de7-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7de7-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7de7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7de7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="e7de7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7de7-118">Request headers</span></span>
| <span data-ttu-id="e7de7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e7de7-119">Name</span></span>      |<span data-ttu-id="e7de7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7de7-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e7de7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7de7-121">Authorization</span></span>  | <span data-ttu-id="e7de7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7de7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7de7-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7de7-124">Request body</span></span>
<span data-ttu-id="e7de7-125">No corpo da solicitação, forneça o de um usuário , grupo ou `id` [directoryObject](../resources/directoryobject.md) a ser adicionado. [](../resources/user.md) [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="e7de7-125">In the request body, provide the `id` of a [user](../resources/user.md),  [group](../resources/group.md) or [directoryObject](../resources/directoryobject.md) to be added.</span></span>

## <a name="response"></a><span data-ttu-id="e7de7-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7de7-126">Response</span></span>

<span data-ttu-id="e7de7-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7de7-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7de7-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7de7-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="e7de7-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7de7-130">Request</span></span>
<span data-ttu-id="e7de7-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7de7-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_administrativeUnits_members"
} -->
```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
Content-type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/groups/{id}"
}

```
<span data-ttu-id="e7de7-132">No corpo da solicitação, forneça o `id` objeto [do usuário](../resources/user.md) ou grupo que você deseja adicionar. [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="e7de7-132">In the request body, provide the `id` of the [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

### <a name="response"></a><span data-ttu-id="e7de7-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7de7-133">Response</span></span>
<span data-ttu-id="e7de7-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7de7-134">Here is an example of the response.</span></span>
 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```


