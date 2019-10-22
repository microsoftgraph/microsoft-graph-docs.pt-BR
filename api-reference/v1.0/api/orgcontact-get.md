---
title: Obter orgContact
description: Recupere as propriedades de um objeto orgContact.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9699006f2ec9c88af4c12f41e6e5d14486a004ee
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37622569"
---
# <a name="get-orgcontact"></a><span data-ttu-id="0ea76-103">Obter orgContact</span><span class="sxs-lookup"><span data-stu-id="0ea76-103">Get orgContact</span></span>

<span data-ttu-id="0ea76-104">Obtenha as propriedades e os relacionamentos de um [contato organizacional](../resources/orgcontact.md).</span><span class="sxs-lookup"><span data-stu-id="0ea76-104">Get the properties and relationships of an [organizational contact](../resources/orgcontact.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0ea76-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0ea76-105">Permissions</span></span>
<span data-ttu-id="0ea76-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ea76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ea76-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ea76-108">Permission type</span></span>      | <span data-ttu-id="0ea76-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0ea76-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ea76-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ea76-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0ea76-111">OrgContact. Read. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="0ea76-111">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0ea76-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ea76-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ea76-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ea76-113">Not supported.</span></span>    |
|<span data-ttu-id="0ea76-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ea76-114">Application</span></span> | <span data-ttu-id="0ea76-115">OrgContact. Read. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0ea76-115">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ea76-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ea76-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0ea76-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0ea76-117">Optional query parameters</span></span>
<span data-ttu-id="0ea76-118">Este método oferece suporte `$select` aos `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0ea76-118">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ea76-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ea76-119">Request headers</span></span>
| <span data-ttu-id="0ea76-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0ea76-120">Header</span></span>       | <span data-ttu-id="0ea76-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0ea76-121">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="0ea76-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ea76-122">Authorization</span></span>  | <span data-ttu-id="0ea76-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ea76-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ea76-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ea76-125">Request body</span></span>
<span data-ttu-id="0ea76-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0ea76-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ea76-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ea76-127">Response</span></span>

<span data-ttu-id="0ea76-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [orgContact](../resources/orgcontact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ea76-128">If successful, this method returns a `200 OK` response code and an [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0ea76-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ea76-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ea76-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ea76-130">Request</span></span>
<span data-ttu-id="0ea76-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ea76-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_orgcontact"
}-->
```http
GET https://graph.microsoft.com/v1.0/contacts/{id}
```

##### <a name="response"></a><span data-ttu-id="0ea76-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ea76-132">Response</span></span>
<span data-ttu-id="0ea76-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0ea76-133">The following is an example of the response.</span></span>
><span data-ttu-id="0ea76-134">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0ea76-134">**Note**: The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "addresses":[
      {
        "city": "string",
        "countryOrRegion": "string",
        "officeLocation": "string",
        "postalCode": "string",
        "state": "string",
        "street": "string"
      }
  ],
  "companyName": "companyName-value",
  "department": "department-value",
  "displayName": "displayName-value",
  "phones":[
      {
        "type": "string",
        "number": "string"
      }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
