---
title: Obter organizationSettings
description: Recupere as propriedades e os relacionamentos do objeto organizationSettings.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 755c71a85fe906c1fdf4b24dbceb3a0056d271b3
ms.sourcegitcommit: 20b951f8bd245bb3a2bc7d3f5533e8619e9db084
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/27/2020
ms.locfileid: "45427113"
---
# <a name="get-organizationsettings"></a><span data-ttu-id="4c338-103">Obter organizationSettings</span><span class="sxs-lookup"><span data-stu-id="4c338-103">Get organizationSettings</span></span>

<span data-ttu-id="4c338-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c338-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c338-105">Recupere as propriedades e os relacionamentos de um objeto [organizationSettings](../resources/organizationsettings.md) , incluindo **profileCardProperties**.</span><span class="sxs-lookup"><span data-stu-id="4c338-105">Retrieve the properties and relationships of an [organizationSettings](../resources/organizationsettings.md) object, including **profileCardProperties**.</span></span>

<span data-ttu-id="4c338-106">Essa operação não retorna [itemInsightsSettings](../resources/iteminsightssettings.md) por meio da propriedade de navegação **persights** .</span><span class="sxs-lookup"><span data-stu-id="4c338-106">This operation does not return [itemInsightsSettings](../resources/iteminsightssettings.md) through the **itemInsights** navigation property.</span></span> <span data-ttu-id="4c338-107">Use [Get itemInsightsSettings](iteminsightssettings-get.md) em vez disso.</span><span class="sxs-lookup"><span data-stu-id="4c338-107">Use [get itemInsightsSettings](iteminsightssettings-get.md) instead.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c338-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="4c338-108">Permissions</span></span>

<span data-ttu-id="4c338-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c338-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c338-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c338-111">Permission type</span></span>                        | <span data-ttu-id="4c338-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4c338-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4c338-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c338-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="4c338-114">User. Read, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="4c338-114">User.Read, User.Read.All</span></span>                    |
| <span data-ttu-id="4c338-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c338-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c338-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c338-116">Not supported.</span></span>                              |
| <span data-ttu-id="4c338-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c338-117">Application</span></span>                            | <span data-ttu-id="4c338-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c338-118">Not supported.</span></span>                              |

><span data-ttu-id="4c338-119">**Observação:** O uso de permissões delegadas para esta operação exige que o usuário conectado tenha um administrador de locatários ou uma função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="4c338-119">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="4c338-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c338-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4c338-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4c338-121">Optional query parameters</span></span>

<span data-ttu-id="4c338-122">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4c338-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4c338-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4c338-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c338-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c338-124">Request headers</span></span>

| <span data-ttu-id="4c338-125">Nome</span><span class="sxs-lookup"><span data-stu-id="4c338-125">Name</span></span>          |<span data-ttu-id="4c338-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c338-126">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="4c338-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c338-127">Authorization</span></span> | <span data-ttu-id="4c338-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c338-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="4c338-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4c338-130">Content-Type</span></span>  | <span data-ttu-id="4c338-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c338-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c338-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c338-133">Request body</span></span>

<span data-ttu-id="4c338-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4c338-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c338-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c338-135">Response</span></span>

<span data-ttu-id="4c338-136">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [organizationSettings](../resources/organizationsettings.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c338-136">If successful, this method returns a `200 OK` response code and the requested [organizationSettings](../resources/organizationsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4c338-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4c338-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4c338-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c338-138">Request</span></span>

<span data-ttu-id="4c338-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c338-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4c338-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c338-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationsettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/settings
```
# <a name="c"></a>[<span data-ttu-id="4c338-141">C#</span><span class="sxs-lookup"><span data-stu-id="4c338-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c338-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c338-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c338-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c338-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4c338-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c338-144">Response</span></span>

<span data-ttu-id="4c338-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4c338-145">The following is an example of the response.</span></span>

> <span data-ttu-id="4c338-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c338-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
