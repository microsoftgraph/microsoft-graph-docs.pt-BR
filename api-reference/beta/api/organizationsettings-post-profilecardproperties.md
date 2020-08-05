---
title: Criar profileCardProperty
description: Use esta API para criar um novo profileCardProperty.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: fc40b90cf390cc4e996b66bda0929ddd99c824d0
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566640"
---
# <a name="create-profilecardproperty"></a><span data-ttu-id="6da7b-103">Criar profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="6da7b-103">Create profileCardProperty</span></span>

<span data-ttu-id="6da7b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6da7b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6da7b-105">Crie um novo [profileCardProperty](../resources/profilecardproperty.md) para uma organização.</span><span class="sxs-lookup"><span data-stu-id="6da7b-105">Create a new [profileCardProperty](../resources/profilecardproperty.md) for an organization.</span></span> <span data-ttu-id="6da7b-106">A nova propriedade é identificada pela propriedade **directoryPropertyName** .</span><span class="sxs-lookup"><span data-stu-id="6da7b-106">The new property is identified by its **directoryPropertyName** property.</span></span>

<span data-ttu-id="6da7b-107">Para obter mais informações sobre como adicionar propriedades ao cartão de perfil de uma organização, consulte [Customize The Profile Card](/graph/add-properties-profilecard).</span><span class="sxs-lookup"><span data-stu-id="6da7b-107">For more information on adding properties to the profile card for an organization, see [customize the profile card](/graph/add-properties-profilecard).</span></span>

## <a name="permissions"></a><span data-ttu-id="6da7b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="6da7b-108">Permissions</span></span>

<span data-ttu-id="6da7b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6da7b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6da7b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6da7b-111">Permission type</span></span>                        | <span data-ttu-id="6da7b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6da7b-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6da7b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6da7b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="6da7b-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6da7b-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="6da7b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6da7b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6da7b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6da7b-116">Not supported.</span></span>                              |
| <span data-ttu-id="6da7b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6da7b-117">Application</span></span>                            | <span data-ttu-id="6da7b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6da7b-118">Not supported.</span></span>                              |

><span data-ttu-id="6da7b-119">**Observação:** O uso de permissões delegadas para esta operação exige que o usuário conectado tenha um administrador de locatários ou uma função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="6da7b-119">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="6da7b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6da7b-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties
```

## <a name="request-headers"></a><span data-ttu-id="6da7b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6da7b-121">Request headers</span></span>

| <span data-ttu-id="6da7b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="6da7b-122">Name</span></span>          |<span data-ttu-id="6da7b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6da7b-123">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="6da7b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6da7b-124">Authorization</span></span> | <span data-ttu-id="6da7b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6da7b-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="6da7b-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6da7b-127">Content-Type</span></span>  | <span data-ttu-id="6da7b-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6da7b-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6da7b-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6da7b-130">Request body</span></span>

<span data-ttu-id="6da7b-131">No corpo da solicitação, forneça uma representação JSON de um objeto [profileCardProperty](../resources/profilecardproperty.md) .</span><span class="sxs-lookup"><span data-stu-id="6da7b-131">In the request body, supply a JSON representation of a [profileCardProperty](../resources/profilecardproperty.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6da7b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="6da7b-132">Response</span></span>

<span data-ttu-id="6da7b-133">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um novo objeto [profileCardProperty](../resources/profilecardproperty.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6da7b-133">If successful, this method returns `201 Created` response code and a new [profileCardProperty](../resources/profilecardproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6da7b-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6da7b-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6da7b-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6da7b-135">Request</span></span>

<span data-ttu-id="6da7b-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6da7b-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6da7b-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="6da7b-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_profilecardproperty_from_organizationsettings"
}-->

```http
POST https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties
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
# <a name="javascript"></a>[<span data-ttu-id="6da7b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6da7b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-profilecardproperty-from-organizationsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="6da7b-139">C#</span><span class="sxs-lookup"><span data-stu-id="6da7b-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-profilecardproperty-from-organizationsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6da7b-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6da7b-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-profilecardproperty-from-organizationsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6da7b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="6da7b-141">Response</span></span>

<span data-ttu-id="6da7b-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6da7b-142">The following is an example of the response.</span></span>

> <span data-ttu-id="6da7b-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6da7b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profileCardProperty"
} -->

```http
HTTP/1.1 201 Created
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
  "description": "Create profileCardProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
