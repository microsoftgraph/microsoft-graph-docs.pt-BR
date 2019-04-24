---
title: Criar domínio
description: Adiciona um domínio ao inquilino.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8f7c9677d4bd3dd7088f3b3d67c49fad6caa360e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454838"
---
# <a name="create-domain"></a><span data-ttu-id="b463d-103">Criar domínio</span><span class="sxs-lookup"><span data-stu-id="b463d-103">Create domain</span></span>

<span data-ttu-id="b463d-104">Adiciona um domínio ao inquilino.</span><span class="sxs-lookup"><span data-stu-id="b463d-104">Adds a domain to the tenant.</span></span>

<span data-ttu-id="b463d-p101">**Importante**: Você não pode usar um domínio associado ao seu locatário do Azure AD até que a propriedade seja verificada. Confira [Listar verificationDnsRecords](domain-list-verificationdnsrecords.md) para obter mais detalhes. Os domínios raiz exigem verificação. Por exemplo, contoso.com exige verificação. Se um domínio raiz for verificado, os subdomínios do domínio raiz serão verificados automaticamente. Por exemplo, o subdominio.contoso.com é automaticamente verificado se contoso.com for verificado.</span><span class="sxs-lookup"><span data-stu-id="b463d-p101">**Important**: You cannot use an associated domain with your Azure AD tenant until ownership is verified. See [List verificationDnsRecords](domain-list-verificationdnsrecords.md) for details. Root domains require verification. For example, contoso.com requires verification. If a root domain is verified, subdomains of the root domain are automatically verified. For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="b463d-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="b463d-111">Permissions</span></span>

<span data-ttu-id="b463d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b463d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b463d-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b463d-114">Permission type</span></span>      | <span data-ttu-id="b463d-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b463d-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b463d-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b463d-116">Delegated (work or school account)</span></span> | <span data-ttu-id="b463d-117">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b463d-117">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b463d-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b463d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b463d-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b463d-119">Not supported.</span></span>    |
|<span data-ttu-id="b463d-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b463d-120">Application</span></span> | <span data-ttu-id="b463d-121">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b463d-121">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b463d-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b463d-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains
```
## <a name="request-headers"></a><span data-ttu-id="b463d-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b463d-123">Request headers</span></span>
| <span data-ttu-id="b463d-124">Nome</span><span class="sxs-lookup"><span data-stu-id="b463d-124">Name</span></span>       | <span data-ttu-id="b463d-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b463d-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b463d-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="b463d-126">Authorization</span></span>  | <span data-ttu-id="b463d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b463d-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="b463d-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b463d-129">Content-Type</span></span>  | <span data-ttu-id="b463d-130">application/json</span><span class="sxs-lookup"><span data-stu-id="b463d-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b463d-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b463d-131">Request body</span></span>
<span data-ttu-id="b463d-132">No corpo da solicitação, forneça uma representação JSON do objeto [domain](../resources/domain.md).</span><span class="sxs-lookup"><span data-stu-id="b463d-132">In the request body, supply a JSON representation of [domain](../resources/domain.md) object.</span></span>

> <span data-ttu-id="b463d-p104">O corpo da solicitação contém a propriedade id do novo domínio. Id é a única propriedade que pode ser especificada e isso é necessário. O valor da propriedade id é o nome de domínio totalmente qualificado para criar.</span><span class="sxs-lookup"><span data-stu-id="b463d-p104">The request body contains the id property for the new domain. Id is the only property that can be specified and it is required. The id property value is the fully qualified domain name to create.</span></span>

## <a name="response"></a><span data-ttu-id="b463d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b463d-136">Response</span></span>

<span data-ttu-id="b463d-137">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b463d-137">If successful, this method returns `201 Created` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b463d-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b463d-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b463d-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b463d-139">Request</span></span>

<span data-ttu-id="b463d-140">No corpo da solicitação, forneça uma representação JSON do objeto [domain](../resources/domain.md).</span><span class="sxs-lookup"><span data-stu-id="b463d-140">In the request body, supply a JSON representation of [domain](../resources/domain.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="b463d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b463d-141">Response</span></span>
<span data-ttu-id="b463d-p105">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b463d-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
