---
title: Listar profileCardProperties
description: Recupere uma lista de objetos profilecardproperty.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 7d0c064b6d422285d078a07edbc2ef24184a7d2a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052051"
---
# <a name="list-profilecardproperties"></a><span data-ttu-id="3c922-103">Listar profileCardProperties</span><span class="sxs-lookup"><span data-stu-id="3c922-103">List profileCardProperties</span></span>

<span data-ttu-id="3c922-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c922-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c922-105">Obter uma coleção de [recursos profileCardProperty](../resources/profilecardproperty.md) de uma organização.</span><span class="sxs-lookup"><span data-stu-id="3c922-105">Get a collection of [profileCardProperty](../resources/profilecardproperty.md) resources of an organization.</span></span> <span data-ttu-id="3c922-106">Cada recurso é identificado por **sua propriedade directoryPropertyName.**</span><span class="sxs-lookup"><span data-stu-id="3c922-106">Each resource is identified by its **directoryPropertyName** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c922-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3c922-107">Permissions</span></span>

<span data-ttu-id="3c922-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c922-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3c922-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c922-110">Permission type</span></span>                        | <span data-ttu-id="3c922-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3c922-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3c922-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c922-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3c922-113">User.Read, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c922-113">User.Read, User.Read.All</span></span>                    |
| <span data-ttu-id="3c922-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c922-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c922-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c922-115">Not supported.</span></span>                              |
| <span data-ttu-id="3c922-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c922-116">Application</span></span>                            | <span data-ttu-id="3c922-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c922-117">Not supported.</span></span>                              |

><span data-ttu-id="3c922-118">**Observação:** O uso de permissões delegadas para essa operação exige que o usuário in-loco tenha um administrador de locatário ou uma função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="3c922-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="3c922-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c922-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3c922-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3c922-120">Optional query parameters</span></span>

<span data-ttu-id="3c922-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3c922-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3c922-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3c922-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c922-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c922-123">Request headers</span></span>

| <span data-ttu-id="3c922-124">Nome</span><span class="sxs-lookup"><span data-stu-id="3c922-124">Name</span></span>          |<span data-ttu-id="3c922-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c922-125">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="3c922-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c922-126">Authorization</span></span> | <span data-ttu-id="3c922-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c922-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="3c922-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3c922-129">Content-Type</span></span>  | <span data-ttu-id="3c922-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c922-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c922-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c922-132">Request body</span></span>

<span data-ttu-id="3c922-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3c922-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c922-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c922-134">Response</span></span>

<span data-ttu-id="3c922-135">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objetos profileCardProperty](../resources/profilecardproperty.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c922-135">If successful, this method returns a `200 OK` response code and a collection of [profileCardProperty](../resources/profilecardproperty.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3c922-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3c922-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3c922-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c922-137">Request</span></span>

<span data-ttu-id="3c922-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c922-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3c922-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c922-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profilecardproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties
```
# <a name="c"></a>[<span data-ttu-id="3c922-140">C#</span><span class="sxs-lookup"><span data-stu-id="3c922-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profilecardproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c922-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c922-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profilecardproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c922-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c922-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profilecardproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3c922-143">Java</span><span class="sxs-lookup"><span data-stu-id="3c922-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-profilecardproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3c922-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c922-144">Response</span></span>

<span data-ttu-id="3c922-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3c922-145">The following is an example of the response.</span></span>

> <span data-ttu-id="3c922-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3c922-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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


