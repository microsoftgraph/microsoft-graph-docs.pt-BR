---
title: 'educationSchool: delta'
description: Get newly created or updated schools without having to perform a full read of the entire school collection.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3604a9296d7419d20e1b2b9016a2dc724b65c222
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232140"
---
# <a name="educationschool-delta"></a><span data-ttu-id="5870a-103">educationSchool: delta</span><span class="sxs-lookup"><span data-stu-id="5870a-103">educationSchool: delta</span></span>

<span data-ttu-id="5870a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5870a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5870a-105">Get newly created or updated schools without having to perform a full read of the entire school collection.</span><span class="sxs-lookup"><span data-stu-id="5870a-105">Get newly created or updated schools without having to perform a full read of the entire school collection.</span></span> <span data-ttu-id="5870a-106">Consulte [Usar consulta delta para](/graph/delta-query-overview) obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="5870a-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="5870a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5870a-107">Permissions</span></span>

<span data-ttu-id="5870a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5870a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5870a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5870a-110">Permission type</span></span>                        | <span data-ttu-id="5870a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5870a-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="5870a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5870a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5870a-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="5870a-113">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="5870a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5870a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5870a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5870a-115">Not supported.</span></span>                              |
| <span data-ttu-id="5870a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5870a-116">Application</span></span>                            | <span data-ttu-id="5870a-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5870a-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5870a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5870a-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/schools/delta
```

## <a name="request-headers"></a><span data-ttu-id="5870a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5870a-119">Request headers</span></span>

| <span data-ttu-id="5870a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5870a-120">Name</span></span>          | <span data-ttu-id="5870a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5870a-121">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5870a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5870a-122">Authorization</span></span> | <span data-ttu-id="5870a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5870a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5870a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5870a-125">Request body</span></span>

<span data-ttu-id="5870a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5870a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5870a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5870a-127">Response</span></span>

<span data-ttu-id="5870a-128">Se tiver êxito, essa função retornará um código `200 OK` de resposta e uma coleção [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5870a-128">If successful, this function returns a `200 OK` response code and a [educationSchool](../resources/educationschool.md) collection in the response body.</span></span> <span data-ttu-id="5870a-129">A resposta também inclui uma URL `nextLink` ou `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="5870a-129">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="5870a-130">Se uma URL `nextLink` é retornada, existem páginas de dado adicionais a serem recuperadas na sessão.</span><span class="sxs-lookup"><span data-stu-id="5870a-130">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="5870a-131">O aplicativo continua fazendo solicitações usando a URL `nextLink` até uma URL `deltaLink` ser incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="5870a-131">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
- <span data-ttu-id="5870a-132">Se uma URL `deltaLink` é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="5870a-132">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="5870a-133">Persista e use `deltaLink` a URL para saber mais sobre as alterações no recurso no futuro.</span><span class="sxs-lookup"><span data-stu-id="5870a-133">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="5870a-134">Para obter detalhes, consulte [Using delta query](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="5870a-134">For details, see [Using delta query](/graph/delta-query-overview).</span></span> <span data-ttu-id="5870a-135">Por exemplo, solicitações, [consulte Obter alterações incrementais para usuários](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="5870a-135">For example requests, see [Get incremental changes for users](/graph/delta-query-users).</span></span>

## <a name="examples"></a><span data-ttu-id="5870a-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5870a-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5870a-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5870a-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "educationschool_delta"
}
-->

```http
GET https://graph.microsoft.com/v1.0/education/schools/delta
```

### <a name="response"></a><span data-ttu-id="5870a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5870a-138">Response</span></span>

> <span data-ttu-id="5870a-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5870a-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.educationSchool)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(educationSchool)",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/education/schools/delta?$skiptoken=VwhMSQw1l1O5v2F1ZPm...",
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationSchool",
      "id": "String (identifier)",
      "displayName": "String",
      "description": "String",
      "externalSource": "String",
      "externalSourceDetail": "String",
      "principalEmail": "String",
      "principalName": "String",
      "externalPrincipalId": "String",
      "lowestGrade": "String",
      "highestGrade": "String",
      "schoolNumber": "String",
      "externalId": "String",
      "phone": "String",
      "fax": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "address": {
        "@odata.type": "microsoft.graph.physicalAddress"
      }
    }
  ]
}
```
