---
title: Criar domínio
description: Adiciona um domínio ao inquilino.
author: lleonard-msft
ms.openlocfilehash: eae00bb3da0321d5c06d0fc3e4dc76e3ac410589
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308887"
---
# <a name="create-domain"></a><span data-ttu-id="bf38c-103">Criar domínio</span><span class="sxs-lookup"><span data-stu-id="bf38c-103">Create domain</span></span>

> <span data-ttu-id="bf38c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bf38c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf38c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bf38c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bf38c-106">Adiciona um domínio ao inquilino.</span><span class="sxs-lookup"><span data-stu-id="bf38c-106">Adds a domain to the tenant.</span></span>

<span data-ttu-id="bf38c-p102">**Importante**: Você não pode usar um domínio associado ao seu locatário do Azure AD até que a propriedade seja verificada. Confira [Listar verificationDnsRecords](domain-list-verificationdnsrecords.md) para obter mais detalhes. Os domínios raiz exigem verificação. Por exemplo, contoso.com exige verificação. Se um domínio raiz for verificado, os subdomínios do domínio raiz serão verificados automaticamente. Por exemplo, o subdominio.contoso.com é automaticamente verificado se contoso.com for verificado.</span><span class="sxs-lookup"><span data-stu-id="bf38c-p102">**Important**: You cannot use an associated domain with your Azure AD tenant until ownership is verified. See [List verificationDnsRecords](domain-list-verificationdnsrecords.md) for details. Root domains require verification. For example, contoso.com requires verification. If a root domain is verified, subdomains of the root domain are automatically verified. For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf38c-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="bf38c-113">Permissions</span></span>

<span data-ttu-id="bf38c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf38c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bf38c-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf38c-116">Permission type</span></span>      | <span data-ttu-id="bf38c-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bf38c-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf38c-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf38c-118">Delegated (work or school account)</span></span> | <span data-ttu-id="bf38c-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bf38c-119">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bf38c-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf38c-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf38c-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf38c-121">Not supported.</span></span>    |
|<span data-ttu-id="bf38c-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf38c-122">Application</span></span> | <span data-ttu-id="bf38c-123">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf38c-123">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf38c-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf38c-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains
```
## <a name="request-headers"></a><span data-ttu-id="bf38c-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf38c-125">Request headers</span></span>
| <span data-ttu-id="bf38c-126">Nome</span><span class="sxs-lookup"><span data-stu-id="bf38c-126">Name</span></span>       | <span data-ttu-id="bf38c-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf38c-127">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bf38c-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf38c-128">Authorization</span></span>  | <span data-ttu-id="bf38c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf38c-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="bf38c-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bf38c-131">Content-Type</span></span>  | <span data-ttu-id="bf38c-132">application/json</span><span class="sxs-lookup"><span data-stu-id="bf38c-132">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bf38c-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf38c-133">Request body</span></span>
<span data-ttu-id="bf38c-134">No corpo da solicitação, forneça uma representação JSON do objeto [domain](../resources/domain.md).</span><span class="sxs-lookup"><span data-stu-id="bf38c-134">In the request body, supply a JSON representation of [domain](../resources/domain.md) object.</span></span>

> <span data-ttu-id="bf38c-p105">O corpo da solicitação contém a propriedade id do novo domínio. Id é a única propriedade que pode ser especificada e isso é necessário. O valor da propriedade id é o nome de domínio totalmente qualificado para criar.</span><span class="sxs-lookup"><span data-stu-id="bf38c-p105">The request body contains the id property for the new domain. Id is the only property that can be specified and it is required. The id property value is the fully qualified domain name to create.</span></span>

## <a name="response"></a><span data-ttu-id="bf38c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf38c-138">Response</span></span>

<span data-ttu-id="bf38c-139">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf38c-139">If successful, this method returns `201 Created` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf38c-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf38c-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bf38c-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf38c-141">Request</span></span>

<span data-ttu-id="bf38c-142">No corpo da solicitação, forneça uma representação JSON do objeto [domain](../resources/domain.md).</span><span class="sxs-lookup"><span data-stu-id="bf38c-142">In the request body, supply a JSON representation of [domain](../resources/domain.md) object.</span></span>

<!-- {
  "blockType": "request",
  "id": "create_domain_from_domains"
}-->
```http
POST https://graph.microsoft.com/beta/domains
Content-type: application/json
Content-length: 192

{
  "id": "contoso.com"
}
```

##### <a name="response"></a><span data-ttu-id="bf38c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf38c-143">Response</span></span>
<span data-ttu-id="bf38c-p106">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bf38c-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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