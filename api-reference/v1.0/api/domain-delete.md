---
title: Excluir domínio
description: Exclui um domínio de um locatário.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0cfcd80109640e7fc2025407ac4872906204b4d3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947152"
---
# <a name="delete-domain"></a><span data-ttu-id="344de-103">Excluir domínio</span><span class="sxs-lookup"><span data-stu-id="344de-103">Delete domain</span></span>

<span data-ttu-id="344de-104">Exclui um domínio de um locatário.</span><span class="sxs-lookup"><span data-stu-id="344de-104">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="344de-105">**Importante:**</span><span class="sxs-lookup"><span data-stu-id="344de-105">**Important:**</span></span>
> - <span data-ttu-id="344de-106">Os domínios excluídos não podem ser recuperados.</span><span class="sxs-lookup"><span data-stu-id="344de-106">Deleted domains are not recoverable.</span></span><br />
> - <span data-ttu-id="344de-p101">As tentativas de exclusão falharão se houver objetos ou recursos dependentes no domínio. Você pode encontrar todos os recursos dependentes usando a API [Listar domainNameReferences](domain-list-domainnamereferences.md).</span><span class="sxs-lookup"><span data-stu-id="344de-p101">Attempts to delete will fail if there are any resources or objects still dependent on the domain. You can find all dependent resources by using the [List domainNameReferences](domain-list-domainnamereferences.md) API.</span></span>

## <a name="permissions"></a><span data-ttu-id="344de-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="344de-109">Permissions</span></span>

<span data-ttu-id="344de-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="344de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="344de-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="344de-112">Permission type</span></span>      | <span data-ttu-id="344de-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="344de-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="344de-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="344de-114">Delegated (work or school account)</span></span> | <span data-ttu-id="344de-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="344de-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="344de-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="344de-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="344de-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="344de-117">Not supported.</span></span>    |
|<span data-ttu-id="344de-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="344de-118">Application</span></span> | <span data-ttu-id="344de-119">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="344de-119">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="344de-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="344de-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="344de-121">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="344de-121">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="344de-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="344de-122">Request headers</span></span>

| <span data-ttu-id="344de-123">Nome</span><span class="sxs-lookup"><span data-stu-id="344de-123">Name</span></span>       | <span data-ttu-id="344de-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="344de-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="344de-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="344de-125">Authorization</span></span>  | <span data-ttu-id="344de-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="344de-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="344de-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="344de-128">Content-Type</span></span>  | <span data-ttu-id="344de-129">application/json</span><span class="sxs-lookup"><span data-stu-id="344de-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="344de-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="344de-130">Request body</span></span>

<span data-ttu-id="344de-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="344de-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="344de-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="344de-132">Response</span></span>

<span data-ttu-id="344de-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="344de-p104">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="344de-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="344de-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="344de-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="344de-136">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/domains/contoso.com
```

##### <a name="response"></a><span data-ttu-id="344de-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="344de-137">Response</span></span>

<span data-ttu-id="344de-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="344de-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
