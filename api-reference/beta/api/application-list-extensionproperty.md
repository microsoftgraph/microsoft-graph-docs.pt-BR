---
title: List extensionproperties
description: Recupere uma lista de objetos extensionproperty.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8d7693768a57f4aae4043c79f60c88627e6e9684
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936556"
---
# <a name="list-extensionproperties"></a><span data-ttu-id="43071-103">List extensionproperties</span><span class="sxs-lookup"><span data-stu-id="43071-103">List extensionProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43071-104">Recupere a lista de objetos [extensionproperty](../resources/extensionproperty.md) em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="43071-104">Retrieve the list of [extensionProperty](../resources/extensionproperty.md) objects on an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="43071-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="43071-105">Permissions</span></span>

<span data-ttu-id="43071-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43071-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43071-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43071-108">Permission type</span></span>      | <span data-ttu-id="43071-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="43071-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43071-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43071-110">Delegated (work or school account)</span></span> | <span data-ttu-id="43071-111">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="43071-111">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="43071-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43071-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43071-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43071-113">Not supported.</span></span>    |
|<span data-ttu-id="43071-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43071-114">Application</span></span> | <span data-ttu-id="43071-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="43071-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="43071-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43071-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/extensionProperties
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43071-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="43071-117">Optional query parameters</span></span>

<span data-ttu-id="43071-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="43071-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="43071-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="43071-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="43071-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43071-120">Request headers</span></span>

| <span data-ttu-id="43071-121">Nome</span><span class="sxs-lookup"><span data-stu-id="43071-121">Name</span></span>       | <span data-ttu-id="43071-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="43071-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="43071-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="43071-123">Authorization</span></span>  | <span data-ttu-id="43071-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43071-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="43071-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43071-126">Request body</span></span>

<span data-ttu-id="43071-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="43071-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43071-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="43071-128">Response</span></span>

<span data-ttu-id="43071-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [extensionproperty](../resources/extensionproperty.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43071-129">If successful, this method returns a `200 OK` response code and a collection of [extensionProperty](../resources/extensionproperty.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="43071-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="43071-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="43071-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43071-131">Request</span></span>

<span data-ttu-id="43071-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="43071-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_extensionproperties"
}-->

```http
GET https://graph.microsoft.com/beta/applications/{id}/extensionProperties
```

### <a name="response"></a><span data-ttu-id="43071-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="43071-133">Response</span></span>

<span data-ttu-id="43071-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="43071-134">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.extensionProperty",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "a2c459db-f5dc-4328-ae9b-118e88d04d19",
            "deletedDateTime": null,
            "appDisplayName": "Display name",
            "name": "extension_b3efaf8f68a44275abcff28ef86b2ee3_extensionName",
            "dataType": "String",
            "isSyncedFromOnPremises": false,
            "targetObjects": [
                "Application"
            ]
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List extensionProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
