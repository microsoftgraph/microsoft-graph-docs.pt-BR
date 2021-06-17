---
title: Remover um membro
description: Use essa API para remover um membro (usuário ou grupo) de uma unidade administrativa.
author: DougKirschner
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 2d79d9de1f2cf93cec62678150f564381411e0d6
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992062"
---
# <a name="remove-a-member"></a><span data-ttu-id="0cfac-103">Remover um membro</span><span class="sxs-lookup"><span data-stu-id="0cfac-103">Remove a member</span></span>

<span data-ttu-id="0cfac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cfac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cfac-105">Use essa API para remover um membro (usuário ou grupo) de uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="0cfac-105">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="0cfac-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="0cfac-106">Permissions</span></span>
<span data-ttu-id="0cfac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cfac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0cfac-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0cfac-109">Permission type</span></span>      | <span data-ttu-id="0cfac-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0cfac-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cfac-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0cfac-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0cfac-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0cfac-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0cfac-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0cfac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0cfac-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cfac-114">Not supported.</span></span>    |
|<span data-ttu-id="0cfac-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0cfac-115">Application</span></span> | <span data-ttu-id="0cfac-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cfac-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0cfac-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0cfac-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="0cfac-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0cfac-118">Request headers</span></span>
| <span data-ttu-id="0cfac-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0cfac-119">Name</span></span>      |<span data-ttu-id="0cfac-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cfac-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0cfac-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0cfac-121">Authorization</span></span>  | <span data-ttu-id="0cfac-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0cfac-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0cfac-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0cfac-124">Request body</span></span>
<span data-ttu-id="0cfac-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0cfac-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0cfac-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cfac-126">Response</span></span>

<span data-ttu-id="0cfac-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0cfac-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cfac-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0cfac-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0cfac-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0cfac-130">Request</span></span>
<span data-ttu-id="0cfac-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0cfac-131">Here is an example of the request.</span></span> <span data-ttu-id="0cfac-132">No exemplo abaixo, id1 representa o identificador da unidade administrativa de destino e o id2 representa o identificador exclusivo para o usuário membro ou grupo a ser removido da unidade administrativa de destino.</span><span class="sxs-lookup"><span data-stu-id="0cfac-132">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="0cfac-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cfac-133">Response</span></span>
<span data-ttu-id="0cfac-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0cfac-134">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```


