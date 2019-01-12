---
title: Listar serviceConfigurationRecords
description: Recupera uma lista de objetos domainDnsRecord necessários para ativar os serviços do domínio.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2880a8336d15b675cd5debc6008d8de8f4d191f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965534"
---
# <a name="list-serviceconfigurationrecords"></a><span data-ttu-id="a358a-103">Listar serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="a358a-103">List serviceConfigurationRecords</span></span>

> <span data-ttu-id="a358a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a358a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a358a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a358a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a358a-106">Recupera uma lista de objetos [domainDnsRecord](../resources/domaindnsrecord.md) necessários para ativar os serviços do domínio.</span><span class="sxs-lookup"><span data-stu-id="a358a-106">Retrieves a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects needed to enable services for the domain.</span></span>

<span data-ttu-id="a358a-p102">Use a lista retornada para adicionar registros para ao arquivo de zona do domínio. Isso pode ser feito por meio da configuração do servidor DNS ou do registrador de domínios.</span><span class="sxs-lookup"><span data-stu-id="a358a-p102">Use the returned list to add records to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="a358a-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="a358a-109">Permissions</span></span>

<span data-ttu-id="a358a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a358a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a358a-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a358a-112">Permission type</span></span>      | <span data-ttu-id="a358a-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a358a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a358a-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a358a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a358a-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a358a-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="a358a-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a358a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a358a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a358a-117">Not supported.</span></span>    |
|<span data-ttu-id="a358a-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a358a-118">Application</span></span> | <span data-ttu-id="a358a-119">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a358a-119">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a358a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a358a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/contoso.com/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a358a-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a358a-121">Optional query parameters</span></span>

<span data-ttu-id="a358a-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a358a-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a358a-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a358a-123">Request headers</span></span>

| <span data-ttu-id="a358a-124">Nome</span><span class="sxs-lookup"><span data-stu-id="a358a-124">Name</span></span>      |<span data-ttu-id="a358a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="a358a-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a358a-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="a358a-126">Authorization</span></span>  | <span data-ttu-id="a358a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a358a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a358a-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a358a-129">Content-Type</span></span>  | <span data-ttu-id="a358a-130">application/json</span><span class="sxs-lookup"><span data-stu-id="a358a-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a358a-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a358a-131">Request body</span></span>

<span data-ttu-id="a358a-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a358a-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a358a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a358a-133">Response</span></span>

<span data-ttu-id="a358a-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [domainDnsRecord](../resources/domaindnsrecord.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a358a-134">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a358a-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a358a-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a358a-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a358a-136">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com/serviceConfigurationRecords
```
##### <a name="response"></a><span data-ttu-id="a358a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a358a-137">Response</span></span>
<span data-ttu-id="a358a-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a358a-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List serviceConfigurationRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
