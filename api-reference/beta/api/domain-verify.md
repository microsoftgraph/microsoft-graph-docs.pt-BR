---
title: 'domain: verify'
description: Valida a propriedade do domínio.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e61456ccf7e47283464bddb4103a02dbfdb9bdb3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950624"
---
# <a name="domain-verify"></a><span data-ttu-id="8f417-103">domain: verify</span><span class="sxs-lookup"><span data-stu-id="8f417-103">domain: verify</span></span>

> <span data-ttu-id="8f417-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8f417-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f417-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8f417-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8f417-106">Valida a propriedade do domínio.</span><span class="sxs-lookup"><span data-stu-id="8f417-106">Validates the ownership of the domain.</span></span>

> <span data-ttu-id="8f417-p102">**Importante:** Aplica-se somente a um domínio não verificado. Para um domínio não verificado, a propriedade isVerified do [domínio](../resources/domain.md) é falsa.</span><span class="sxs-lookup"><span data-stu-id="8f417-p102">**Important:** Only applies to an unverified domain. For an unverified domain, the isVerified property of the [domain](../resources/domain.md) is false.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f417-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="8f417-109">Permissions</span></span>

<span data-ttu-id="8f417-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f417-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8f417-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f417-112">Permission type</span></span>      | <span data-ttu-id="8f417-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8f417-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f417-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f417-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8f417-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f417-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="8f417-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f417-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f417-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f417-117">Not supported.</span></span>    |
|<span data-ttu-id="8f417-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f417-118">Application</span></span> | <span data-ttu-id="8f417-119">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f417-119">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f417-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f417-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> <span data-ttu-id="8f417-121">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="8f417-121">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f417-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f417-122">Request headers</span></span>

| <span data-ttu-id="8f417-123">Nome</span><span class="sxs-lookup"><span data-stu-id="8f417-123">Name</span></span>       | <span data-ttu-id="8f417-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f417-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8f417-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f417-125">Authorization</span></span>  | <span data-ttu-id="8f417-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f417-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="8f417-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8f417-128">Content-Type</span></span>  | <span data-ttu-id="8f417-129">application/json</span><span class="sxs-lookup"><span data-stu-id="8f417-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f417-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f417-130">Request body</span></span>

## <a name="response"></a><span data-ttu-id="8f417-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f417-131">Response</span></span>

<span data-ttu-id="8f417-132">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f417-132">If successful, this method returns `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f417-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f417-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8f417-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f417-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/verify
```

##### <a name="response"></a><span data-ttu-id="8f417-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f417-135">Response</span></span>
<span data-ttu-id="8f417-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f417-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "name": "contoso.com"
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
