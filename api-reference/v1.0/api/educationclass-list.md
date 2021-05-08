---
title: Listar educationClasses
description: Obter uma lista dos objetos educationClass e suas propriedades.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6b599217cfb87a853fdc6630f210bea969cbaa97
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232126"
---
# <a name="list-educationclasses"></a><span data-ttu-id="78186-103">Listar educationClasses</span><span class="sxs-lookup"><span data-stu-id="78186-103">List educationClasses</span></span>

<span data-ttu-id="78186-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78186-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="78186-105">Obter uma lista dos [objetos educationClass](../resources/educationclass.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="78186-105">Get a list of the [educationClass](../resources/educationclass.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="78186-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="78186-106">Permissions</span></span>

<span data-ttu-id="78186-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78186-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="78186-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78186-109">Permission type</span></span>                        | <span data-ttu-id="78186-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="78186-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="78186-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78186-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="78186-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="78186-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="78186-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78186-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78186-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="78186-114">Not supported</span></span>                               |
| <span data-ttu-id="78186-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78186-115">Application</span></span>                            | <span data-ttu-id="78186-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78186-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="78186-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78186-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/classes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="78186-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="78186-118">Optional query parameters</span></span>

<span data-ttu-id="78186-119">Use a opção de consulta OData `$orderby` para classificar grupos em uma organização pelos valores **displayName**, conforme exibido no exemplo a seguir:</span><span class="sxs-lookup"><span data-stu-id="78186-119">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

<span data-ttu-id="78186-120">Você também pode usar os `$filter` parâmetros , `$count` e consulta para limitar a `$search` resposta.</span><span class="sxs-lookup"><span data-stu-id="78186-120">You can also use the `$filter`, `$count` and `$search` query parameters to limit the response.</span></span> 

<span data-ttu-id="78186-121">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="78186-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="78186-122">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="78186-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="78186-123">Para obter mais informações sobre as opções de consulta OData, veja [ Parâmetros de consulta OData ](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="78186-123">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="78186-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78186-124">Request headers</span></span>

| <span data-ttu-id="78186-125">Nome</span><span class="sxs-lookup"><span data-stu-id="78186-125">Name</span></span>          | <span data-ttu-id="78186-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="78186-126">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="78186-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="78186-127">Authorization</span></span> | <span data-ttu-id="78186-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78186-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78186-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78186-130">Request body</span></span>

<span data-ttu-id="78186-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="78186-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78186-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="78186-132">Response</span></span>

<span data-ttu-id="78186-133">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78186-133">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="78186-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="78186-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="78186-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78186-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_educationclass"
}
-->

```http
GET https://graph.microsoft.com/v1.0/education/classes
```

### <a name="response"></a><span data-ttu-id="78186-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="78186-136">Response</span></span>

> <span data-ttu-id="78186-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="78186-137">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationClass",
      "id": "64ef8ce5-8ce5-64ef-e58c-ef64e58cef64",
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
