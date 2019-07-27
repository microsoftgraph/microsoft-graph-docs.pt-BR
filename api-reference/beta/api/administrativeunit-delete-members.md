---
title: Remover um membro
description: Use esta API para remover um membro (usuário ou grupo) de uma unidade administrativa.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c307a802e2d574950b89c3f5644b5fbf70d90e34
ms.sourcegitcommit: 27e8ddb53b699f70b676c9648db8f06bb8d831a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/27/2019
ms.locfileid: "35917928"
---
# <a name="remove-a-member"></a><span data-ttu-id="bd4f4-103">Remover um membro</span><span class="sxs-lookup"><span data-stu-id="bd4f4-103">Remove a member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd4f4-104">Use esta API para remover um membro (usuário ou grupo) de uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="bd4f4-104">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd4f4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bd4f4-105">Permissions</span></span>
<span data-ttu-id="bd4f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd4f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bd4f4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd4f4-108">Permission type</span></span>      | <span data-ttu-id="bd4f4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bd4f4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd4f4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd4f4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bd4f4-111">AdministrativeUnit. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="bd4f4-111">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bd4f4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd4f4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd4f4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd4f4-113">Not supported.</span></span>    |
|<span data-ttu-id="bd4f4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd4f4-114">Application</span></span> | <span data-ttu-id="bd4f4-115">AdministrativeUnit. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bd4f4-115">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd4f4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd4f4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="bd4f4-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd4f4-117">Request headers</span></span>
| <span data-ttu-id="bd4f4-118">Nome</span><span class="sxs-lookup"><span data-stu-id="bd4f4-118">Name</span></span>      |<span data-ttu-id="bd4f4-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd4f4-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bd4f4-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd4f4-120">Authorization</span></span>  | <span data-ttu-id="bd4f4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd4f4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd4f4-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd4f4-123">Request body</span></span>
<span data-ttu-id="bd4f4-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bd4f4-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd4f4-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd4f4-125">Response</span></span>

<span data-ttu-id="bd4f4-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd4f4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd4f4-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bd4f4-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bd4f4-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd4f4-129">Request</span></span>
<span data-ttu-id="bd4f4-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd4f4-130">Here is an example of the request.</span></span> <span data-ttu-id="bd4f4-131">No exemplo abaixo, ID1 representa o identificador para a unidade administrativa de destino e ID2 representa o identificador exclusivo para o usuário ou grupo membro a ser removido da unidade administrativa do direcionada.</span><span class="sxs-lookup"><span data-stu-id="bd4f4-131">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="bd4f4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd4f4-132">Response</span></span>
<span data-ttu-id="bd4f4-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd4f4-133">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
