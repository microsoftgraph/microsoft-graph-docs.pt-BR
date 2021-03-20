---
title: Adicionar um membro
description: Use essa API para adicionar um membro (usuário ou grupo) a uma unidade administrativa.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 97c21c9b688d160f314ea31a8fe0e47dafd5778e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945526"
---
# <a name="add-a-member"></a><span data-ttu-id="dbcbc-103">Adicionar um membro</span><span class="sxs-lookup"><span data-stu-id="dbcbc-103">Add a member</span></span>

<span data-ttu-id="dbcbc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbcbc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dbcbc-105">Use essa API para adicionar um membro (usuário ou grupo) a uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="dbcbc-105">Use this API to add a member (user or group) to an administrative unit.</span></span>

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a><span data-ttu-id="dbcbc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dbcbc-106">Permissions</span></span>
<span data-ttu-id="dbcbc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbcbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dbcbc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbcbc-109">Permission type</span></span>      | <span data-ttu-id="dbcbc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dbcbc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbcbc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbcbc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dbcbc-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dbcbc-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dbcbc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbcbc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbcbc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbcbc-114">Not supported.</span></span>    |
|<span data-ttu-id="dbcbc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbcbc-115">Application</span></span> | <span data-ttu-id="dbcbc-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbcbc-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbcbc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbcbc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="dbcbc-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbcbc-118">Request headers</span></span>
| <span data-ttu-id="dbcbc-119">Nome</span><span class="sxs-lookup"><span data-stu-id="dbcbc-119">Name</span></span>      |<span data-ttu-id="dbcbc-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbcbc-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dbcbc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbcbc-121">Authorization</span></span>  | <span data-ttu-id="dbcbc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbcbc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dbcbc-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbcbc-124">Request body</span></span>
<span data-ttu-id="dbcbc-125">No corpo da solicitação, forneça o de um usuário , grupo ou `id` [directoryObject](../resources/directoryobject.md) a ser adicionado. [](../resources/user.md) [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="dbcbc-125">In the request body, provide the `id` of a [user](../resources/user.md),  [group](../resources/group.md) or [directoryObject](../resources/directoryobject.md) to be added.</span></span>

## <a name="response"></a><span data-ttu-id="dbcbc-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbcbc-126">Response</span></span>

<span data-ttu-id="dbcbc-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbcbc-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbcbc-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dbcbc-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="dbcbc-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbcbc-130">Request</span></span>
<span data-ttu-id="dbcbc-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbcbc-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_administrativeUnits_members"
} -->
```http
POST https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}/members/$ref
Content-type: application/json
Content-length: 109

{
  "@odata.id":"https://graph.microsoft.com/v1.0/groups/{id}"
}

```
<span data-ttu-id="dbcbc-132">No corpo da solicitação, forneça o `id` objeto [do usuário](../resources/user.md) ou grupo que você deseja adicionar. [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="dbcbc-132">In the request body, provide the `id` of the [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

### <a name="response"></a><span data-ttu-id="dbcbc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbcbc-133">Response</span></span>
<span data-ttu-id="dbcbc-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbcbc-134">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
