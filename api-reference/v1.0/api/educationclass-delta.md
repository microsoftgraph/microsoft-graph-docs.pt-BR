---
title: 'educationClass: delta'
description: Get newly created or updated classes, including membership changes, without having to perform a full read of the entire class collection.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 80ca48a1494281fed4a39dfff342233a268b5122
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232132"
---
# <a name="educationclass-delta"></a><span data-ttu-id="538ee-103">educationClass: delta</span><span class="sxs-lookup"><span data-stu-id="538ee-103">educationClass: delta</span></span>

<span data-ttu-id="538ee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="538ee-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="538ee-105">Get newly created or updated classes, including membership changes, without having to perform a full read of the entire class collection.</span><span class="sxs-lookup"><span data-stu-id="538ee-105">Get newly created or updated classes, including membership changes, without having to perform a full read of the entire class collection.</span></span> <span data-ttu-id="538ee-106">Consulte [Usar consulta delta para](/graph/delta-query-overview) obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="538ee-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="538ee-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="538ee-107">Permissions</span></span>

<span data-ttu-id="538ee-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="538ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="538ee-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="538ee-110">Permission type</span></span>                        | <span data-ttu-id="538ee-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="538ee-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="538ee-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="538ee-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="538ee-113">EduRoster.ReadBasic, EduRoster.Read ou EduRoster.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="538ee-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="538ee-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="538ee-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="538ee-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="538ee-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="538ee-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="538ee-116">Application</span></span>                            | <span data-ttu-id="538ee-117">EduRoster.ReadBasic.All, EduRoster.Read.All ou EduRoster.WriteWrite.All</span><span class="sxs-lookup"><span data-stu-id="538ee-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="538ee-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="538ee-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/classes/delta
```

## <a name="request-headers"></a><span data-ttu-id="538ee-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="538ee-119">Request headers</span></span>

| <span data-ttu-id="538ee-120">Nome</span><span class="sxs-lookup"><span data-stu-id="538ee-120">Name</span></span>          | <span data-ttu-id="538ee-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="538ee-121">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="538ee-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="538ee-122">Authorization</span></span> | <span data-ttu-id="538ee-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="538ee-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="538ee-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="538ee-125">Request body</span></span>

<span data-ttu-id="538ee-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="538ee-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="538ee-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="538ee-127">Response</span></span>

<span data-ttu-id="538ee-128">Se tiver êxito, essa função retornará um código `200 OK` de resposta e uma coleção [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="538ee-128">If successful, this function returns an `200 OK` response code and an [educationClass](../resources/educationclass.md) collection in the response body.</span></span> <span data-ttu-id="538ee-129">A resposta também inclui uma URL `nextLink` ou `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="538ee-129">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="538ee-130">Se uma URL `nextLink` é retornada, existem páginas de dado adicionais a serem recuperadas na sessão.</span><span class="sxs-lookup"><span data-stu-id="538ee-130">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="538ee-131">O aplicativo continua fazendo solicitações usando a URL `nextLink` até uma URL `deltaLink` ser incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="538ee-131">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
- <span data-ttu-id="538ee-132">Se uma URL `deltaLink` é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="538ee-132">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="538ee-133">Persista e use `deltaLink` a URL para saber mais sobre as alterações no recurso no futuro.</span><span class="sxs-lookup"><span data-stu-id="538ee-133">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="538ee-134">Para obter detalhes, consulte [Using delta query](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="538ee-134">For details, see [Using delta query](/graph/delta-query-overview).</span></span> <span data-ttu-id="538ee-135">Por exemplo, solicitações, [consulte Obter alterações incrementais para usuários](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="538ee-135">For example requests, see [Get incremental changes for users](/graph/delta-query-users).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="538ee-136">os deltas educationClass não incluem classes excluídas.</span><span class="sxs-lookup"><span data-stu-id="538ee-136">educationClass deltas do not include deleted classes.</span></span>

## <a name="examples"></a><span data-ttu-id="538ee-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="538ee-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="538ee-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="538ee-138">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "educationclass_delta"
}
-->

```http
GET https://graph.microsoft.com/v1.0/education/classes/delta
```

### <a name="response"></a><span data-ttu-id="538ee-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="538ee-139">Response</span></span>

> <span data-ttu-id="538ee-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="538ee-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.educationClass)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{

  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(educationClass)",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/education/classes/delta?$skiptoken=sU1S4IJGk3hwxbia8...",
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationClass",
      "id": "String (identifier)",
      "displayName": "String",
      "mailNickname": "String",
      "description": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "classCode": "String",
      "externalName": "String",
      "externalId": "String",
      "externalSource": "String",
      "externalSourceDetail": "String",
      "grade": "String",
      "term": {
        "@odata.type": "microsoft.graph.educationTerm"
      }
    }
  ]
}
```
