---
title: 'educationSchool: Delta'
description: Obter escolas recém-criadas ou atualizadas sem ter que realizar uma leitura completa de toda a coleção de escola.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b34ff6bad00194ce6d1967e503e280d0e0af2478
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42425545"
---
# <a name="educationschool-delta"></a><span data-ttu-id="15735-103">educationSchool: Delta</span><span class="sxs-lookup"><span data-stu-id="15735-103">educationSchool: delta</span></span>

<span data-ttu-id="15735-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="15735-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15735-105">Obter escolas recém-criadas ou atualizadas sem ter que realizar uma leitura completa de toda a coleção de escola.</span><span class="sxs-lookup"><span data-stu-id="15735-105">Get newly created or updated schools without having to perform a full read of the entire school collection.</span></span> <span data-ttu-id="15735-106">Consulte [usar a consulta Delta](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="15735-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="15735-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="15735-107">Permissions</span></span>

<span data-ttu-id="15735-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15735-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="15735-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15735-110">Permission type</span></span>                        | <span data-ttu-id="15735-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="15735-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="15735-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15735-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="15735-113">EduRoster. ReadBasic, EduRoster. Read ou EduRoster. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15735-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="15735-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15735-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15735-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15735-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="15735-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15735-116">Application</span></span>                            | <span data-ttu-id="15735-117">EduRoster. ReadBasic. All, EduRoster. Read. All ou EduRoster. WriteWrite. All</span><span class="sxs-lookup"><span data-stu-id="15735-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="15735-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15735-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/schools/{id}/delta
POST /education/me/schools/{id}/delta
POST /education/users/{id}/schools/{id}/delta

```

## <a name="request-headers"></a><span data-ttu-id="15735-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15735-119">Request headers</span></span>

| <span data-ttu-id="15735-120">Nome</span><span class="sxs-lookup"><span data-stu-id="15735-120">Name</span></span>          | <span data-ttu-id="15735-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="15735-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="15735-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="15735-122">Authorization</span></span> | <span data-ttu-id="15735-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="15735-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="15735-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15735-124">Request body</span></span>

<span data-ttu-id="15735-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="15735-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15735-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="15735-126">Response</span></span>

<span data-ttu-id="15735-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto da coleção [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15735-127">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15735-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15735-128">Example</span></span>

<span data-ttu-id="15735-129">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="15735-129">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="15735-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15735-130">Request</span></span>

<span data-ttu-id="15735-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="15735-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationschool_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/schools/{id}/delta
```

##### <a name="response"></a><span data-ttu-id="15735-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="15735-132">Response</span></span>

<span data-ttu-id="15735-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="15735-133">The following is an example of the response.</span></span> 

><span data-ttu-id="15735-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15735-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 313

{
  "value": [
    {
      "principalEmail": "principalEmail-value",
      "principalName": "principalName-value",
      "externalPrincipalId": "externalPrincipalId-value",
      "lowestGrade": "lowestGrade-value",
      "highestGrade": "highestGrade-value",
      "schoolNumber": "schoolNumber-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
