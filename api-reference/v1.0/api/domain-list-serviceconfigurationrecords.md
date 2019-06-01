---
title: Listar serviceConfigurationRecords
description: Recupera uma lista de objetos domainDnsRecord necessários para habilitar serviços para o domínio.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 93dee921ec6eea70a1d94d887ce2e5501ee5efc6
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656640"
---
# <a name="list-serviceconfigurationrecords"></a><span data-ttu-id="885a0-103">Listar serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="885a0-103">List serviceConfigurationRecords</span></span>

<span data-ttu-id="885a0-104">Recupera uma lista de objetos [domainDnsRecord](../resources/domaindnsrecord.md) necessários para habilitar serviços para o domínio.</span><span class="sxs-lookup"><span data-stu-id="885a0-104">Retrieves a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects needed to enable services for the domain.</span></span>

<span data-ttu-id="885a0-105">Use a lista retornada para adicionar registros ao arquivo de zona do domínio.</span><span class="sxs-lookup"><span data-stu-id="885a0-105">Use the returned list to add records to the zone file of the domain.</span></span> <span data-ttu-id="885a0-106">Isso pode ser feito por meio do registrador de domínio ou configuração do servidor DNS.</span><span class="sxs-lookup"><span data-stu-id="885a0-106">This can be done through the domain registrar or DNS server configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="885a0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="885a0-107">Permissions</span></span>

<span data-ttu-id="885a0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="885a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="885a0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="885a0-110">Permission type</span></span>      | <span data-ttu-id="885a0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="885a0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="885a0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="885a0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="885a0-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="885a0-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="885a0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="885a0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="885a0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="885a0-115">Not supported.</span></span>    |
|<span data-ttu-id="885a0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="885a0-116">Application</span></span> | <span data-ttu-id="885a0-117">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="885a0-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="885a0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="885a0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/contoso.com/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a><span data-ttu-id="885a0-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="885a0-119">Optional query parameters</span></span>

<span data-ttu-id="885a0-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="885a0-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="885a0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="885a0-121">Request headers</span></span>

| <span data-ttu-id="885a0-122">Nome</span><span class="sxs-lookup"><span data-stu-id="885a0-122">Name</span></span>      |<span data-ttu-id="885a0-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="885a0-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="885a0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="885a0-124">Authorization</span></span>  | <span data-ttu-id="885a0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="885a0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="885a0-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="885a0-127">Content-Type</span></span>  | <span data-ttu-id="885a0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="885a0-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="885a0-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="885a0-129">Request body</span></span>

<span data-ttu-id="885a0-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="885a0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="885a0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="885a0-131">Response</span></span>

<span data-ttu-id="885a0-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [domainDnsRecord](../resources/domaindnsrecord.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="885a0-132">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="885a0-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="885a0-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="885a0-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="885a0-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/serviceConfigurationRecords
```
##### <a name="response"></a><span data-ttu-id="885a0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="885a0-135">Response</span></span>
<span data-ttu-id="885a0-p104">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="885a0-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "@odata.type":"microsoft.graph.domainDnsMxRecord",
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Mx",
      "supportedService": "Email",
      "ttl": 3600,
      "mailExchange": "contoso-com.mail.protection.outlook.com",
      "preference": 0
    },
    {
      "@odata.type":"microsoft.graph.domainDnsTxtRecord",
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Txt",
      "supportedService": "Email",
      "ttl": 3600,
      "text": "v=spf1 include: spf.protection.outlook.com ~all"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="885a0-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="885a0-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="885a0-139">C#</span><span class="sxs-lookup"><span data-stu-id="885a0-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_serviceconfigurationrecords-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="885a0-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="885a0-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_serviceconfigurationrecords-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List serviceConfigurationRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/domain-list-serviceconfigurationrecords.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/domain-list-serviceconfigurationrecords.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
