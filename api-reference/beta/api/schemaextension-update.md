---
title: Atualizar schemaExtension
description: Atualize as propriedades na definição da schemaExtension especificada.
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: f457609af15716ef2ada3945132afd285fd2394c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515535"
---
# <a name="update-schemaextension"></a><span data-ttu-id="c42f5-103">Atualizar schemaExtension</span><span class="sxs-lookup"><span data-stu-id="c42f5-103">Update schemaExtension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c42f5-104">Atualize as propriedades na definição da [schemaExtension](../resources/schemaextension.md) especificada.</span><span class="sxs-lookup"><span data-stu-id="c42f5-104">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="c42f5-p101">A atualização se aplica a todos os recursos que estão incluídos na propriedade **targetTypes** da extensão. Esses recursos estão entre os [tipos de recurso de suporte](/graph/extensibility-overview#supported-resources).</span><span class="sxs-lookup"><span data-stu-id="c42f5-p101">The update applies to all the resources that are included in the **targetTypes** property of the extension. These resources are among the [supporting resource types](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="c42f5-p102">Somente o aplicativo que criou uma extensão de esquema (proprietário do aplicativo) pode fazer atualizações aditivas à extensão quando a extensão estiver com o status **InDevelopment** ou **Available**. Isso significa que o aplicativo não consegue remover propriedades personalizadas ou tipos de recursos de destino da definição. Porém, o aplicativo pode alterar a descrição da extensão.</span><span class="sxs-lookup"><span data-stu-id="c42f5-p102">Only the app that created a schema extension (owner app) can make additive updates to the extension when the extension is in the **InDevelopment** or **Available** status. That means the app cannot remove custom properties or target resource types from the definition. The app can, however, change the description of the extension.</span></span>

## <a name="permissions"></a><span data-ttu-id="c42f5-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="c42f5-110">Permissions</span></span>

<span data-ttu-id="c42f5-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c42f5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c42f5-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c42f5-113">Permission type</span></span>      | <span data-ttu-id="c42f5-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c42f5-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c42f5-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c42f5-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c42f5-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c42f5-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c42f5-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c42f5-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c42f5-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c42f5-118">Not supported.</span></span>    |
|<span data-ttu-id="c42f5-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c42f5-119">Application</span></span> | <span data-ttu-id="c42f5-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c42f5-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c42f5-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c42f5-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="c42f5-122">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="c42f5-122">Optional request headers</span></span>

| <span data-ttu-id="c42f5-123">Nome</span><span class="sxs-lookup"><span data-stu-id="c42f5-123">Name</span></span>      |<span data-ttu-id="c42f5-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c42f5-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c42f5-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c42f5-125">Authorization</span></span>  | <span data-ttu-id="c42f5-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c42f5-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c42f5-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c42f5-128">Content-Type</span></span>   | <span data-ttu-id="c42f5-129">application/json</span><span class="sxs-lookup"><span data-stu-id="c42f5-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c42f5-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c42f5-130">Request body</span></span>

<span data-ttu-id="c42f5-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c42f5-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c42f5-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c42f5-134">Property</span></span>   | <span data-ttu-id="c42f5-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="c42f5-135">Type</span></span> |<span data-ttu-id="c42f5-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="c42f5-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c42f5-137">description</span><span class="sxs-lookup"><span data-stu-id="c42f5-137">description</span></span>|<span data-ttu-id="c42f5-138">String</span><span class="sxs-lookup"><span data-stu-id="c42f5-138">String</span></span>|<span data-ttu-id="c42f5-139">Descrição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="c42f5-139">Description for the schema extension.</span></span>|
|<span data-ttu-id="c42f5-140">properties</span><span class="sxs-lookup"><span data-stu-id="c42f5-140">properties</span></span>|<span data-ttu-id="c42f5-141">Coleção [extensionSchemaProperty](../resources/extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="c42f5-141">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="c42f5-p106">A coleção de tipos e nomes de propriedades que compõem a definição da extensão de esquema. Somente as alterações aditivas são permitidas.</span><span class="sxs-lookup"><span data-stu-id="c42f5-p106">The collection of property names and types that make up the schema extension definition. Only additive changes are permitted.</span></span> |
|<span data-ttu-id="c42f5-144">status</span><span class="sxs-lookup"><span data-stu-id="c42f5-144">status</span></span>|<span data-ttu-id="c42f5-145">String</span><span class="sxs-lookup"><span data-stu-id="c42f5-145">String</span></span>|<span data-ttu-id="c42f5-146">O estado de ciclo de vida da extensão do esquema.</span><span class="sxs-lookup"><span data-stu-id="c42f5-146">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="c42f5-147">O estado inicial após a criação é **InDevelopment**.</span><span class="sxs-lookup"><span data-stu-id="c42f5-147">The initial state upon creation is **InDevelopment**.</span></span> <span data-ttu-id="c42f5-148">Transições de estados possíveis vão de **InDevelopment** a **disponível** e **disponível** para **obsoleto**.</span><span class="sxs-lookup"><span data-stu-id="c42f5-148">Possible states transitions are from **InDevelopment** to **Available** and **Available** to **Deprecated**.</span></span>|
|<span data-ttu-id="c42f5-149">targetTypes</span><span class="sxs-lookup"><span data-stu-id="c42f5-149">targetTypes</span></span>|<span data-ttu-id="c42f5-150">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c42f5-150">String collection</span></span>|<span data-ttu-id="c42f5-p108">O conjunto de tipos do Microsoft Graph (que podem suportar extensões) ao qual a extensão de esquema pode ser aplicada.  Somente as alterações aditivas são permitidas.</span><span class="sxs-lookup"><span data-stu-id="c42f5-p108">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.  Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="c42f5-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="c42f5-153">Response</span></span>

<span data-ttu-id="c42f5-154">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c42f5-154">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c42f5-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c42f5-155">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c42f5-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c42f5-156">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/beta/schemaExtensions/{id}
Content-type: application/json
Content-length: 201

{
  "properties": [
    {
      "name":"new-name-value",
      "type":"new-type-value"
    },
    {
      "name":"additional-name-value",
      "type":"additional-type-value"
    }
  ],
}
```

##### <a name="response"></a><span data-ttu-id="c42f5-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="c42f5-157">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="c42f5-158">Confira também</span><span class="sxs-lookup"><span data-stu-id="c42f5-158">See also</span></span>

- [<span data-ttu-id="c42f5-159">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="c42f5-159">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="c42f5-160">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="c42f5-160">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schemaextension-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
