---
title: Obter educationSchool
description: Leia as propriedades e as relações de um objeto educationSchool.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 21732795ec15c16a92563eccebdeb7e8d33d3793
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231260"
---
# <a name="get-educationschool"></a><span data-ttu-id="1546e-103">Obter educationSchool</span><span class="sxs-lookup"><span data-stu-id="1546e-103">Get educationSchool</span></span>

<span data-ttu-id="1546e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1546e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1546e-105">Leia as propriedades e as relações de um [objeto educationSchool.](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="1546e-105">Read the properties and relationships of an [educationSchool](../resources/educationschool.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1546e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1546e-106">Permissions</span></span>

<span data-ttu-id="1546e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1546e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1546e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1546e-109">Permission type</span></span>                        | <span data-ttu-id="1546e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1546e-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="1546e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1546e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1546e-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="1546e-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="1546e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1546e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1546e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1546e-114">Not supported.</span></span>                              |
| <span data-ttu-id="1546e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1546e-115">Application</span></span>                            | <span data-ttu-id="1546e-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1546e-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1546e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1546e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/schools/{educationSchoolId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1546e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1546e-118">Optional query parameters</span></span>

<span data-ttu-id="1546e-119">Este método dá suporte aos mesmos parâmetros de consulta OData que [Get User](../api/user-get.md#optional-query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1546e-119">This method supports the same OData query parameters as [Get User](../api/user-get.md#optional-query-parameters).</span></span> <span data-ttu-id="1546e-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1546e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1546e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1546e-121">Request headers</span></span>

| <span data-ttu-id="1546e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1546e-122">Name</span></span>          | <span data-ttu-id="1546e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1546e-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1546e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1546e-124">Authorization</span></span> | <span data-ttu-id="1546e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1546e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1546e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1546e-127">Request body</span></span>

<span data-ttu-id="1546e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1546e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1546e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1546e-129">Response</span></span>

<span data-ttu-id="1546e-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1546e-130">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1546e-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1546e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1546e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1546e-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}
-->

```http
GET https://graph.microsoft.com/v1.0/education/schools/{educationSchoolId}
```

### <a name="response"></a><span data-ttu-id="1546e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1546e-133">Response</span></span>

><span data-ttu-id="1546e-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1546e-134">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.educationSchool",
    "id": "1c23c12e-c12e-1c23-2ec1-231c2ec1231c",
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
}
```
