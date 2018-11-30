---
title: Excluir administrativeUnit
description: Exclua um administrativeUnit.
ms.openlocfilehash: 6cb1885193e03da027d8d7680c0e5f33ec7f7d2b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034345"
---
# <a name="delete-administrativeunit"></a><span data-ttu-id="66f1c-103">Excluir administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="66f1c-103">Delete administrativeUnit</span></span>

> <span data-ttu-id="66f1c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="66f1c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66f1c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="66f1c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="66f1c-106">Exclua um [administrativeUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="66f1c-106">Delete an [administrativeUnit](../resources/administrativeunit.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="66f1c-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="66f1c-107">Permissions</span></span>
<span data-ttu-id="66f1c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66f1c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="66f1c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66f1c-110">Permission type</span></span>      | <span data-ttu-id="66f1c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66f1c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66f1c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66f1c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="66f1c-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="66f1c-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="66f1c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66f1c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66f1c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66f1c-115">Not supported.</span></span>    |
|<span data-ttu-id="66f1c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66f1c-116">Application</span></span> | <span data-ttu-id="66f1c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66f1c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="66f1c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66f1c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}

```
## <a name="request-headers"></a><span data-ttu-id="66f1c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66f1c-119">Request headers</span></span>
| <span data-ttu-id="66f1c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="66f1c-120">Name</span></span>       | <span data-ttu-id="66f1c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="66f1c-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="66f1c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="66f1c-122">Authorization</span></span>  | <span data-ttu-id="66f1c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66f1c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66f1c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66f1c-125">Request body</span></span>
<span data-ttu-id="66f1c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="66f1c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66f1c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="66f1c-127">Response</span></span>

<span data-ttu-id="66f1c-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66f1c-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66f1c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66f1c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="66f1c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66f1c-131">Request</span></span>
<span data-ttu-id="66f1c-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="66f1c-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_administrativeunit"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}
```
##### <a name="response"></a><span data-ttu-id="66f1c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="66f1c-133">Response</span></span>
<span data-ttu-id="66f1c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66f1c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
