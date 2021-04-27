---
title: Obter profileCardProperty
description: Recupere as propriedades e as relações de um objeto profileCardProperty.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 35c6f2cf1d0beb56d1dafbc8e31b93973e0e2aa5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036711"
---
# <a name="get-profilecardproperty"></a><span data-ttu-id="2cf66-103">Obter profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="2cf66-103">Get profileCardProperty</span></span>

<span data-ttu-id="2cf66-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cf66-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2cf66-105">Recupere as propriedades e as relações de uma entidade [profileCardProperty,](../resources/profilecardproperty.md) que contém as personalizações de cartão de perfil que existem em sua organização Microsoft 365 para um determinado campo.</span><span class="sxs-lookup"><span data-stu-id="2cf66-105">Retrieve the properties and relationships of a [profileCardProperty](../resources/profilecardproperty.md) entity, which contains the profile card customizations that exist in your Microsoft 365 organization for a given field.</span></span> <span data-ttu-id="2cf66-106">O profileCardProperty é identificado por **sua propriedade directoryPropertyName.**</span><span class="sxs-lookup"><span data-stu-id="2cf66-106">The profileCardProperty is identified by its **directoryPropertyName** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="2cf66-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2cf66-107">Permissions</span></span>

<span data-ttu-id="2cf66-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cf66-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2cf66-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2cf66-110">Permission type</span></span>                        | <span data-ttu-id="2cf66-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2cf66-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2cf66-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2cf66-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2cf66-113">User.Read, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2cf66-113">User.Read, User.Read.All</span></span>                    |
| <span data-ttu-id="2cf66-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2cf66-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2cf66-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2cf66-115">Not supported.</span></span>                              |
| <span data-ttu-id="2cf66-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2cf66-116">Application</span></span>                            | <span data-ttu-id="2cf66-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2cf66-117">Not supported.</span></span>                              |

><span data-ttu-id="2cf66-118">**Observação:** O uso de permissões delegadas para essa operação exige que o usuário in-loco tenha um administrador de locatário ou uma função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="2cf66-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="2cf66-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2cf66-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2cf66-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2cf66-120">Optional query parameters</span></span>

<span data-ttu-id="2cf66-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2cf66-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2cf66-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2cf66-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2cf66-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2cf66-123">Request headers</span></span>

| <span data-ttu-id="2cf66-124">Nome</span><span class="sxs-lookup"><span data-stu-id="2cf66-124">Name</span></span>      |<span data-ttu-id="2cf66-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cf66-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2cf66-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="2cf66-126">Authorization</span></span> | <span data-ttu-id="2cf66-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2cf66-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2cf66-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2cf66-129">Request body</span></span>

<span data-ttu-id="2cf66-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2cf66-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2cf66-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2cf66-131">Response</span></span>

<span data-ttu-id="2cf66-132">Se tiver êxito, este método retornará um código de `200 OK` resposta e o objeto [profileCardProperty](../resources/profilecardproperty.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2cf66-132">If successful, this method returns a `200 OK` response code and the requested [profileCardProperty](../resources/profilecardproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2cf66-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2cf66-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2cf66-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2cf66-134">Request</span></span>

<span data-ttu-id="2cf66-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2cf66-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2cf66-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2cf66-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profilecardproperty"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/{id}
```
# <a name="c"></a>[<span data-ttu-id="2cf66-137">C#</span><span class="sxs-lookup"><span data-stu-id="2cf66-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profilecardproperty-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2cf66-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2cf66-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profilecardproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2cf66-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2cf66-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profilecardproperty-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2cf66-140">Java</span><span class="sxs-lookup"><span data-stu-id="2cf66-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-profilecardproperty-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2cf66-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2cf66-141">Response</span></span>

<span data-ttu-id="2cf66-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2cf66-142">The following is an example of the response.</span></span>

> <span data-ttu-id="2cf66-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2cf66-143">**Note:** The response object shown here might be shortened for readability.</span></span>

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


