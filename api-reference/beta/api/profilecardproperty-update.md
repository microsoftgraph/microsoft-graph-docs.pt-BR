---
title: Atualizar profileCardProperty
description: Atualize as propriedades de um objeto profileCardProperty.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 53d95deee5be591745e62d7c41b2ab232b3b19d8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036685"
---
# <a name="update-profilecardproperty"></a><span data-ttu-id="ab61f-103">Atualizar profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="ab61f-103">Update profileCardProperty</span></span>

<span data-ttu-id="ab61f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab61f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab61f-105">Atualize as propriedades de [um objeto profileCardProperty,](../resources/profilecardproperty.md) identificado por **sua propriedade directoryPropertyName.**</span><span class="sxs-lookup"><span data-stu-id="ab61f-105">Update the properties of a [profileCardProperty](../resources/profilecardproperty.md) object, identified by its **directoryPropertyName** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab61f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab61f-106">Permissions</span></span>

<span data-ttu-id="ab61f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab61f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ab61f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab61f-109">Permission type</span></span>                        | <span data-ttu-id="ab61f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab61f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ab61f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab61f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ab61f-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab61f-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="ab61f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab61f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab61f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab61f-114">Not supported.</span></span>                              |
| <span data-ttu-id="ab61f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab61f-115">Application</span></span>                            | <span data-ttu-id="ab61f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab61f-116">Not supported.</span></span>                              |

><span data-ttu-id="ab61f-117">**Observação:** O uso de permissões delegadas para essa operação exige que o usuário in-loco tenha um administrador de locatário ou uma função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="ab61f-117">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="ab61f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab61f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ab61f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab61f-119">Request headers</span></span>

| <span data-ttu-id="ab61f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ab61f-120">Name</span></span>       | <span data-ttu-id="ab61f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab61f-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ab61f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab61f-122">Authorization</span></span> | <span data-ttu-id="ab61f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab61f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ab61f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ab61f-125">Content-Type</span></span>  | <span data-ttu-id="ab61f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab61f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab61f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab61f-128">Request body</span></span>

<span data-ttu-id="ab61f-129">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="ab61f-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ab61f-130">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="ab61f-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ab61f-131">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ab61f-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ab61f-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab61f-132">Property</span></span>     | <span data-ttu-id="ab61f-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab61f-133">Type</span></span>        | <span data-ttu-id="ab61f-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab61f-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ab61f-135">anotações</span><span class="sxs-lookup"><span data-stu-id="ab61f-135">annotations</span></span>|<span data-ttu-id="ab61f-136">Coleção profileCardAnnotation</span><span class="sxs-lookup"><span data-stu-id="ab61f-136">profileCardAnnotation collection</span></span>| <span data-ttu-id="ab61f-137">Contém qualquer rótulo alternativo ou localizado que um administrador optou por especificar.</span><span class="sxs-lookup"><span data-stu-id="ab61f-137">Contains any alternative or localized labels an administrator has chosen to specify.</span></span>|
|<span data-ttu-id="ab61f-138">directoryPropertyName</span><span class="sxs-lookup"><span data-stu-id="ab61f-138">directoryPropertyName</span></span>|<span data-ttu-id="ab61f-139">String</span><span class="sxs-lookup"><span data-stu-id="ab61f-139">String</span></span>|<span data-ttu-id="ab61f-140">Contém o nome da propriedade directory que se destina a aparecer no cartão de perfil.</span><span class="sxs-lookup"><span data-stu-id="ab61f-140">Contains the name of the directory property which is intended to surface on the profile card.</span></span> |

## <a name="response"></a><span data-ttu-id="ab61f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab61f-141">Response</span></span>

<span data-ttu-id="ab61f-142">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto profileCardProperty](../resources/profilecardproperty.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab61f-142">If successful, this method returns a `200 OK` response code and an updated [profileCardProperty](../resources/profilecardproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ab61f-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ab61f-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ab61f-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab61f-144">Request</span></span>

<span data-ttu-id="ab61f-145">O exemplo a seguir adiciona um rótulo localizado "Kostnads Senter" para a localidade "no-NB".</span><span class="sxs-lookup"><span data-stu-id="ab61f-145">The following example adds a localized label "Kostnads Senter" for the locale "no-NB".</span></span>

# <a name="http"></a>[<span data-ttu-id="ab61f-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab61f-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilecardproperty"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/CustomAttribute1
Content-type: application/json

{
  "annotations": [
    {
      "localizations": [
        {
          "languageTag": "no-NB",
          "displayName": "Kostnads Senter"
        }
      ]
    }
  ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="ab61f-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab61f-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilecardproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="ab61f-148">C#</span><span class="sxs-lookup"><span data-stu-id="ab61f-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-profilecardproperty-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab61f-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab61f-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-profilecardproperty-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ab61f-150">Java</span><span class="sxs-lookup"><span data-stu-id="ab61f-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-profilecardproperty-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ab61f-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab61f-151">Response</span></span>

<span data-ttu-id="ab61f-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ab61f-152">The following is an example of the response.</span></span>

> <span data-ttu-id="ab61f-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ab61f-153">**Note:** The response object shown here might be shortened for readability.</span></span>

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
        },
        {
          "languageTag": "no-NB",
          "displayName": "Kostnads Senter"
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
  "description": "Update profilecardproperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


