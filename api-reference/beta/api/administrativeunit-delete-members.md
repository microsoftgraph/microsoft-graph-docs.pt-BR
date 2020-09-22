---
title: Remover um membro
description: Use esta API para remover um membro (usuário ou grupo) de uma unidade administrativa.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0d4763a7ab2782b33be6c254f13a852ca8f14787
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991793"
---
# <a name="remove-a-member"></a><span data-ttu-id="356bd-103">Remover um membro</span><span class="sxs-lookup"><span data-stu-id="356bd-103">Remove a member</span></span>

<span data-ttu-id="356bd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="356bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="356bd-105">Use esta API para remover um membro (usuário ou grupo) de uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="356bd-105">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="356bd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="356bd-106">Permissions</span></span>
<span data-ttu-id="356bd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="356bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="356bd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="356bd-109">Permission type</span></span>      | <span data-ttu-id="356bd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="356bd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="356bd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="356bd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="356bd-112">AdministrativeUnit. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="356bd-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="356bd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="356bd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="356bd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="356bd-114">Not supported.</span></span>    |
|<span data-ttu-id="356bd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="356bd-115">Application</span></span> | <span data-ttu-id="356bd-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="356bd-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="356bd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="356bd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="356bd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="356bd-118">Request headers</span></span>
| <span data-ttu-id="356bd-119">Nome</span><span class="sxs-lookup"><span data-stu-id="356bd-119">Name</span></span>      |<span data-ttu-id="356bd-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="356bd-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="356bd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="356bd-121">Authorization</span></span>  | <span data-ttu-id="356bd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="356bd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="356bd-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="356bd-124">Request body</span></span>
<span data-ttu-id="356bd-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="356bd-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="356bd-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="356bd-126">Response</span></span>

<span data-ttu-id="356bd-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="356bd-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="356bd-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="356bd-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="356bd-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="356bd-130">Request</span></span>
<span data-ttu-id="356bd-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="356bd-131">Here is an example of the request.</span></span> <span data-ttu-id="356bd-132">No exemplo abaixo, ID1 representa o identificador para a unidade administrativa de destino e ID2 representa o identificador exclusivo para o usuário ou grupo membro a ser removido da unidade administrativa do direcionada.</span><span class="sxs-lookup"><span data-stu-id="356bd-132">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="356bd-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="356bd-133">Response</span></span>
<span data-ttu-id="356bd-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="356bd-134">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```


