---
title: Listar orgContacts
description: Recupere a lista de contatos organizacionais desta organização.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2ced1cd140f322617d1b7a75d1af83fd938360fc
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37622571"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="6f793-103">Listar orgContacts</span><span class="sxs-lookup"><span data-stu-id="6f793-103">List orgContacts</span></span>

<span data-ttu-id="6f793-104">Obtenha a lista de [contatos organizacionais](../resources/orgcontact.md) para esta organização.</span><span class="sxs-lookup"><span data-stu-id="6f793-104">Get the list of [organizational contacts](../resources/orgcontact.md) for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f793-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6f793-105">Permissions</span></span>
<span data-ttu-id="6f793-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f793-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f793-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f793-108">Permission type</span></span>      | <span data-ttu-id="6f793-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6f793-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f793-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f793-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6f793-111">OrgContact. Read. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="6f793-111">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6f793-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f793-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f793-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f793-113">Not supported.</span></span>    |
|<span data-ttu-id="6f793-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f793-114">Application</span></span> | <span data-ttu-id="6f793-115">OrgContact. Read. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6f793-115">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f793-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f793-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6f793-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6f793-117">Optional query parameters</span></span>
<span data-ttu-id="6f793-118">Este método oferece suporte `$expand`aos `$filter`parâmetros `$select`de `$top` [consulta OData](/graph/query-parameters) ,, e OData, para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6f793-118">This method supports the `$expand`, `$filter`, `$select`, and `$top` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6f793-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f793-119">Request headers</span></span>
| <span data-ttu-id="6f793-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6f793-120">Header</span></span>       | <span data-ttu-id="6f793-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6f793-121">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="6f793-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f793-122">Authorization</span></span>  |<span data-ttu-id="6f793-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f793-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f793-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f793-125">Request body</span></span>
<span data-ttu-id="6f793-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6f793-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f793-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f793-127">Response</span></span>

<span data-ttu-id="6f793-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [orgContact](../resources/orgcontact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f793-128">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6f793-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f793-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6f793-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f793-130">Request</span></span>
<span data-ttu-id="6f793-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f793-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```http
GET https://graph.microsoft.com/v1.0/contacts
```

##### <a name="response"></a><span data-ttu-id="6f793-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f793-132">Response</span></span>
<span data-ttu-id="6f793-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6f793-133">The following is an example of the response.</span></span>
><span data-ttu-id="6f793-134">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6f793-134">**Note**: The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
