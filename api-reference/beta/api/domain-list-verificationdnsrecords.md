---
title: Listar verificationDnsRecords
description: Recupere uma lista de objetos domainDnsRecord.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6338f9c6f61594d9485a2241da85e9add7e6efb0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436495"
---
# <a name="list-verificationdnsrecords"></a><span data-ttu-id="88a12-103">Listar verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="88a12-103">List verificationDnsRecords</span></span>

<span data-ttu-id="88a12-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88a12-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88a12-105">Recupere uma lista de [objetos domainDnsRecord.](../resources/domaindnsrecord.md)</span><span class="sxs-lookup"><span data-stu-id="88a12-105">Retrieve a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects.</span></span>

<span data-ttu-id="88a12-106">Não é possível usar um domínio associado ao locatário do Azure AD até que a propriedade seja verificada.</span><span class="sxs-lookup"><span data-stu-id="88a12-106">You cannot use an associated domain with your Azure AD tenant until ownership is verified.</span></span> <span data-ttu-id="88a12-107">Para verificar a propriedade do domínio, recupere os registros de verificação de domínio e adicione os detalhes ao arquivo de zona do domínio.</span><span class="sxs-lookup"><span data-stu-id="88a12-107">To verify the ownership of the domain, retrieve the domain verification records and add the details to the zone file of the domain.</span></span> <span data-ttu-id="88a12-108">Isso pode ser feito por meio do registrador de domínio ou da configuração do servidor DNS.</span><span class="sxs-lookup"><span data-stu-id="88a12-108">This can be done through the domain registrar or DNS server configuration.</span></span>

<span data-ttu-id="88a12-109">Domínios raiz exigem verificação.</span><span class="sxs-lookup"><span data-stu-id="88a12-109">Root domains require verification.</span></span> <span data-ttu-id="88a12-110">Por exemplo, contoso.com requer verificação.</span><span class="sxs-lookup"><span data-stu-id="88a12-110">For example, contoso.com requires verification.</span></span> <span data-ttu-id="88a12-111">Se um domínio raiz for verificado, subdomas do domínio raiz serão verificados automaticamente.</span><span class="sxs-lookup"><span data-stu-id="88a12-111">If a root domain is verified, subdomains of the root domain are automatically verified.</span></span> <span data-ttu-id="88a12-112">Por exemplo, subdomain.contoso.com será verificado automaticamente se contoso.com tiver sido verificado.</span><span class="sxs-lookup"><span data-stu-id="88a12-112">For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="88a12-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="88a12-113">Permissions</span></span>

<span data-ttu-id="88a12-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88a12-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="88a12-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88a12-116">Permission type</span></span>      | <span data-ttu-id="88a12-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="88a12-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88a12-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88a12-118">Delegated (work or school account)</span></span> | <span data-ttu-id="88a12-119">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="88a12-119">Directory.Read.All</span></span>    |
|<span data-ttu-id="88a12-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88a12-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88a12-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88a12-121">Not supported.</span></span>    |
|<span data-ttu-id="88a12-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88a12-122">Application</span></span> | <span data-ttu-id="88a12-123">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a12-123">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="88a12-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88a12-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/verificationDnsRecords
```

> <span data-ttu-id="88a12-125">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="88a12-125">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="88a12-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="88a12-126">Optional query parameters</span></span>

<span data-ttu-id="88a12-127">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="88a12-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88a12-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88a12-128">Request headers</span></span>

| <span data-ttu-id="88a12-129">Nome</span><span class="sxs-lookup"><span data-stu-id="88a12-129">Name</span></span>      |<span data-ttu-id="88a12-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="88a12-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="88a12-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="88a12-131">Authorization</span></span>  | <span data-ttu-id="88a12-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88a12-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="88a12-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="88a12-134">Content-Type</span></span>  | <span data-ttu-id="88a12-135">application/json</span><span class="sxs-lookup"><span data-stu-id="88a12-135">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="88a12-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88a12-136">Request body</span></span>

<span data-ttu-id="88a12-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="88a12-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88a12-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="88a12-138">Response</span></span>

<span data-ttu-id="88a12-139">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [domainDnsRecord](../resources/domaindnsrecord.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88a12-139">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88a12-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88a12-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88a12-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88a12-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="88a12-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="88a12-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_verificationdnsrecords"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/domains/contoso.com/verificationDnsRecords
```
# <a name="c"></a>[<span data-ttu-id="88a12-143">C#</span><span class="sxs-lookup"><span data-stu-id="88a12-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-verificationdnsrecords-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88a12-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88a12-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-verificationdnsrecords-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88a12-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88a12-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-verificationdnsrecords-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="88a12-146">Java</span><span class="sxs-lookup"><span data-stu-id="88a12-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-verificationdnsrecords-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="88a12-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="88a12-147">Response</span></span>

<span data-ttu-id="88a12-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88a12-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
