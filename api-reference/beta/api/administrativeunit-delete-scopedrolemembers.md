---
title: Remover um scopedRoleMember
description: Remova um membro da função com escopo de uma unidade administrativas.
author: lleonard-msft
ms.openlocfilehash: 0c312266b672a93d58723fd39a26cf7bd48bd7f4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303000"
---
# <a name="remove-a-scopedrolemember"></a><span data-ttu-id="01c65-103">Remover um scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="01c65-103">Remove a scopedRoleMember</span></span>

> <span data-ttu-id="01c65-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="01c65-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01c65-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="01c65-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="01c65-106">Remova um membro da função com escopo de uma unidade administrativas.</span><span class="sxs-lookup"><span data-stu-id="01c65-106">Remove a scoped-role member from an adminstrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="01c65-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="01c65-107">Permissions</span></span>
<span data-ttu-id="01c65-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01c65-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="01c65-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01c65-110">Permission type</span></span>      | <span data-ttu-id="01c65-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="01c65-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01c65-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01c65-112">Delegated (work or school account)</span></span> | <span data-ttu-id="01c65-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="01c65-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="01c65-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01c65-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01c65-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01c65-115">Not supported.</span></span>    |
|<span data-ttu-id="01c65-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01c65-116">Application</span></span> | <span data-ttu-id="01c65-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01c65-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="01c65-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01c65-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/scopedRoleMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="01c65-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01c65-119">Request headers</span></span>
| <span data-ttu-id="01c65-120">Nome</span><span class="sxs-lookup"><span data-stu-id="01c65-120">Name</span></span>       | <span data-ttu-id="01c65-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="01c65-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="01c65-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="01c65-122">Authorization</span></span>  | <span data-ttu-id="01c65-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01c65-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01c65-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01c65-125">Request body</span></span>
<span data-ttu-id="01c65-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="01c65-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01c65-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="01c65-127">Response</span></span>

<span data-ttu-id="01c65-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01c65-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01c65-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01c65-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01c65-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01c65-131">Request</span></span>
<span data-ttu-id="01c65-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01c65-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_scopedrolemember"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
##### <a name="response"></a><span data-ttu-id="01c65-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="01c65-133">Response</span></span>
<span data-ttu-id="01c65-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01c65-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->