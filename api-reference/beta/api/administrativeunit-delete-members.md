---
title: Remover um membro
description: Use essa API para remover o membro (usuário ou grupo) a partir de uma unidade administrativa.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 09cb727c60e102786948311f10df48f9230a9dd2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865189"
---
# <a name="remove-a-member"></a><span data-ttu-id="82940-103">Remover um membro</span><span class="sxs-lookup"><span data-stu-id="82940-103">Remove a member</span></span>

> <span data-ttu-id="82940-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="82940-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="82940-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="82940-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="82940-106">Use essa API para remover o membro (usuário ou grupo) a partir de uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="82940-106">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="82940-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="82940-107">Permissions</span></span>
<span data-ttu-id="82940-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82940-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="82940-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82940-110">Permission type</span></span>      | <span data-ttu-id="82940-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="82940-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82940-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82940-112">Delegated (work or school account)</span></span> | <span data-ttu-id="82940-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="82940-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="82940-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82940-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82940-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82940-115">Not supported.</span></span>    |
|<span data-ttu-id="82940-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82940-116">Application</span></span> | <span data-ttu-id="82940-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82940-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="82940-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82940-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="82940-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82940-119">Request headers</span></span>
| <span data-ttu-id="82940-120">Nome</span><span class="sxs-lookup"><span data-stu-id="82940-120">Name</span></span>      |<span data-ttu-id="82940-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="82940-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="82940-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="82940-122">Authorization</span></span>  | <span data-ttu-id="82940-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82940-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82940-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82940-125">Request body</span></span>
<span data-ttu-id="82940-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="82940-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82940-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="82940-127">Response</span></span>

<span data-ttu-id="82940-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="82940-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82940-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82940-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="82940-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82940-131">Request</span></span>
<span data-ttu-id="82940-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="82940-132">Here is an example of the request.</span></span> <span data-ttu-id="82940-133">No exemplo a seguir, id1 representa o identificador para a unidade administrativa de destino e ID2 da representa o identificador exclusivo para o usuário membro ou grupo a ser removido da unidade administrativa alvos.</span><span class="sxs-lookup"><span data-stu-id="82940-133">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="82940-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="82940-134">Response</span></span>
<span data-ttu-id="82940-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="82940-135">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
