---
title: Listar directReports
description: Obter os subordinados diretos do contato.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f75c23e3b6b1aa79aeea0a812f7175a1b70f52e0
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37622577"
---
# <a name="list-directreports"></a><span data-ttu-id="c53d0-103">Listar directReports</span><span class="sxs-lookup"><span data-stu-id="c53d0-103">List directReports</span></span>

<span data-ttu-id="c53d0-104">Obtenha os subordinados diretos para este [contato organizacional](../resources/orgcontact.md).</span><span class="sxs-lookup"><span data-stu-id="c53d0-104">Get the direct reports for this [organizational contact](../resources/orgcontact.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c53d0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c53d0-105">Permissions</span></span>
<span data-ttu-id="c53d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c53d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c53d0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c53d0-108">Permission type</span></span>      | <span data-ttu-id="c53d0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c53d0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c53d0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c53d0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c53d0-111">OrgContact. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="c53d0-111">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="c53d0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c53d0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c53d0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c53d0-113">Not supported.</span></span>    |
|<span data-ttu-id="c53d0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c53d0-114">Application</span></span> | <span data-ttu-id="c53d0-115">OrgContact. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="c53d0-115">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c53d0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c53d0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c53d0-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c53d0-117">Optional query parameters</span></span>
<span data-ttu-id="c53d0-118">Este método oferece suporte `$select` aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c53d0-118">This method supports the `$select` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c53d0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c53d0-119">Request headers</span></span>
| <span data-ttu-id="c53d0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c53d0-120">Header</span></span>       | <span data-ttu-id="c53d0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c53d0-121">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="c53d0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c53d0-122">Authorization</span></span>  | <span data-ttu-id="c53d0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c53d0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c53d0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c53d0-125">Request body</span></span>
<span data-ttu-id="c53d0-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c53d0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c53d0-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c53d0-127">Response</span></span>

<span data-ttu-id="c53d0-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c53d0-128">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c53d0-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c53d0-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c53d0-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c53d0-130">Request</span></span>
<span data-ttu-id="c53d0-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c53d0-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "contacts_get_directreports"
}-->
```http
GET https://graph.microsoft.com/v1.0/contacts/{id}/directReports
```

##### <a name="response"></a><span data-ttu-id="c53d0-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c53d0-132">Response</span></span>
<span data-ttu-id="c53d0-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c53d0-133">The following is an example of the response.</span></span>
><span data-ttu-id="c53d0-134">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c53d0-134">**Note**: The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 455

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "24fcbca3-c3e2-48bf-9ffc-c7f81b81483d",
      "businessPhones": [
          "+1 205 555 0108"
      ],
      "displayName": "Diego Siciliani",
      "givenName": "Diego",
      "jobTitle": "CVP Finance",
      "mail": "DiegoS@contoso.com",
      "mobilePhone": null,
      "officeLocation": "14/1108",
      "preferredLanguage": "en-US",
      "surname": "Siciliani",
      "userPrincipalName": "DiegoS@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
