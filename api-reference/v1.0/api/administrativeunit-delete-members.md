---
title: Remover um membro
description: Use essa API para remover um membro (usuário ou grupo) de uma unidade administrativa.
author: DougKirschner
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 04783b343cd304c666ee03a8872223adef13c2c1
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991600"
---
# <a name="remove-a-member"></a><span data-ttu-id="37d5b-103">Remover um membro</span><span class="sxs-lookup"><span data-stu-id="37d5b-103">Remove a member</span></span>

<span data-ttu-id="37d5b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37d5b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="37d5b-105">Use essa API para remover um membro (usuário ou grupo) de uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="37d5b-105">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="37d5b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="37d5b-106">Permissions</span></span>
<span data-ttu-id="37d5b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37d5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="37d5b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37d5b-109">Permission type</span></span>      | <span data-ttu-id="37d5b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37d5b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37d5b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37d5b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="37d5b-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="37d5b-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="37d5b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37d5b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37d5b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37d5b-114">Not supported.</span></span>    |
|<span data-ttu-id="37d5b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37d5b-115">Application</span></span> | <span data-ttu-id="37d5b-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37d5b-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37d5b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37d5b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="37d5b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37d5b-118">Request headers</span></span>
| <span data-ttu-id="37d5b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="37d5b-119">Name</span></span>      |<span data-ttu-id="37d5b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="37d5b-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="37d5b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="37d5b-121">Authorization</span></span>  | <span data-ttu-id="37d5b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37d5b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37d5b-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37d5b-124">Request body</span></span>
<span data-ttu-id="37d5b-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="37d5b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37d5b-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="37d5b-126">Response</span></span>

<span data-ttu-id="37d5b-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37d5b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37d5b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37d5b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="37d5b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37d5b-130">Request</span></span>
<span data-ttu-id="37d5b-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37d5b-131">Here is an example of the request.</span></span> <span data-ttu-id="37d5b-132">No exemplo abaixo, id1 representa o identificador da unidade administrativa de destino e o id2 representa o identificador exclusivo para o usuário membro ou grupo a ser removido da unidade administrativa de destino.</span><span class="sxs-lookup"><span data-stu-id="37d5b-132">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="37d5b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="37d5b-133">Response</span></span>
<span data-ttu-id="37d5b-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37d5b-134">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
