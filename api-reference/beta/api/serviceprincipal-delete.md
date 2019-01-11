---
title: Excluir servicePrincipal
description: Exclua servicePrincipal.
localization_priority: Normal
ms.openlocfilehash: 4e2cd3adeacc1e7c1f7e3c955f247800a63673b8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873833"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="8c48a-103">Excluir servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="8c48a-103">Delete servicePrincipal</span></span>

> <span data-ttu-id="8c48a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8c48a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c48a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8c48a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8c48a-106">Exclua servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="8c48a-106">Delete servicePrincipal.</span></span>
## <a name="permissions"></a><span data-ttu-id="8c48a-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="8c48a-107">Permissions</span></span>
<span data-ttu-id="8c48a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c48a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c48a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c48a-110">Permission type</span></span>      | <span data-ttu-id="8c48a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8c48a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c48a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c48a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8c48a-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8c48a-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8c48a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c48a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c48a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c48a-115">Not supported.</span></span>    |
|<span data-ttu-id="8c48a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c48a-116">Application</span></span> | <span data-ttu-id="8c48a-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c48a-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c48a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c48a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}

```
## <a name="request-headers"></a><span data-ttu-id="8c48a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c48a-119">Request headers</span></span>
| <span data-ttu-id="8c48a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8c48a-120">Name</span></span>       | <span data-ttu-id="8c48a-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c48a-121">Type</span></span> | <span data-ttu-id="8c48a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c48a-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8c48a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c48a-123">Authorization</span></span>  | <span data-ttu-id="8c48a-124">string</span><span class="sxs-lookup"><span data-stu-id="8c48a-124">string</span></span>  | <span data-ttu-id="8c48a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c48a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c48a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c48a-127">Request body</span></span>
<span data-ttu-id="8c48a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8c48a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c48a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c48a-129">Response</span></span>

<span data-ttu-id="8c48a-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c48a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c48a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c48a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8c48a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c48a-133">Request</span></span>
<span data-ttu-id="8c48a-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c48a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}
```
##### <a name="response"></a><span data-ttu-id="8c48a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c48a-135">Response</span></span>
<span data-ttu-id="8c48a-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c48a-136">Here is an example of the response.</span></span> 
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
