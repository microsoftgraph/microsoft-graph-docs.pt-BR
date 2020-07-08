---
title: Criar profileCardProperty
description: Use esta API para criar um novo profileCardProperty.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 24fe1a2f4257475849ecb3c057843d7cd0661a21
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080630"
---
# <a name="create-profilecardproperty"></a><span data-ttu-id="b8d13-103">Criar profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="b8d13-103">Create profileCardProperty</span></span>

<span data-ttu-id="b8d13-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8d13-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8d13-105">Crie um novo [profileCardProperty](../resources/profilecardproperty.md) para uma organização.</span><span class="sxs-lookup"><span data-stu-id="b8d13-105">Create a new [profileCardProperty](../resources/profilecardproperty.md) for an organization.</span></span> <span data-ttu-id="b8d13-106">A nova propriedade é identificada pela propriedade **directoryPropertyName** .</span><span class="sxs-lookup"><span data-stu-id="b8d13-106">The new property is identified by its **directoryPropertyName** property.</span></span>

<span data-ttu-id="b8d13-107">Para obter mais informações sobre como adicionar propriedades ao cartão de perfil de uma organização, consulte [Customize The Profile Card](/graph/add-properties-profilecard).</span><span class="sxs-lookup"><span data-stu-id="b8d13-107">For more information on adding properties to the profile card for an organization, see [customize the profile card](/graph/add-properties-profilecard).</span></span>

## <a name="permissions"></a><span data-ttu-id="b8d13-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8d13-108">Permissions</span></span>

<span data-ttu-id="b8d13-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b8d13-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b8d13-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8d13-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b8d13-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8d13-111">Permission type</span></span>                        | <span data-ttu-id="b8d13-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8d13-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b8d13-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8d13-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b8d13-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b8d13-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="b8d13-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8d13-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8d13-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8d13-116">Not supported.</span></span>                              |
| <span data-ttu-id="b8d13-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8d13-117">Application</span></span>                            | <span data-ttu-id="b8d13-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8d13-118">Not supported.</span></span>                              |

><span data-ttu-id="b8d13-119">**Observação:** O uso de permissões delegadas para esta operação exige que o usuário conectado tenha um administrador de locatários ou uma função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="b8d13-119">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="b8d13-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8d13-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/organization/settings/profileCardProperties
```

## <a name="request-headers"></a><span data-ttu-id="b8d13-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8d13-121">Request headers</span></span>

| <span data-ttu-id="b8d13-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b8d13-122">Name</span></span>          |<span data-ttu-id="b8d13-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8d13-123">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="b8d13-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8d13-124">Authorization</span></span> | <span data-ttu-id="b8d13-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="b8d13-125">Bearer {token}.</span></span> <span data-ttu-id="b8d13-126">Required.</span><span class="sxs-lookup"><span data-stu-id="b8d13-126">Required.</span></span>   |
| <span data-ttu-id="b8d13-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b8d13-127">Content-Type</span></span>  | <span data-ttu-id="b8d13-128">application/json.</span><span class="sxs-lookup"><span data-stu-id="b8d13-128">application/json.</span></span> <span data-ttu-id="b8d13-129">Required.</span><span class="sxs-lookup"><span data-stu-id="b8d13-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8d13-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8d13-130">Request body</span></span>

<span data-ttu-id="b8d13-131">No corpo da solicitação, forneça uma representação JSON de um objeto [profileCardProperty](../resources/profilecardproperty.md) .</span><span class="sxs-lookup"><span data-stu-id="b8d13-131">In the request body, supply a JSON representation of a [profileCardProperty](../resources/profilecardproperty.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b8d13-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8d13-132">Response</span></span>

<span data-ttu-id="b8d13-133">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um novo objeto [profileCardProperty](../resources/profilecardproperty.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8d13-133">If successful, this method returns `201 Created` response code and a new [profileCardProperty](../resources/profilecardproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b8d13-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b8d13-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b8d13-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8d13-135">Request</span></span>

<span data-ttu-id="b8d13-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8d13-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b8d13-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8d13-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_profilecardproperty_from_organizationsettings"
}-->

```http
POST https://graph.microsoft.com/beta/organization/settings/profileCardProperties
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
# <a name="javascript"></a>[<span data-ttu-id="b8d13-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8d13-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-profilecardproperty-from-organizationsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b8d13-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8d13-139">Response</span></span>

<span data-ttu-id="b8d13-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b8d13-140">The following is an example of the response.</span></span>

> <span data-ttu-id="b8d13-141">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="b8d13-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b8d13-142">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b8d13-142">All the properties will be returned from an actual call.</span></span>

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
