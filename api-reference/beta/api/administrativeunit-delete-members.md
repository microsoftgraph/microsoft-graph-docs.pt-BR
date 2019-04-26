---
title: Remover um membro
description: Use esta API para remover um membro (usuário ou grupo) de uma unidade administrativa.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9c605f9c77a715c8754edf3d83f7997e7cc4e865
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322982"
---
# <a name="remove-a-member"></a><span data-ttu-id="49050-103">Remover um membro</span><span class="sxs-lookup"><span data-stu-id="49050-103">Remove a member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49050-104">Use esta API para remover um membro (usuário ou grupo) de uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="49050-104">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="49050-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="49050-105">Permissions</span></span>
<span data-ttu-id="49050-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49050-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="49050-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49050-108">Permission type</span></span>      | <span data-ttu-id="49050-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="49050-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49050-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49050-110">Delegated (work or school account)</span></span> | <span data-ttu-id="49050-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="49050-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="49050-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49050-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49050-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49050-113">Not supported.</span></span>    |
|<span data-ttu-id="49050-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49050-114">Application</span></span> | <span data-ttu-id="49050-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49050-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49050-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49050-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="49050-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49050-117">Request headers</span></span>
| <span data-ttu-id="49050-118">Nome</span><span class="sxs-lookup"><span data-stu-id="49050-118">Name</span></span>      |<span data-ttu-id="49050-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="49050-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="49050-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="49050-120">Authorization</span></span>  | <span data-ttu-id="49050-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49050-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49050-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49050-123">Request body</span></span>
<span data-ttu-id="49050-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="49050-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49050-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="49050-125">Response</span></span>

<span data-ttu-id="49050-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49050-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49050-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49050-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49050-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49050-129">Request</span></span>
<span data-ttu-id="49050-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49050-130">Here is an example of the request.</span></span> <span data-ttu-id="49050-131">No exemplo abaixo, ID1 representa o identificador para a unidade administrativa de destino e ID2 representa o identificador exclusivo para o usuário ou grupo membro a ser removido da unidade administrativa do direcionada.</span><span class="sxs-lookup"><span data-stu-id="49050-131">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="49050-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="49050-132">Response</span></span>
<span data-ttu-id="49050-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49050-133">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
