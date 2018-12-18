---
title: Excluir domínio
description: Exclui um domínio de um locatário.
author: lleonard-msft
ms.openlocfilehash: eeebfb0c4c654dbfc119b4af97ccab6e27fbef91
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353050"
---
# <a name="delete-domain"></a><span data-ttu-id="e4a7a-103">Excluir domínio</span><span class="sxs-lookup"><span data-stu-id="e4a7a-103">Delete domain</span></span>

<span data-ttu-id="e4a7a-104">Exclui um domínio de um locatário.</span><span class="sxs-lookup"><span data-stu-id="e4a7a-104">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="e4a7a-105">**Importante:**</span><span class="sxs-lookup"><span data-stu-id="e4a7a-105">**Important:**</span></span>
> - <span data-ttu-id="e4a7a-106">Os domínios excluídos não podem ser recuperados.</span><span class="sxs-lookup"><span data-stu-id="e4a7a-106">Deleted domains are not recoverable.</span></span><br />
> - <span data-ttu-id="e4a7a-p101">As tentativas de exclusão falharão se houver objetos ou recursos dependentes no domínio. Você pode encontrar todos os recursos dependentes usando a API [Listar domainNameReferences](domain-list-domainnamereferences.md).</span><span class="sxs-lookup"><span data-stu-id="e4a7a-p101">Attempts to delete will fail if there are any resources or objects still dependent on the domain. You can find all dependent resources by using the [List domainNameReferences](domain-list-domainnamereferences.md) API.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4a7a-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="e4a7a-109">Permissions</span></span>

<span data-ttu-id="e4a7a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4a7a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e4a7a-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4a7a-112">Permission type</span></span>      | <span data-ttu-id="e4a7a-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e4a7a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4a7a-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4a7a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e4a7a-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e4a7a-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e4a7a-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4a7a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4a7a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4a7a-117">Not supported.</span></span>    |
|<span data-ttu-id="e4a7a-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4a7a-118">Application</span></span> | <span data-ttu-id="e4a7a-119">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4a7a-119">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4a7a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4a7a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="e4a7a-121">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="e4a7a-121">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4a7a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4a7a-122">Request headers</span></span>

| <span data-ttu-id="e4a7a-123">Nome</span><span class="sxs-lookup"><span data-stu-id="e4a7a-123">Name</span></span>       | <span data-ttu-id="e4a7a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4a7a-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e4a7a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4a7a-125">Authorization</span></span>  | <span data-ttu-id="e4a7a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4a7a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e4a7a-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e4a7a-128">Content-Type</span></span>  | <span data-ttu-id="e4a7a-129">application/json</span><span class="sxs-lookup"><span data-stu-id="e4a7a-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4a7a-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4a7a-130">Request body</span></span>

<span data-ttu-id="e4a7a-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e4a7a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4a7a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4a7a-132">Response</span></span>

<span data-ttu-id="e4a7a-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e4a7a-p104">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4a7a-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4a7a-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4a7a-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4a7a-136">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/domains/contoso.com
```

##### <a name="response"></a><span data-ttu-id="e4a7a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4a7a-137">Response</span></span>

<span data-ttu-id="e4a7a-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4a7a-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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