---
title: Listar educationSchools
description: Obter uma lista dos objetos educationSchool e suas propriedades.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 98602e535864f7c62c673af66b717758bebb2c97
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232130"
---
# <a name="list-educationschools"></a><span data-ttu-id="9f32c-103">Listar educationSchools</span><span class="sxs-lookup"><span data-stu-id="9f32c-103">List educationSchools</span></span>

<span data-ttu-id="9f32c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f32c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9f32c-105">Obter uma lista dos [objetos educationSchool](../resources/educationschool.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="9f32c-105">Get a list of the [educationSchool](../resources/educationschool.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f32c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9f32c-106">Permissions</span></span>

<span data-ttu-id="9f32c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f32c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9f32c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f32c-109">Permission type</span></span>                        | <span data-ttu-id="9f32c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9f32c-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="9f32c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f32c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f32c-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="9f32c-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="9f32c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f32c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f32c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f32c-114">Not supported.</span></span>                              |
| <span data-ttu-id="9f32c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f32c-115">Application</span></span>                            | <span data-ttu-id="9f32c-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f32c-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f32c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f32c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/schools
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f32c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9f32c-118">Optional query parameters</span></span>

<span data-ttu-id="9f32c-119">Este método dá suporte aos mesmos parâmetros de consulta OData que [Usuários de Lista.](../api/user-list.md#optional-query-parameters)</span><span class="sxs-lookup"><span data-stu-id="9f32c-119">This method supports the same OData query parameters as [List Users](../api/user-list.md#optional-query-parameters).</span></span> <span data-ttu-id="9f32c-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9f32c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f32c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f32c-121">Request headers</span></span>

| <span data-ttu-id="9f32c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="9f32c-122">Name</span></span>          | <span data-ttu-id="9f32c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f32c-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9f32c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f32c-124">Authorization</span></span> | <span data-ttu-id="9f32c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f32c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f32c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f32c-127">Request body</span></span>

<span data-ttu-id="9f32c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9f32c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f32c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f32c-129">Response</span></span>

<span data-ttu-id="9f32c-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f32c-130">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9f32c-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9f32c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9f32c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f32c-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_educationschool"
}
-->

```http
GET https://graph.microsoft.com/v1.0/education/schools
```

### <a name="response"></a><span data-ttu-id="9f32c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f32c-133">Response</span></span>

> <span data-ttu-id="9f32c-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9f32c-134">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "value": [
    {
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
  ]
}
```
