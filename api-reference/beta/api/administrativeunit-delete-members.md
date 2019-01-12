---
title: Remover um membro
description: Use essa API para remover o membro (usuário ou grupo) a partir de uma unidade administrativa.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e79dac5b7ae3a20675f6faaf9b209f8117ca2252
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941524"
---
# <a name="remove-a-member"></a><span data-ttu-id="f3121-103">Remover um membro</span><span class="sxs-lookup"><span data-stu-id="f3121-103">Remove a member</span></span>

> <span data-ttu-id="f3121-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f3121-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3121-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f3121-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f3121-106">Use essa API para remover o membro (usuário ou grupo) a partir de uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="f3121-106">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3121-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="f3121-107">Permissions</span></span>
<span data-ttu-id="f3121-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3121-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f3121-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3121-110">Permission type</span></span>      | <span data-ttu-id="f3121-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f3121-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3121-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3121-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f3121-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f3121-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f3121-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3121-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3121-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3121-115">Not supported.</span></span>    |
|<span data-ttu-id="f3121-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3121-116">Application</span></span> | <span data-ttu-id="f3121-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3121-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3121-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3121-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="f3121-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3121-119">Request headers</span></span>
| <span data-ttu-id="f3121-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f3121-120">Name</span></span>      |<span data-ttu-id="f3121-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3121-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f3121-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3121-122">Authorization</span></span>  | <span data-ttu-id="f3121-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3121-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3121-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3121-125">Request body</span></span>
<span data-ttu-id="f3121-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f3121-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3121-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3121-127">Response</span></span>

<span data-ttu-id="f3121-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3121-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3121-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3121-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f3121-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3121-131">Request</span></span>
<span data-ttu-id="f3121-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3121-132">Here is an example of the request.</span></span> <span data-ttu-id="f3121-133">No exemplo a seguir, id1 representa o identificador para a unidade administrativa de destino e ID2 da representa o identificador exclusivo para o usuário membro ou grupo a ser removido da unidade administrativa alvos.</span><span class="sxs-lookup"><span data-stu-id="f3121-133">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="f3121-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3121-134">Response</span></span>
<span data-ttu-id="f3121-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3121-135">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
