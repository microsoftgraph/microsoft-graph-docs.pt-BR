---
title: Listar serviceConfigurationRecords
description: Recupera uma lista de objetos domainDnsRecord necessários para habilitar serviços para o domínio.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1aead8505135347826c4cbca9c758de689549ff1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454880"
---
# <a name="list-serviceconfigurationrecords"></a><span data-ttu-id="7d387-103">Listar serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="7d387-103">List serviceConfigurationRecords</span></span>

<span data-ttu-id="7d387-104">Recupera uma lista de objetos [domainDnsRecord](../resources/domaindnsrecord.md) necessários para habilitar serviços para o domínio.</span><span class="sxs-lookup"><span data-stu-id="7d387-104">Retrieves a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects needed to enable services for the domain.</span></span>

<span data-ttu-id="7d387-105">Use a lista retornada para adicionar registros ao arquivo de zona do domínio.</span><span class="sxs-lookup"><span data-stu-id="7d387-105">Use the returned list to add records to the zone file of the domain.</span></span> <span data-ttu-id="7d387-106">Isso pode ser feito por meio do registrador de domínio ou configuração do servidor DNS.</span><span class="sxs-lookup"><span data-stu-id="7d387-106">This can be done through the domain registrar or DNS server configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d387-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7d387-107">Permissions</span></span>

<span data-ttu-id="7d387-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d387-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7d387-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d387-110">Permission type</span></span>      | <span data-ttu-id="7d387-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7d387-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d387-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d387-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7d387-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7d387-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="7d387-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d387-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d387-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d387-115">Not supported.</span></span>    |
|<span data-ttu-id="7d387-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d387-116">Application</span></span> | <span data-ttu-id="7d387-117">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d387-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d387-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d387-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/contoso.com/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7d387-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7d387-119">Optional query parameters</span></span>

<span data-ttu-id="7d387-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7d387-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d387-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d387-121">Request headers</span></span>

| <span data-ttu-id="7d387-122">Nome</span><span class="sxs-lookup"><span data-stu-id="7d387-122">Name</span></span>      |<span data-ttu-id="7d387-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d387-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7d387-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d387-124">Authorization</span></span>  | <span data-ttu-id="7d387-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d387-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7d387-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7d387-127">Content-Type</span></span>  | <span data-ttu-id="7d387-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7d387-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d387-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d387-129">Request body</span></span>

<span data-ttu-id="7d387-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7d387-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d387-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d387-131">Response</span></span>

<span data-ttu-id="7d387-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [domainDnsRecord](../resources/domaindnsrecord.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d387-132">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d387-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d387-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7d387-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d387-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/serviceConfigurationRecords
```
##### <a name="response"></a><span data-ttu-id="7d387-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d387-135">Response</span></span>
<span data-ttu-id="7d387-p104">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d387-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List serviceConfigurationRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
