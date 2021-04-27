---
title: Criar profileCardProperty
description: Use essa API para criar um novo profileCardProperty.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 5c9b43c3ca76416db4d319fdfcd7631d5eaf3a9b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055586"
---
# <a name="create-profilecardproperty"></a><span data-ttu-id="05112-103">Criar profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="05112-103">Create profileCardProperty</span></span>

<span data-ttu-id="05112-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05112-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05112-105">Crie um novo [profileCardProperty](../resources/profilecardproperty.md) para uma organização.</span><span class="sxs-lookup"><span data-stu-id="05112-105">Create a new [profileCardProperty](../resources/profilecardproperty.md) for an organization.</span></span> <span data-ttu-id="05112-106">A nova propriedade é identificada por **sua propriedade directoryPropertyName.**</span><span class="sxs-lookup"><span data-stu-id="05112-106">The new property is identified by its **directoryPropertyName** property.</span></span>

<span data-ttu-id="05112-107">Para obter mais informações sobre como adicionar propriedades ao cartão de perfil de uma organização, consulte [personalizar o cartão de perfil](/graph/add-properties-profilecard).</span><span class="sxs-lookup"><span data-stu-id="05112-107">For more information on adding properties to the profile card for an organization, see [customize the profile card](/graph/add-properties-profilecard).</span></span>

## <a name="permissions"></a><span data-ttu-id="05112-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="05112-108">Permissions</span></span>

<span data-ttu-id="05112-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05112-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="05112-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05112-111">Permission type</span></span>                        | <span data-ttu-id="05112-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="05112-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="05112-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05112-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="05112-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05112-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="05112-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05112-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05112-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05112-116">Not supported.</span></span>                              |
| <span data-ttu-id="05112-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05112-117">Application</span></span>                            | <span data-ttu-id="05112-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05112-118">Not supported.</span></span>                              |

><span data-ttu-id="05112-119">**Observação:** O uso de permissões delegadas para essa operação exige que o usuário in-loco tenha um administrador de locatário ou uma função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="05112-119">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="05112-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05112-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties
```

## <a name="request-headers"></a><span data-ttu-id="05112-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05112-121">Request headers</span></span>

| <span data-ttu-id="05112-122">Nome</span><span class="sxs-lookup"><span data-stu-id="05112-122">Name</span></span>          |<span data-ttu-id="05112-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="05112-123">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="05112-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="05112-124">Authorization</span></span> | <span data-ttu-id="05112-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05112-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="05112-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="05112-127">Content-Type</span></span>  | <span data-ttu-id="05112-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05112-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="05112-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05112-130">Request body</span></span>

<span data-ttu-id="05112-131">No corpo da solicitação, fornece uma representação JSON de um [objeto profileCardProperty.](../resources/profilecardproperty.md)</span><span class="sxs-lookup"><span data-stu-id="05112-131">In the request body, supply a JSON representation of a [profileCardProperty](../resources/profilecardproperty.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="05112-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="05112-132">Response</span></span>

<span data-ttu-id="05112-133">Se tiver êxito, este método retornará `201 Created` o código de resposta e um novo objeto [profileCardProperty](../resources/profilecardproperty.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05112-133">If successful, this method returns `201 Created` response code and a new [profileCardProperty](../resources/profilecardproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="05112-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="05112-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="05112-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05112-135">Request</span></span>

<span data-ttu-id="05112-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="05112-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="05112-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="05112-137">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="05112-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05112-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-profilecardproperty-from-organizationsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="05112-139">C#</span><span class="sxs-lookup"><span data-stu-id="05112-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-profilecardproperty-from-organizationsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="05112-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05112-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-profilecardproperty-from-organizationsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="05112-141">Java</span><span class="sxs-lookup"><span data-stu-id="05112-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-profilecardproperty-from-organizationsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="05112-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="05112-142">Response</span></span>

<span data-ttu-id="05112-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="05112-143">The following is an example of the response.</span></span>

> <span data-ttu-id="05112-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="05112-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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


