---
title: Excluir política
description: Excluir uma política.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: d86f4011df727ec31e2c054e0fa2ea10736ca9e5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455526"
---
# <a name="delete-policy"></a><span data-ttu-id="090da-103">Excluir política</span><span class="sxs-lookup"><span data-stu-id="090da-103">Delete Policy</span></span>

<span data-ttu-id="090da-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="090da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="090da-105">Excluir uma [política](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="090da-105">Delete a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="090da-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="090da-106">Permissions</span></span>
<span data-ttu-id="090da-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="090da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="090da-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="090da-109">Permission type</span></span>      | <span data-ttu-id="090da-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="090da-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="090da-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="090da-111">Delegated (work or school account)</span></span> | <span data-ttu-id="090da-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="090da-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="090da-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="090da-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="090da-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="090da-114">Not supported.</span></span>    |
|<span data-ttu-id="090da-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="090da-115">Application</span></span> | <span data-ttu-id="090da-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="090da-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="090da-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="090da-117">HTTP request</span></span>

```http
DELETE /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="090da-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="090da-118">Request headers</span></span>
| <span data-ttu-id="090da-119">Nome</span><span class="sxs-lookup"><span data-stu-id="090da-119">Name</span></span>       | <span data-ttu-id="090da-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="090da-120">Type</span></span> | <span data-ttu-id="090da-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="090da-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="090da-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="090da-122">Authorization</span></span>  | <span data-ttu-id="090da-123">string</span><span class="sxs-lookup"><span data-stu-id="090da-123">string</span></span>  | <span data-ttu-id="090da-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="090da-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="090da-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="090da-126">Request body</span></span>
<span data-ttu-id="090da-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="090da-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="090da-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="090da-128">Response</span></span>

<span data-ttu-id="090da-129">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="090da-129">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="090da-130">Se não tiver êxito...</span><span class="sxs-lookup"><span data-stu-id="090da-130">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="090da-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="090da-131">Example</span></span>
<span data-ttu-id="090da-132">O exemplo a seguir exclui uma política.</span><span class="sxs-lookup"><span data-stu-id="090da-132">The following example deletes a policy.</span></span>

##### <a name="request"></a><span data-ttu-id="090da-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="090da-133">Request</span></span>
<span data-ttu-id="090da-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="090da-134">Here is an example of the request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="090da-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="090da-135">Response</span></span>
<span data-ttu-id="090da-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="090da-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
