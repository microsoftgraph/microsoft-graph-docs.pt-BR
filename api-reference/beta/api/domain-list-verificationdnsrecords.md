---
title: Listar verificationDnsRecords
description: Recupere uma lista de objetos domainDnsRecord.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a470f6bddb9cade8083afb3eb5d5cf76cf4dba32
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522837"
---
# <a name="list-verificationdnsrecords"></a><span data-ttu-id="2109d-103">Listar verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="2109d-103">List verificationDnsRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2109d-104">Recupere uma lista de objetos [domainDnsRecord](../resources/domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="2109d-104">Retrieve a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects.</span></span>

<span data-ttu-id="2109d-p101">Você não pode usar um domínio associado ao seu locatário do Azure AD até que a propriedade seja verificada. Para verificar a propriedade do domínio, recupere os registros de verificação de domínio e adicione os detalhes ao arquivo de zona do domínio. Isso pode ser feito por meio da configuração do servidor DNS ou do registrador de domínios.</span><span class="sxs-lookup"><span data-stu-id="2109d-p101">You cannot use an associated domain with your Azure AD tenant until ownership is verified. To verify the ownership of the domain, retrieve the domain verification records and add the details to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

<span data-ttu-id="2109d-p102">Os domínios raiz exigem verificação. Por exemplo, contoso.com exige verificação. Se um domínio raiz for verificado, os subdomínios do domínio raiz serão verificados automaticamente. Por exemplo, o subdominio.contoso.com é automaticamente verificado se contoso.com for verificado.</span><span class="sxs-lookup"><span data-stu-id="2109d-p102">Root domains require verification. For example, contoso.com requires verification. If a root domain is verified, subdomains of the root domain are automatically verified. For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="2109d-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="2109d-112">Permissions</span></span>

<span data-ttu-id="2109d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2109d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2109d-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2109d-115">Permission type</span></span>      | <span data-ttu-id="2109d-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2109d-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2109d-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2109d-117">Delegated (work or school account)</span></span> | <span data-ttu-id="2109d-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2109d-118">Directory.Read.All</span></span>    |
|<span data-ttu-id="2109d-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2109d-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2109d-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2109d-120">Not supported.</span></span>    |
|<span data-ttu-id="2109d-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2109d-121">Application</span></span> | <span data-ttu-id="2109d-122">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2109d-122">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2109d-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2109d-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/verificationDnsRecords
```

> <span data-ttu-id="2109d-124">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="2109d-124">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="2109d-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2109d-125">Optional query parameters</span></span>

<span data-ttu-id="2109d-126">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2109d-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2109d-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2109d-127">Request headers</span></span>

| <span data-ttu-id="2109d-128">Nome</span><span class="sxs-lookup"><span data-stu-id="2109d-128">Name</span></span>      |<span data-ttu-id="2109d-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="2109d-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2109d-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="2109d-130">Authorization</span></span>  | <span data-ttu-id="2109d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2109d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2109d-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2109d-133">Content-Type</span></span>  | <span data-ttu-id="2109d-134">application/json</span><span class="sxs-lookup"><span data-stu-id="2109d-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2109d-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2109d-135">Request body</span></span>

<span data-ttu-id="2109d-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2109d-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2109d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="2109d-137">Response</span></span>

<span data-ttu-id="2109d-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [domainDnsRecord](../resources/domaindnsrecord.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2109d-138">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2109d-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2109d-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2109d-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2109d-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_verificationdnsrecords"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com/verificationDnsRecords
```

##### <a name="response"></a><span data-ttu-id="2109d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2109d-141">Response</span></span>

<span data-ttu-id="2109d-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2109d-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List verificationDnsRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-list-verificationdnsrecords.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
