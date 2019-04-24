---
title: 'domain: verify'
description: Valida a propriedade do domínio.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c4289e6c67844238460be9e706b8ff2f51c55035
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454852"
---
# <a name="domain-verify"></a><span data-ttu-id="f4150-103">domain: verify</span><span class="sxs-lookup"><span data-stu-id="f4150-103">domain: verify</span></span>

<span data-ttu-id="f4150-104">Valida a propriedade do domínio.</span><span class="sxs-lookup"><span data-stu-id="f4150-104">Validates the ownership of the domain.</span></span>

> <span data-ttu-id="f4150-p101">**Importante:** Aplica-se somente a um domínio não verificado. Para um domínio não verificado, a propriedade isVerified do [domínio](../resources/domain.md) é falsa.</span><span class="sxs-lookup"><span data-stu-id="f4150-p101">**Important:** Only applies to an unverified domain. For an unverified domain, the isVerified property of the [domain](../resources/domain.md) is false.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4150-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f4150-107">Permissions</span></span>

<span data-ttu-id="f4150-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4150-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f4150-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4150-110">Permission type</span></span>      | <span data-ttu-id="f4150-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f4150-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4150-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4150-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f4150-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4150-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="f4150-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4150-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4150-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4150-115">Not supported.</span></span>    |
|<span data-ttu-id="f4150-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4150-116">Application</span></span> | <span data-ttu-id="f4150-117">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4150-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4150-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4150-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> <span data-ttu-id="f4150-119">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="f4150-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4150-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4150-120">Request headers</span></span>

| <span data-ttu-id="f4150-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f4150-121">Name</span></span>       | <span data-ttu-id="f4150-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4150-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f4150-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4150-123">Authorization</span></span>  | <span data-ttu-id="f4150-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4150-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="f4150-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f4150-126">Content-Type</span></span>  | <span data-ttu-id="f4150-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f4150-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4150-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4150-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="f4150-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4150-129">Response</span></span>

<span data-ttu-id="f4150-130">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4150-130">If successful, this method returns `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4150-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4150-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f4150-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4150-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/v1.0/domains/{domain-name}/verify
```

##### <a name="response"></a><span data-ttu-id="f4150-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4150-133">Response</span></span>
<span data-ttu-id="f4150-p104">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f4150-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "id": "contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: verify",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
