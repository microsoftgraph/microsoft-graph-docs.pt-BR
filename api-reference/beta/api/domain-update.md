---
title: Atualizar domínio
description: Atualize as propriedades do objeto de domínio.
ms.openlocfilehash: 38a4baca42b22465ba2ea98081b7619d5f8af0e1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035883"
---
# <a name="update-domain"></a><span data-ttu-id="1aa9e-103">Atualizar domínio</span><span class="sxs-lookup"><span data-stu-id="1aa9e-103">Update domain</span></span>

> <span data-ttu-id="1aa9e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1aa9e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1aa9e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1aa9e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1aa9e-106">Atualize as propriedades do objeto de domínio.</span><span class="sxs-lookup"><span data-stu-id="1aa9e-106">Update the properties of domain object.</span></span>

> <span data-ttu-id="1aa9e-107">**Importante:** Somente domínios verificados podem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="1aa9e-107">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="1aa9e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1aa9e-108">Permissions</span></span>

<span data-ttu-id="1aa9e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1aa9e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1aa9e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1aa9e-111">Permission type</span></span>      | <span data-ttu-id="1aa9e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1aa9e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1aa9e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1aa9e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1aa9e-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1aa9e-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1aa9e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1aa9e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1aa9e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1aa9e-116">Not supported.</span></span>    |
|<span data-ttu-id="1aa9e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1aa9e-117">Application</span></span> | <span data-ttu-id="1aa9e-118">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1aa9e-118">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1aa9e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1aa9e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="1aa9e-120">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="1aa9e-120">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1aa9e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1aa9e-121">Request headers</span></span>

| <span data-ttu-id="1aa9e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1aa9e-122">Name</span></span>       | <span data-ttu-id="1aa9e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1aa9e-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1aa9e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1aa9e-124">Authorization</span></span>  | <span data-ttu-id="1aa9e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1aa9e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1aa9e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1aa9e-127">Content-Type</span></span>  | <span data-ttu-id="1aa9e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1aa9e-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1aa9e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1aa9e-129">Request body</span></span>

<span data-ttu-id="1aa9e-p104">No corpo da solicitação, forneça os valores para os campos relevantes que serão atualizados. As propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade. Para obter melhor desempenho, somente inclua valores alterados.</span><span class="sxs-lookup"><span data-stu-id="1aa9e-p104">In the request body, supply the values for relevant fields to be updated. Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="1aa9e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1aa9e-133">Response</span></span>

<span data-ttu-id="1aa9e-134">Se bem-sucedido, este método retorna o código de resposta `204 No Content` e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1aa9e-134">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="1aa9e-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1aa9e-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1aa9e-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1aa9e-136">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/beta/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="1aa9e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1aa9e-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->