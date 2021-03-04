---
title: Listar serviceConfigurationRecords
description: Recupera uma lista de objetos domainDnsRecord necessários para habilitar serviços para o domínio.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: eb0afcfc5882be85ed69174527b0a233f679b9e0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436502"
---
# <a name="list-serviceconfigurationrecords"></a><span data-ttu-id="1fa6b-103">Listar serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="1fa6b-103">List serviceConfigurationRecords</span></span>

<span data-ttu-id="1fa6b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fa6b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fa6b-105">Recupera uma lista de [objetos domainDnsRecord](../resources/domaindnsrecord.md) necessários para habilitar serviços para o domínio.</span><span class="sxs-lookup"><span data-stu-id="1fa6b-105">Retrieves a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects needed to enable services for the domain.</span></span>

<span data-ttu-id="1fa6b-106">Use a lista retornada para adicionar registros ao arquivo de zona do domínio.</span><span class="sxs-lookup"><span data-stu-id="1fa6b-106">Use the returned list to add records to the zone file of the domain.</span></span> <span data-ttu-id="1fa6b-107">Isso pode ser feito por meio do registrador de domínio ou da configuração do servidor DNS.</span><span class="sxs-lookup"><span data-stu-id="1fa6b-107">This can be done through the domain registrar or DNS server configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="1fa6b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1fa6b-108">Permissions</span></span>

<span data-ttu-id="1fa6b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fa6b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1fa6b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1fa6b-111">Permission type</span></span>      | <span data-ttu-id="1fa6b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1fa6b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1fa6b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1fa6b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1fa6b-114">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1fa6b-114">Directory.Read.All</span></span>    |
|<span data-ttu-id="1fa6b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1fa6b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fa6b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fa6b-116">Not supported.</span></span>    |
|<span data-ttu-id="1fa6b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1fa6b-117">Application</span></span> | <span data-ttu-id="1fa6b-118">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fa6b-118">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1fa6b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1fa6b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1fa6b-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1fa6b-120">Optional query parameters</span></span>

<span data-ttu-id="1fa6b-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1fa6b-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1fa6b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1fa6b-122">Request headers</span></span>

| <span data-ttu-id="1fa6b-123">Nome</span><span class="sxs-lookup"><span data-stu-id="1fa6b-123">Name</span></span>      |<span data-ttu-id="1fa6b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fa6b-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1fa6b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1fa6b-125">Authorization</span></span>  | <span data-ttu-id="1fa6b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fa6b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1fa6b-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1fa6b-128">Content-Type</span></span>  | <span data-ttu-id="1fa6b-129">application/json</span><span class="sxs-lookup"><span data-stu-id="1fa6b-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1fa6b-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1fa6b-130">Request body</span></span>

<span data-ttu-id="1fa6b-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1fa6b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1fa6b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fa6b-132">Response</span></span>

<span data-ttu-id="1fa6b-133">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [domainDnsRecord](../resources/domaindnsrecord.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1fa6b-133">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fa6b-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1fa6b-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1fa6b-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1fa6b-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1fa6b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="1fa6b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/domains/contoso.com/serviceConfigurationRecords
```
# <a name="c"></a>[<span data-ttu-id="1fa6b-137">C#</span><span class="sxs-lookup"><span data-stu-id="1fa6b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceconfigurationrecords-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1fa6b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1fa6b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceconfigurationrecords-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1fa6b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1fa6b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceconfigurationrecords-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1fa6b-140">Java</span><span class="sxs-lookup"><span data-stu-id="1fa6b-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceconfigurationrecords-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1fa6b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fa6b-141">Response</span></span>
<span data-ttu-id="1fa6b-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1fa6b-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "mailExchange": "contoso-com.mail.protection.outlook.com",
      "preference": 0
    },
    {
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Txt",
      "supportedServices": "Email",
      "ttl": 3600,
      "text": "v=spf1 include: spf.protection.outlook.com ~all"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List serviceConfigurationRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
