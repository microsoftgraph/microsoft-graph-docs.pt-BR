---
title: Criar domínio
description: Adiciona um domínio ao inquilino.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: fd4f9ffe35ff7c04b2a5aefb3bd27042229304c6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441939"
---
# <a name="create-domain"></a><span data-ttu-id="9444f-103">Criar domínio</span><span class="sxs-lookup"><span data-stu-id="9444f-103">Create domain</span></span>

<span data-ttu-id="9444f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9444f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9444f-105">Adiciona um domínio ao inquilino.</span><span class="sxs-lookup"><span data-stu-id="9444f-105">Adds a domain to the tenant.</span></span>

<span data-ttu-id="9444f-p101">**Importante**: Você não pode usar um domínio associado ao seu locatário do Azure AD até que a propriedade seja verificada. Confira [Listar verificationDnsRecords](domain-list-verificationdnsrecords.md) para obter mais detalhes. Os domínios raiz exigem verificação. Por exemplo, contoso.com exige verificação. Se um domínio raiz for verificado, os subdomínios do domínio raiz serão verificados automaticamente. Por exemplo, o subdominio.contoso.com é automaticamente verificado se contoso.com for verificado.</span><span class="sxs-lookup"><span data-stu-id="9444f-p101">**Important**: You cannot use an associated domain with your Azure AD tenant until ownership is verified. See [List verificationDnsRecords](domain-list-verificationdnsrecords.md) for details. Root domains require verification. For example, contoso.com requires verification. If a root domain is verified, subdomains of the root domain are automatically verified. For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="9444f-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="9444f-112">Permissions</span></span>

<span data-ttu-id="9444f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9444f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9444f-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9444f-115">Permission type</span></span>      | <span data-ttu-id="9444f-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9444f-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9444f-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9444f-117">Delegated (work or school account)</span></span> | <span data-ttu-id="9444f-118">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9444f-118">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9444f-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9444f-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9444f-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9444f-120">Not supported.</span></span>    |
|<span data-ttu-id="9444f-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9444f-121">Application</span></span> | <span data-ttu-id="9444f-122">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9444f-122">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9444f-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9444f-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains
```
## <a name="request-headers"></a><span data-ttu-id="9444f-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9444f-124">Request headers</span></span>
| <span data-ttu-id="9444f-125">Nome</span><span class="sxs-lookup"><span data-stu-id="9444f-125">Name</span></span>       | <span data-ttu-id="9444f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="9444f-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9444f-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="9444f-127">Authorization</span></span>  | <span data-ttu-id="9444f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9444f-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="9444f-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9444f-130">Content-Type</span></span>  | <span data-ttu-id="9444f-131">application/json</span><span class="sxs-lookup"><span data-stu-id="9444f-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9444f-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9444f-132">Request body</span></span>
<span data-ttu-id="9444f-133">No corpo da solicitação, forneça uma representação JSON do objeto [domain](../resources/domain.md).</span><span class="sxs-lookup"><span data-stu-id="9444f-133">In the request body, supply a JSON representation of [domain](../resources/domain.md) object.</span></span>

> <span data-ttu-id="9444f-p104">O corpo da solicitação contém a propriedade id do novo domínio. Id é a única propriedade que pode ser especificada e isso é necessário. O valor da propriedade id é o nome de domínio totalmente qualificado para criar.</span><span class="sxs-lookup"><span data-stu-id="9444f-p104">The request body contains the id property for the new domain. Id is the only property that can be specified and it is required. The id property value is the fully qualified domain name to create.</span></span>

## <a name="response"></a><span data-ttu-id="9444f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="9444f-137">Response</span></span>

<span data-ttu-id="9444f-138">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9444f-138">If successful, this method returns `201 Created` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9444f-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9444f-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9444f-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9444f-140">Request</span></span>

<span data-ttu-id="9444f-141">No corpo da solicitação, forneça uma representação JSON do objeto [domain](../resources/domain.md).</span><span class="sxs-lookup"><span data-stu-id="9444f-141">In the request body, supply a JSON representation of [domain](../resources/domain.md) object.</span></span>

<!-- {
  "blockType": "request",
  "id": "create_domain_from_domains"
}-->
```http
POST https://graph.microsoft.com/v1.0/domains
Content-type: application/json
Content-length: 192

{
  "id": "contoso.com"
}
```

##### <a name="response"></a><span data-ttu-id="9444f-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="9444f-142">Response</span></span>
<span data-ttu-id="9444f-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9444f-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

