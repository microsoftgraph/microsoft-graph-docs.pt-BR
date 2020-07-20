---
title: Obter organizationSettings
description: Recupere as propriedades e os relacionamentos do objeto organizationSettings.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 1de3e239f64b81a6e8f2995bfa626a0d7734ef9e
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080673"
---
# <a name="get-organizationsettings"></a><span data-ttu-id="ccef0-103">Obter organizationSettings</span><span class="sxs-lookup"><span data-stu-id="ccef0-103">Get organizationSettings</span></span>

<span data-ttu-id="ccef0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccef0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccef0-105">Recupere as propriedades e os relacionamentos de um objeto [organizationSettings](../resources/organizationsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="ccef0-105">Retrieve the properties and relationships of an [organizationSettings](../resources/organizationsettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ccef0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ccef0-106">Permissions</span></span>

<span data-ttu-id="ccef0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccef0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ccef0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ccef0-109">Permission type</span></span>                        | <span data-ttu-id="ccef0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ccef0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ccef0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ccef0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ccef0-112">User. Read, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="ccef0-112">User.Read, User.Read.All</span></span>                    |
| <span data-ttu-id="ccef0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ccef0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccef0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ccef0-114">Not supported.</span></span>                              |
| <span data-ttu-id="ccef0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ccef0-115">Application</span></span>                            | <span data-ttu-id="ccef0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ccef0-116">Not supported.</span></span>                              |

><span data-ttu-id="ccef0-117">**Observação:** O uso de permissões delegadas para esta operação exige que o usuário conectado tenha um administrador de locatários ou uma função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="ccef0-117">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="ccef0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ccef0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ccef0-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ccef0-119">Optional query parameters</span></span>

<span data-ttu-id="ccef0-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ccef0-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ccef0-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ccef0-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ccef0-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ccef0-122">Request headers</span></span>

| <span data-ttu-id="ccef0-123">Nome</span><span class="sxs-lookup"><span data-stu-id="ccef0-123">Name</span></span>          |<span data-ttu-id="ccef0-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccef0-124">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="ccef0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ccef0-125">Authorization</span></span> | <span data-ttu-id="ccef0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ccef0-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="ccef0-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ccef0-128">Content-Type</span></span>  | <span data-ttu-id="ccef0-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ccef0-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ccef0-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ccef0-131">Request body</span></span>

<span data-ttu-id="ccef0-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ccef0-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ccef0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccef0-133">Response</span></span>

<span data-ttu-id="ccef0-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [organizationSettings](../resources/organizationsettings.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ccef0-134">If successful, this method returns a `200 OK` response code and the requested [organizationSettings](../resources/organizationsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ccef0-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ccef0-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ccef0-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ccef0-136">Request</span></span>

<span data-ttu-id="ccef0-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ccef0-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ccef0-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccef0-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationsettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/settings
```
# <a name="c"></a>[<span data-ttu-id="ccef0-139">C#</span><span class="sxs-lookup"><span data-stu-id="ccef0-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ccef0-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccef0-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ccef0-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccef0-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ccef0-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccef0-142">Response</span></span>

<span data-ttu-id="ccef0-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ccef0-143">The following is an example of the response.</span></span>

> <span data-ttu-id="ccef0-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ccef0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "345233-676277-644334-445677-334556",
  "profileCardProperties": [
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
  "description": "Get organizationSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
