---
title: Excluir política
description: Excluir uma política.
localization_priority: Normal
ms.openlocfilehash: 6467259fc0cca067deb25bc561ddf18f54760e92
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337457"
---
# <a name="delete-policy"></a><span data-ttu-id="ac4e8-103">Excluir política</span><span class="sxs-lookup"><span data-stu-id="ac4e8-103">Delete Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac4e8-104">Excluir uma [política](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="ac4e8-104">Delete a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ac4e8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ac4e8-105">Permissions</span></span>
<span data-ttu-id="ac4e8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac4e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac4e8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac4e8-108">Permission type</span></span>      | <span data-ttu-id="ac4e8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ac4e8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac4e8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac4e8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ac4e8-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ac4e8-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ac4e8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac4e8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac4e8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac4e8-113">Not supported.</span></span>    |
|<span data-ttu-id="ac4e8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac4e8-114">Application</span></span> | <span data-ttu-id="ac4e8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac4e8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac4e8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac4e8-116">HTTP request</span></span>

```http
DELETE /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ac4e8-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac4e8-117">Request headers</span></span>
| <span data-ttu-id="ac4e8-118">Nome</span><span class="sxs-lookup"><span data-stu-id="ac4e8-118">Name</span></span>       | <span data-ttu-id="ac4e8-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac4e8-119">Type</span></span> | <span data-ttu-id="ac4e8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac4e8-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ac4e8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac4e8-121">Authorization</span></span>  | <span data-ttu-id="ac4e8-122">string</span><span class="sxs-lookup"><span data-stu-id="ac4e8-122">string</span></span>  | <span data-ttu-id="ac4e8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac4e8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac4e8-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac4e8-125">Request body</span></span>
<span data-ttu-id="ac4e8-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ac4e8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac4e8-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac4e8-127">Response</span></span>

<span data-ttu-id="ac4e8-128">Quando é bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ac4e8-128">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="ac4e8-129">Se não tiver êxito...</span><span class="sxs-lookup"><span data-stu-id="ac4e8-129">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="ac4e8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac4e8-130">Example</span></span>
<span data-ttu-id="ac4e8-131">O exemplo a seguir exclui uma política.</span><span class="sxs-lookup"><span data-stu-id="ac4e8-131">The following example deletes a policy.</span></span>

##### <a name="request"></a><span data-ttu-id="ac4e8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac4e8-132">Request</span></span>
<span data-ttu-id="ac4e8-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac4e8-133">Here is an example of the request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="ac4e8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac4e8-134">Response</span></span>
<span data-ttu-id="ac4e8-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ac4e8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
