---
title: Adicionar um membro
description: Use esta API para adicionar um membro (usuário ou grupo) a uma unidade administrativa.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 91767a0d83fe35363879045cc703fb564806d228
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123262"
---
# <a name="add-a-member"></a><span data-ttu-id="54911-103">Adicionar um membro</span><span class="sxs-lookup"><span data-stu-id="54911-103">Add a member</span></span>

<span data-ttu-id="54911-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54911-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54911-105">Use esta API para adicionar um membro (usuário ou grupo) a uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="54911-105">Use this API to add a member (user or group) to an administrative unit.</span></span>

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a><span data-ttu-id="54911-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="54911-106">Permissions</span></span>
<span data-ttu-id="54911-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54911-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="54911-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54911-109">Permission type</span></span>      | <span data-ttu-id="54911-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="54911-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54911-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54911-111">Delegated (work or school account)</span></span> | <span data-ttu-id="54911-112">AdministrativeUnit. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="54911-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="54911-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54911-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54911-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54911-114">Not supported.</span></span>    |
|<span data-ttu-id="54911-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54911-115">Application</span></span> | <span data-ttu-id="54911-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54911-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="54911-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54911-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="54911-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54911-118">Request headers</span></span>
| <span data-ttu-id="54911-119">Nome</span><span class="sxs-lookup"><span data-stu-id="54911-119">Name</span></span>      |<span data-ttu-id="54911-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="54911-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="54911-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="54911-121">Authorization</span></span>  | <span data-ttu-id="54911-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54911-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54911-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54911-124">Request body</span></span>
<span data-ttu-id="54911-125">No corpo da solicitação, forneça o `id` de um [usuário](../resources/user.md), [grupo](../resources/group.md) ou [directoryobject](../resources/directoryobject.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="54911-125">In the request body, provide the `id` of a [user](../resources/user.md),  [group](../resources/group.md) or [directoryObject](../resources/directoryobject.md) to be added.</span></span>

## <a name="response"></a><span data-ttu-id="54911-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="54911-126">Response</span></span>

<span data-ttu-id="54911-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54911-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54911-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54911-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="54911-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54911-130">Request</span></span>
<span data-ttu-id="54911-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="54911-131">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
Content-type: application/json
Content-length: 109

{
  "@odata.id":"https://graph.microsoft.com/beta/groups/{id}"
}

```
<span data-ttu-id="54911-132">No corpo da solicitação, forneça o `id` do objeto [User](../resources/user.md) ou [Group](../resources/group.md) que você deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="54911-132">In the request body, provide the `id` of the [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

##### <a name="response"></a><span data-ttu-id="54911-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="54911-133">Response</span></span>
<span data-ttu-id="54911-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54911-134">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
