---
title: Listar verificationDnsRecords
description: Recupere uma lista de objetos domainDnsRecord.
author: lleonard-msft
ms.openlocfilehash: 4beaac56892a33a5b5dfe46e2739b933d1598c45
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323251"
---
# <a name="list-verificationdnsrecords"></a><span data-ttu-id="d37b4-103">Listar verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="d37b4-103">List verificationDnsRecords</span></span>

> <span data-ttu-id="d37b4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d37b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d37b4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d37b4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d37b4-106">Recupere uma lista de objetos [domainDnsRecord](../resources/domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="d37b4-106">Retrieve a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects.</span></span>

<span data-ttu-id="d37b4-p102">Você não pode usar um domínio associado ao seu locatário do Azure AD até que a propriedade seja verificada. Para verificar a propriedade do domínio, recupere os registros de verificação de domínio e adicione os detalhes ao arquivo de zona do domínio. Isso pode ser feito por meio da configuração do servidor DNS ou do registrador de domínios.</span><span class="sxs-lookup"><span data-stu-id="d37b4-p102">You cannot use an associated domain with your Azure AD tenant until ownership is verified. To verify the ownership of the domain, retrieve the domain verification records and add the details to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

<span data-ttu-id="d37b4-p103">Os domínios raiz exigem verificação. Por exemplo, contoso.com exige verificação. Se um domínio raiz for verificado, os subdomínios do domínio raiz serão verificados automaticamente. Por exemplo, o subdominio.contoso.com é automaticamente verificado se contoso.com for verificado.</span><span class="sxs-lookup"><span data-stu-id="d37b4-p103">Root domains require verification. For example, contoso.com requires verification. If a root domain is verified, subdomains of the root domain are automatically verified. For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="d37b4-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="d37b4-114">Permissions</span></span>

<span data-ttu-id="d37b4-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d37b4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d37b4-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d37b4-117">Permission type</span></span>      | <span data-ttu-id="d37b4-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d37b4-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d37b4-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d37b4-119">Delegated (work or school account)</span></span> | <span data-ttu-id="d37b4-120">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d37b4-120">Directory.Read.All</span></span>    |
|<span data-ttu-id="d37b4-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d37b4-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d37b4-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d37b4-122">Not supported.</span></span>    |
|<span data-ttu-id="d37b4-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d37b4-123">Application</span></span> | <span data-ttu-id="d37b4-124">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d37b4-124">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d37b4-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d37b4-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/verificationDnsRecords
```

> <span data-ttu-id="d37b4-126">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="d37b4-126">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="d37b4-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d37b4-127">Optional query parameters</span></span>

<span data-ttu-id="d37b4-128">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d37b4-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d37b4-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d37b4-129">Request headers</span></span>

| <span data-ttu-id="d37b4-130">Nome</span><span class="sxs-lookup"><span data-stu-id="d37b4-130">Name</span></span>      |<span data-ttu-id="d37b4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d37b4-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d37b4-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="d37b4-132">Authorization</span></span>  | <span data-ttu-id="d37b4-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d37b4-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d37b4-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d37b4-135">Content-Type</span></span>  | <span data-ttu-id="d37b4-136">application/json</span><span class="sxs-lookup"><span data-stu-id="d37b4-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d37b4-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d37b4-137">Request body</span></span>

<span data-ttu-id="d37b4-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d37b4-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d37b4-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d37b4-139">Response</span></span>

<span data-ttu-id="d37b4-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [domainDnsRecord](../resources/domaindnsrecord.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d37b4-140">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d37b4-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d37b4-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d37b4-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d37b4-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_verificationdnsrecords"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com/verificationDnsRecords
```

##### <a name="response"></a><span data-ttu-id="d37b4-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d37b4-143">Response</span></span>

<span data-ttu-id="d37b4-p106">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d37b4-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domainDnsRecord",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 220

{
  "value": [
    {
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Mx",
      "supportedService": "Email",
      "ttl": 3600,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List verificationDnsRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->