---
title: Obter profileCardProperty
description: Recupere as propriedades e os relacionamentos de um objeto profileCardProperty.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 11be3c0976515e800583b88898683548f5da92d7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980843"
---
# <a name="get-profilecardproperty"></a><span data-ttu-id="c5f7d-103">Obter profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="c5f7d-103">Get profileCardProperty</span></span>

<span data-ttu-id="c5f7d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5f7d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5f7d-105">Recupere as propriedades e os relacionamentos de uma entidade do [profileCardProperty](../resources/profilecardproperty.md) , que contém as personalizações de cartão de perfil existentes na sua organização do Microsoft 365 para um determinado campo.</span><span class="sxs-lookup"><span data-stu-id="c5f7d-105">Retrieve the properties and relationships of a [profileCardProperty](../resources/profilecardproperty.md) entity, which contains the profile card customizations that exist in your Microsoft 365 organization for a given field.</span></span> <span data-ttu-id="c5f7d-106">O profileCardProperty é identificado pela propriedade **directoryPropertyName** .</span><span class="sxs-lookup"><span data-stu-id="c5f7d-106">The profileCardProperty is identified by its **directoryPropertyName** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5f7d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c5f7d-107">Permissions</span></span>

<span data-ttu-id="c5f7d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5f7d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c5f7d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5f7d-110">Permission type</span></span>                        | <span data-ttu-id="c5f7d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5f7d-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c5f7d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5f7d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c5f7d-113">User. Read, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="c5f7d-113">User.Read, User.Read.All</span></span>                    |
| <span data-ttu-id="c5f7d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5f7d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5f7d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5f7d-115">Not supported.</span></span>                              |
| <span data-ttu-id="c5f7d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5f7d-116">Application</span></span>                            | <span data-ttu-id="c5f7d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5f7d-117">Not supported.</span></span>                              |

><span data-ttu-id="c5f7d-118">**Observação:** O uso de permissões delegadas para esta operação exige que o usuário conectado tenha um administrador de locatários ou uma função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="c5f7d-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="c5f7d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5f7d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c5f7d-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c5f7d-120">Optional query parameters</span></span>

<span data-ttu-id="c5f7d-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c5f7d-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c5f7d-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c5f7d-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5f7d-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5f7d-123">Request headers</span></span>

| <span data-ttu-id="c5f7d-124">Nome</span><span class="sxs-lookup"><span data-stu-id="c5f7d-124">Name</span></span>      |<span data-ttu-id="c5f7d-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5f7d-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c5f7d-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5f7d-126">Authorization</span></span> | <span data-ttu-id="c5f7d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5f7d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5f7d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5f7d-129">Request body</span></span>

<span data-ttu-id="c5f7d-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5f7d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5f7d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5f7d-131">Response</span></span>

<span data-ttu-id="c5f7d-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [profileCardProperty](../resources/profilecardproperty.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5f7d-132">If successful, this method returns a `200 OK` response code and the requested [profileCardProperty](../resources/profilecardproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c5f7d-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c5f7d-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c5f7d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5f7d-134">Request</span></span>

<span data-ttu-id="c5f7d-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5f7d-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c5f7d-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5f7d-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profilecardproperty"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/{id}
```
# <a name="c"></a>[<span data-ttu-id="c5f7d-137">C#</span><span class="sxs-lookup"><span data-stu-id="c5f7d-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profilecardproperty-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5f7d-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5f7d-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profilecardproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5f7d-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5f7d-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profilecardproperty-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5f7d-140">Java</span><span class="sxs-lookup"><span data-stu-id="c5f7d-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-profilecardproperty-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c5f7d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5f7d-141">Response</span></span>

<span data-ttu-id="c5f7d-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c5f7d-142">The following is an example of the response.</span></span>

> <span data-ttu-id="c5f7d-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5f7d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profileCardProperty"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get profileCardProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


