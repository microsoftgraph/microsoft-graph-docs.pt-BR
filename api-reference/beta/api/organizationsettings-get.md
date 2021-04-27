---
title: Obter organizationSettings
description: Recupere as propriedades e as relações do objeto organizationSettings.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 53bf7e03d56ad949683b0c363af3d4aa017502d6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052065"
---
# <a name="get-organizationsettings"></a><span data-ttu-id="9894f-103">Obter organizationSettings</span><span class="sxs-lookup"><span data-stu-id="9894f-103">Get organizationSettings</span></span>

<span data-ttu-id="9894f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9894f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9894f-105">Recupere as propriedades e as relações de um [objeto organizationSettings,](../resources/organizationsettings.md) incluindo **profileCardProperties**.</span><span class="sxs-lookup"><span data-stu-id="9894f-105">Retrieve the properties and relationships of an [organizationSettings](../resources/organizationsettings.md) object, including **profileCardProperties**.</span></span>

<span data-ttu-id="9894f-106">Esta operação não retorna [itemInsightsSettings](../resources/iteminsightssettings.md) por meio da propriedade de navegação **itemInsights.**</span><span class="sxs-lookup"><span data-stu-id="9894f-106">This operation does not return [itemInsightsSettings](../resources/iteminsightssettings.md) through the **itemInsights** navigation property.</span></span> <span data-ttu-id="9894f-107">Use [get itemInsightsSettings](iteminsightssettings-get.md) em vez disso.</span><span class="sxs-lookup"><span data-stu-id="9894f-107">Use [get itemInsightsSettings](iteminsightssettings-get.md) instead.</span></span>

## <a name="permissions"></a><span data-ttu-id="9894f-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="9894f-108">Permissions</span></span>

<span data-ttu-id="9894f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9894f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9894f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9894f-111">Permission type</span></span>                        | <span data-ttu-id="9894f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9894f-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9894f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9894f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="9894f-114">User.Read, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9894f-114">User.Read, User.Read.All</span></span>                    |
| <span data-ttu-id="9894f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9894f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9894f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9894f-116">Not supported.</span></span>                              |
| <span data-ttu-id="9894f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9894f-117">Application</span></span>                            | <span data-ttu-id="9894f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9894f-118">Not supported.</span></span>                              |

><span data-ttu-id="9894f-119">**Observação:** O uso de permissões delegadas para essa operação exige que o usuário in-loco tenha um administrador de locatário ou uma função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="9894f-119">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="9894f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9894f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9894f-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9894f-121">Optional query parameters</span></span>

<span data-ttu-id="9894f-122">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9894f-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="9894f-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9894f-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9894f-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9894f-124">Request headers</span></span>

| <span data-ttu-id="9894f-125">Nome</span><span class="sxs-lookup"><span data-stu-id="9894f-125">Name</span></span>          |<span data-ttu-id="9894f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="9894f-126">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="9894f-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="9894f-127">Authorization</span></span> | <span data-ttu-id="9894f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9894f-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="9894f-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9894f-130">Content-Type</span></span>  | <span data-ttu-id="9894f-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9894f-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9894f-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9894f-133">Request body</span></span>

<span data-ttu-id="9894f-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9894f-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9894f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9894f-135">Response</span></span>

<span data-ttu-id="9894f-136">Se tiver êxito, este método retornará um código de `200 OK` resposta e o objeto [organizationSettings](../resources/organizationsettings.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9894f-136">If successful, this method returns a `200 OK` response code and the requested [organizationSettings](../resources/organizationsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9894f-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9894f-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9894f-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9894f-138">Request</span></span>

<span data-ttu-id="9894f-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9894f-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9894f-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="9894f-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationsettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/settings
```
# <a name="c"></a>[<span data-ttu-id="9894f-141">C#</span><span class="sxs-lookup"><span data-stu-id="9894f-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9894f-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9894f-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9894f-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9894f-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9894f-144">Java</span><span class="sxs-lookup"><span data-stu-id="9894f-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9894f-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="9894f-145">Response</span></span>

<span data-ttu-id="9894f-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9894f-146">The following is an example of the response.</span></span>

> <span data-ttu-id="9894f-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9894f-147">**Note:** The response object shown here might be shortened for readability.</span></span>

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


