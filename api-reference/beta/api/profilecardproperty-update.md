---
title: Atualizar profileCardProperty
description: Atualiza as propriedades de um objeto profileCardProperty.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 122b8c0007067dafd2f7326cffc1b4e3b1697890
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123840"
---
# <a name="update-profilecardproperty"></a><span data-ttu-id="fa228-103">Atualizar profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="fa228-103">Update profileCardProperty</span></span>

<span data-ttu-id="fa228-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa228-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa228-105">Atualizar as propriedades de um objeto [profileCardProperty](../resources/profilecardproperty.md) , identificadas por sua propriedade **directoryPropertyName** .</span><span class="sxs-lookup"><span data-stu-id="fa228-105">Update the properties of a [profileCardProperty](../resources/profilecardproperty.md) object, identified by its **directoryPropertyName** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa228-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa228-106">Permissions</span></span>

<span data-ttu-id="fa228-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="fa228-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="fa228-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa228-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa228-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa228-109">Permission type</span></span>                        | <span data-ttu-id="fa228-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa228-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fa228-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa228-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa228-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="fa228-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="fa228-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa228-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa228-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa228-114">Not supported.</span></span>                              |
| <span data-ttu-id="fa228-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa228-115">Application</span></span>                            | <span data-ttu-id="fa228-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa228-116">Not supported.</span></span>                              |

><span data-ttu-id="fa228-117">**Observação:** O uso de permissões delegadas para esta operação exige que o usuário conectado tenha um administrador de locatários ou uma função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="fa228-117">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="fa228-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa228-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fa228-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa228-119">Request headers</span></span>

| <span data-ttu-id="fa228-120">Nome</span><span class="sxs-lookup"><span data-stu-id="fa228-120">Name</span></span>       | <span data-ttu-id="fa228-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa228-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="fa228-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa228-122">Authorization</span></span> | <span data-ttu-id="fa228-123">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="fa228-123">Bearer {token}.</span></span> <span data-ttu-id="fa228-124">Required.</span><span class="sxs-lookup"><span data-stu-id="fa228-124">Required.</span></span> |
| <span data-ttu-id="fa228-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fa228-125">Content-Type</span></span>  | <span data-ttu-id="fa228-126">application/json.</span><span class="sxs-lookup"><span data-stu-id="fa228-126">application/json.</span></span> <span data-ttu-id="fa228-127">Required.</span><span class="sxs-lookup"><span data-stu-id="fa228-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa228-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa228-128">Request body</span></span>

<span data-ttu-id="fa228-129">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="fa228-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="fa228-130">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="fa228-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="fa228-131">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="fa228-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fa228-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa228-132">Property</span></span>     | <span data-ttu-id="fa228-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa228-133">Type</span></span>        | <span data-ttu-id="fa228-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa228-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fa228-135">anotações</span><span class="sxs-lookup"><span data-stu-id="fa228-135">annotations</span></span>|<span data-ttu-id="fa228-136">coleção profileCardAnnotation</span><span class="sxs-lookup"><span data-stu-id="fa228-136">profileCardAnnotation collection</span></span>| <span data-ttu-id="fa228-137">Contém quaisquer rótulos alternativos ou localizados que um administrador optou por especificar.</span><span class="sxs-lookup"><span data-stu-id="fa228-137">Contains any alternative or localized labels an administrator has chosen to specify.</span></span>|
|<span data-ttu-id="fa228-138">directoryPropertyName</span><span class="sxs-lookup"><span data-stu-id="fa228-138">directoryPropertyName</span></span>|<span data-ttu-id="fa228-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fa228-139">String</span></span>|<span data-ttu-id="fa228-140">Contém o nome da propriedade de diretório que se destina à superfície no cartão de perfil.</span><span class="sxs-lookup"><span data-stu-id="fa228-140">Contains the name of the directory property which is intended to surface on the profile card.</span></span> |

## <a name="response"></a><span data-ttu-id="fa228-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa228-141">Response</span></span>

<span data-ttu-id="fa228-142">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [profileCardProperty](../resources/profilecardproperty.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa228-142">If successful, this method returns a `200 OK` response code and an updated [profileCardProperty](../resources/profilecardproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fa228-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fa228-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fa228-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa228-144">Request</span></span>

<span data-ttu-id="fa228-145">O exemplo a seguir adiciona um rótulo localizado "Kostnads Senter" para a localidade "no-NB".</span><span class="sxs-lookup"><span data-stu-id="fa228-145">The following example adds a localized label "Kostnads Senter" for the locale "no-NB".</span></span>

# <a name="http"></a>[<span data-ttu-id="fa228-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa228-146">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="fa228-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa228-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilecardproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fa228-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa228-148">Response</span></span>

<span data-ttu-id="fa228-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fa228-149">The following is an example of the response.</span></span>

> <span data-ttu-id="fa228-150">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="fa228-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fa228-151">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="fa228-151">All the properties will be returned from an actual call.</span></span>

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
