---
title: Excluir domínio
description: Exclui um domínio de um locatário.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a870692e6a2710728dac4f2df55aaf8daf0eb95a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960123"
---
# <a name="delete-domain"></a><span data-ttu-id="c69d3-103">Excluir domínio</span><span class="sxs-lookup"><span data-stu-id="c69d3-103">Delete domain</span></span>

> <span data-ttu-id="c69d3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c69d3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c69d3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c69d3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c69d3-106">Exclui um domínio de um locatário.</span><span class="sxs-lookup"><span data-stu-id="c69d3-106">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="c69d3-107">**Importante:** Domínios excluídos não são recuperáveis.</span><span class="sxs-lookup"><span data-stu-id="c69d3-107">**Important:** Deleted domains are not recoverable.</span></span>

## <a name="permissions"></a><span data-ttu-id="c69d3-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="c69d3-108">Permissions</span></span>

<span data-ttu-id="c69d3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c69d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c69d3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c69d3-111">Permission type</span></span>      | <span data-ttu-id="c69d3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c69d3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c69d3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c69d3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c69d3-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c69d3-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c69d3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c69d3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c69d3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c69d3-116">Not supported.</span></span>    |
|<span data-ttu-id="c69d3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c69d3-117">Application</span></span> | <span data-ttu-id="c69d3-118">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c69d3-118">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c69d3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c69d3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="c69d3-120">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="c69d3-120">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c69d3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c69d3-121">Request headers</span></span>

| <span data-ttu-id="c69d3-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c69d3-122">Name</span></span>       | <span data-ttu-id="c69d3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c69d3-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c69d3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c69d3-124">Authorization</span></span>  | <span data-ttu-id="c69d3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c69d3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c69d3-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c69d3-127">Content-Type</span></span>  | <span data-ttu-id="c69d3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c69d3-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c69d3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c69d3-129">Request body</span></span>

<span data-ttu-id="c69d3-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c69d3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c69d3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c69d3-131">Response</span></span>

<span data-ttu-id="c69d3-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c69d3-p104">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="c69d3-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c69d3-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c69d3-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c69d3-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/beta/domains/contoso.com
```

##### <a name="response"></a><span data-ttu-id="c69d3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c69d3-136">Response</span></span>

<span data-ttu-id="c69d3-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c69d3-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
