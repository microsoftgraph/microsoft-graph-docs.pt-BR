---
title: Listar profileCardProperties
description: Recupere uma lista de objetos profilecardproperty.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 732671a5c968b13796113affa403d7c44a9691f9
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080691"
---
# <a name="list-profilecardproperties"></a><span data-ttu-id="288db-103">Listar profileCardProperties</span><span class="sxs-lookup"><span data-stu-id="288db-103">List profileCardProperties</span></span>

<span data-ttu-id="288db-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="288db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="288db-105">Obtenha uma coleção de recursos [profileCardProperty](../resources/profilecardproperty.md) de uma organização.</span><span class="sxs-lookup"><span data-stu-id="288db-105">Get a collection of [profileCardProperty](../resources/profilecardproperty.md) resources of an organization.</span></span> <span data-ttu-id="288db-106">Cada recurso é identificado pela propriedade **directoryPropertyName** .</span><span class="sxs-lookup"><span data-stu-id="288db-106">Each resource is identified by its **directoryPropertyName** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="288db-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="288db-107">Permissions</span></span>

<span data-ttu-id="288db-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="288db-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="288db-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="288db-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="288db-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="288db-110">Permission type</span></span>                        | <span data-ttu-id="288db-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="288db-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="288db-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="288db-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="288db-113">User. Read, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="288db-113">User.Read, User.Read.All</span></span>                    |
| <span data-ttu-id="288db-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="288db-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="288db-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="288db-115">Not supported.</span></span>                              |
| <span data-ttu-id="288db-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="288db-116">Application</span></span>                            | <span data-ttu-id="288db-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="288db-117">Not supported.</span></span>                              |

><span data-ttu-id="288db-118">**Observação:** O uso de permissões delegadas para esta operação exige que o usuário conectado tenha um administrador de locatários ou uma função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="288db-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="288db-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="288db-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/settings/profileCardProperties
```

## <a name="optional-query-parameters"></a><span data-ttu-id="288db-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="288db-120">Optional query parameters</span></span>

<span data-ttu-id="288db-121">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="288db-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="288db-122">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="288db-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="288db-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="288db-123">Request headers</span></span>

| <span data-ttu-id="288db-124">Nome</span><span class="sxs-lookup"><span data-stu-id="288db-124">Name</span></span>          |<span data-ttu-id="288db-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="288db-125">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="288db-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="288db-126">Authorization</span></span> | <span data-ttu-id="288db-127">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="288db-127">Bearer {token}.</span></span> <span data-ttu-id="288db-128">Required.</span><span class="sxs-lookup"><span data-stu-id="288db-128">Required.</span></span>   |
| <span data-ttu-id="288db-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="288db-129">Content-Type</span></span>  | <span data-ttu-id="288db-130">application/json.</span><span class="sxs-lookup"><span data-stu-id="288db-130">application/json.</span></span> <span data-ttu-id="288db-131">Required.</span><span class="sxs-lookup"><span data-stu-id="288db-131">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="288db-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="288db-132">Request body</span></span>

<span data-ttu-id="288db-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="288db-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="288db-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="288db-134">Response</span></span>

<span data-ttu-id="288db-135">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [profileCardProperty](../resources/profilecardproperty.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="288db-135">If successful, this method returns a `200 OK` response code and a collection of [profileCardProperty](../resources/profilecardproperty.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="288db-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="288db-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="288db-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="288db-137">Request</span></span>

<span data-ttu-id="288db-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="288db-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="288db-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="288db-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profilecardproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/settings/profileCardProperties
```
# <a name="c"></a>[<span data-ttu-id="288db-140">C#</span><span class="sxs-lookup"><span data-stu-id="288db-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profilecardproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="288db-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="288db-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profilecardproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="288db-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="288db-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profilecardproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="288db-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="288db-143">Response</span></span>

<span data-ttu-id="288db-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="288db-144">The following is an example of the response.</span></span>

> <span data-ttu-id="288db-145">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="288db-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="288db-146">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="288db-146">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profileCardProperty",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "directoryPropertyName": "CustomAttribute1",
      "annotations": [
        {
          "displayName": "Cost Center",
          "localizations": [
            {
              "languageTag": "ru-RU",
              "displayName": "центр затрат"
            }
          ]
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List profileCardProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
