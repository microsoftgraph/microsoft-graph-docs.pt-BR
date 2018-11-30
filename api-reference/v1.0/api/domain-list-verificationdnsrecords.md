---
title: Listar verificationDnsRecords
description: Recupere uma lista de objetos domainDnsRecord.
ms.openlocfilehash: 30927afe7fdf6e3e2b90847289a73ec2ea590fa4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006820"
---
# <a name="list-verificationdnsrecords"></a><span data-ttu-id="7c61c-103">Listar verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="7c61c-103">List verificationDnsRecords</span></span>

<span data-ttu-id="7c61c-104">Recupere uma lista de objetos [domainDnsRecord](../resources/domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="7c61c-104">Retrieve a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects.</span></span>

<span data-ttu-id="7c61c-p101">Você não pode usar um domínio associado ao seu locatário do Azure AD até que a propriedade seja verificada. Para verificar a propriedade do domínio, recupere os registros de verificação de domínio e adicione os detalhes ao arquivo de zona do domínio. Isso pode ser feito por meio da configuração do servidor DNS ou do registrador de domínios.</span><span class="sxs-lookup"><span data-stu-id="7c61c-p101">You cannot use an associated domain with your Azure AD tenant until ownership is verified. To verify the ownership of the domain, retrieve the domain verification records and add the details to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

<span data-ttu-id="7c61c-p102">Os domínios raiz exigem verificação. Por exemplo, contoso.com exige verificação. Se um domínio raiz for verificado, os subdomínios do domínio raiz serão verificados automaticamente. Por exemplo, o subdominio.contoso.com é automaticamente verificado se contoso.com for verificado.</span><span class="sxs-lookup"><span data-stu-id="7c61c-p102">Root domains require verification. For example, contoso.com requires verification. If a root domain is verified, subdomains of the root domain are automatically verified. For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c61c-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="7c61c-112">Permissions</span></span>

<span data-ttu-id="7c61c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c61c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7c61c-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c61c-115">Permission type</span></span>      | <span data-ttu-id="7c61c-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7c61c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c61c-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c61c-117">Delegated (work or school account)</span></span> | <span data-ttu-id="7c61c-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c61c-118">Directory.Read.All</span></span>    |
|<span data-ttu-id="7c61c-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c61c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c61c-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c61c-120">Not supported.</span></span>    |
|<span data-ttu-id="7c61c-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c61c-121">Application</span></span> | <span data-ttu-id="7c61c-122">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c61c-122">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c61c-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c61c-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/verificationDnsRecords
```

> <span data-ttu-id="7c61c-124">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="7c61c-124">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="7c61c-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7c61c-125">Optional query parameters</span></span>

<span data-ttu-id="7c61c-126">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7c61c-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c61c-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c61c-127">Request headers</span></span>

| <span data-ttu-id="7c61c-128">Nome</span><span class="sxs-lookup"><span data-stu-id="7c61c-128">Name</span></span>      |<span data-ttu-id="7c61c-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c61c-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7c61c-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c61c-130">Authorization</span></span>  | <span data-ttu-id="7c61c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c61c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7c61c-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7c61c-133">Content-Type</span></span>  | <span data-ttu-id="7c61c-134">application/json</span><span class="sxs-lookup"><span data-stu-id="7c61c-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c61c-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c61c-135">Request body</span></span>

<span data-ttu-id="7c61c-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7c61c-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c61c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c61c-137">Response</span></span>

<span data-ttu-id="7c61c-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [domainDnsRecord](../resources/domaindnsrecord.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c61c-138">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c61c-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c61c-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7c61c-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c61c-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_verificationdnsrecords"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/verificationDnsRecords
```

##### <a name="response"></a><span data-ttu-id="7c61c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c61c-141">Response</span></span>

<span data-ttu-id="7c61c-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7c61c-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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