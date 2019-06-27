---
title: Listar verificationDnsRecords
description: Recupere uma lista de objetos domainDnsRecord.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c709137376d4544b45be9facf1d0d894fc5e120b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272104"
---
# <a name="list-verificationdnsrecords"></a><span data-ttu-id="0ba3b-103">Listar verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="0ba3b-103">List verificationDnsRecords</span></span>

<span data-ttu-id="0ba3b-104">Recupere uma lista de objetos [domainDnsRecord](../resources/domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="0ba3b-104">Retrieve a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects.</span></span>

<span data-ttu-id="0ba3b-105">Você não pode usar um domínio associado com seu locatário do Azure AD até que a propriedade seja verificada.</span><span class="sxs-lookup"><span data-stu-id="0ba3b-105">You cannot use an associated domain with your Azure AD tenant until ownership is verified.</span></span> <span data-ttu-id="0ba3b-106">Para verificar a propriedade do domínio, recupere os registros de verificação de domínio e adicione os detalhes ao arquivo de zona do domínio.</span><span class="sxs-lookup"><span data-stu-id="0ba3b-106">To verify the ownership of the domain, retrieve the domain verification records and add the details to the zone file of the domain.</span></span> <span data-ttu-id="0ba3b-107">Isso pode ser feito por meio do registrador de domínio ou configuração do servidor DNS.</span><span class="sxs-lookup"><span data-stu-id="0ba3b-107">This can be done through the domain registrar or DNS server configuration.</span></span>

<span data-ttu-id="0ba3b-108">Os domínios raiz precisam de verificação.</span><span class="sxs-lookup"><span data-stu-id="0ba3b-108">Root domains require verification.</span></span> <span data-ttu-id="0ba3b-109">Por exemplo, contoso.com requer verificação.</span><span class="sxs-lookup"><span data-stu-id="0ba3b-109">For example, contoso.com requires verification.</span></span> <span data-ttu-id="0ba3b-110">Se um domínio raiz é verificado, os subdomínios do domínio raiz são verificados automaticamente.</span><span class="sxs-lookup"><span data-stu-id="0ba3b-110">If a root domain is verified, subdomains of the root domain are automatically verified.</span></span> <span data-ttu-id="0ba3b-111">Por exemplo, subdomain.contoso.com será verificada automaticamente se contoso.com tiver sido verificada.</span><span class="sxs-lookup"><span data-stu-id="0ba3b-111">For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ba3b-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="0ba3b-112">Permissions</span></span>

<span data-ttu-id="0ba3b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ba3b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0ba3b-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ba3b-115">Permission type</span></span>      | <span data-ttu-id="0ba3b-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0ba3b-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ba3b-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ba3b-117">Delegated (work or school account)</span></span> | <span data-ttu-id="0ba3b-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ba3b-118">Directory.Read.All</span></span>    |
|<span data-ttu-id="0ba3b-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ba3b-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ba3b-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ba3b-120">Not supported.</span></span>    |
|<span data-ttu-id="0ba3b-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ba3b-121">Application</span></span> | <span data-ttu-id="0ba3b-122">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ba3b-122">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ba3b-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ba3b-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/verificationDnsRecords
```

> <span data-ttu-id="0ba3b-124">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="0ba3b-124">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="0ba3b-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0ba3b-125">Optional query parameters</span></span>

<span data-ttu-id="0ba3b-126">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0ba3b-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ba3b-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ba3b-127">Request headers</span></span>

| <span data-ttu-id="0ba3b-128">Nome</span><span class="sxs-lookup"><span data-stu-id="0ba3b-128">Name</span></span>      |<span data-ttu-id="0ba3b-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ba3b-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0ba3b-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ba3b-130">Authorization</span></span>  | <span data-ttu-id="0ba3b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ba3b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0ba3b-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0ba3b-133">Content-Type</span></span>  | <span data-ttu-id="0ba3b-134">application/json</span><span class="sxs-lookup"><span data-stu-id="0ba3b-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ba3b-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ba3b-135">Request body</span></span>

<span data-ttu-id="0ba3b-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0ba3b-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ba3b-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ba3b-137">Response</span></span>

<span data-ttu-id="0ba3b-138">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [domainDnsRecord](../resources/domaindnsrecord.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ba3b-138">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ba3b-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ba3b-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ba3b-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ba3b-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_verificationdnsrecords"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/verificationDnsRecords
```

##### <a name="response"></a><span data-ttu-id="0ba3b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ba3b-141">Response</span></span>

<span data-ttu-id="0ba3b-p105">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ba3b-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0ba3b-144">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="0ba3b-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0ba3b-145">C#</span><span class="sxs-lookup"><span data-stu-id="0ba3b-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_verificationdnsrecords-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0ba3b-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="0ba3b-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_verificationdnsrecords-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0ba3b-147">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0ba3b-147">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_verificationdnsrecords-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List verificationDnsRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/domain-list-verificationdnsrecords.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/domain-list-verificationdnsrecords.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/domain-list-verificationdnsrecords.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
