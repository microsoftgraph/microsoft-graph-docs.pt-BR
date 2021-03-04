---
title: Remover um membro
description: Use essa API para remover um membro (usuário ou grupo) de uma unidade administrativa.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 7e5662fef16966edaf0acd8986341ae9b723a5f2
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438936"
---
# <a name="remove-a-member"></a><span data-ttu-id="d3b12-103">Remover um membro</span><span class="sxs-lookup"><span data-stu-id="d3b12-103">Remove a member</span></span>

<span data-ttu-id="d3b12-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3b12-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3b12-105">Use essa API para remover um membro (usuário ou grupo) de uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="d3b12-105">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3b12-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3b12-106">Permissions</span></span>
<span data-ttu-id="d3b12-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3b12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d3b12-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3b12-109">Permission type</span></span>      | <span data-ttu-id="d3b12-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3b12-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3b12-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3b12-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d3b12-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d3b12-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d3b12-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3b12-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3b12-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3b12-114">Not supported.</span></span>    |
|<span data-ttu-id="d3b12-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3b12-115">Application</span></span> | <span data-ttu-id="d3b12-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3b12-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3b12-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3b12-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="d3b12-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3b12-118">Request headers</span></span>
| <span data-ttu-id="d3b12-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d3b12-119">Name</span></span>      |<span data-ttu-id="d3b12-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3b12-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d3b12-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3b12-121">Authorization</span></span>  | <span data-ttu-id="d3b12-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3b12-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3b12-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3b12-124">Request body</span></span>
<span data-ttu-id="d3b12-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d3b12-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3b12-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3b12-126">Response</span></span>

<span data-ttu-id="d3b12-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3b12-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3b12-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3b12-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d3b12-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3b12-130">Request</span></span>
<span data-ttu-id="d3b12-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3b12-131">Here is an example of the request.</span></span> <span data-ttu-id="d3b12-132">No exemplo abaixo, id1 representa o identificador da unidade administrativa de destino e o id2 representa o identificador exclusivo para o usuário membro ou grupo a ser removido da unidade administrativa de destino.</span><span class="sxs-lookup"><span data-stu-id="d3b12-132">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="d3b12-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3b12-133">Response</span></span>
<span data-ttu-id="d3b12-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3b12-134">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```


