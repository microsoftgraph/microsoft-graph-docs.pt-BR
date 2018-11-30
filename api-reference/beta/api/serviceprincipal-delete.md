---
title: Excluir servicePrincipal
description: Exclua servicePrincipal.
ms.openlocfilehash: 363c6a17a7181d72214329c3e6f50433d84a1786
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036004"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="275a3-103">Excluir servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="275a3-103">Delete servicePrincipal</span></span>

> <span data-ttu-id="275a3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="275a3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="275a3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="275a3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="275a3-106">Exclua servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="275a3-106">Delete servicePrincipal.</span></span>
## <a name="permissions"></a><span data-ttu-id="275a3-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="275a3-107">Permissions</span></span>
<span data-ttu-id="275a3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="275a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="275a3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="275a3-110">Permission type</span></span>      | <span data-ttu-id="275a3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="275a3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="275a3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="275a3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="275a3-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="275a3-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="275a3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="275a3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="275a3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="275a3-115">Not supported.</span></span>    |
|<span data-ttu-id="275a3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="275a3-116">Application</span></span> | <span data-ttu-id="275a3-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="275a3-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="275a3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="275a3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}

```
## <a name="request-headers"></a><span data-ttu-id="275a3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="275a3-119">Request headers</span></span>
| <span data-ttu-id="275a3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="275a3-120">Name</span></span>       | <span data-ttu-id="275a3-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="275a3-121">Type</span></span> | <span data-ttu-id="275a3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="275a3-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="275a3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="275a3-123">Authorization</span></span>  | <span data-ttu-id="275a3-124">string</span><span class="sxs-lookup"><span data-stu-id="275a3-124">string</span></span>  | <span data-ttu-id="275a3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="275a3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="275a3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="275a3-127">Request body</span></span>
<span data-ttu-id="275a3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="275a3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="275a3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="275a3-129">Response</span></span>

<span data-ttu-id="275a3-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="275a3-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="275a3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="275a3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="275a3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="275a3-133">Request</span></span>
<span data-ttu-id="275a3-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="275a3-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}
```
##### <a name="response"></a><span data-ttu-id="275a3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="275a3-135">Response</span></span>
<span data-ttu-id="275a3-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="275a3-136">Here is an example of the response.</span></span> 
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
  "description": "Delete servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->