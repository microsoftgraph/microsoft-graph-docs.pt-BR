---
title: Atualizar schemaExtension
description: Atualize as propriedades na definição da schemaExtension especificada.
ms.openlocfilehash: 783999a22f41300f8ea086d98e755d72b3520685
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039414"
---
# <a name="update-schemaextension"></a><span data-ttu-id="bb76c-103">Atualizar schemaExtension</span><span class="sxs-lookup"><span data-stu-id="bb76c-103">Update schemaExtension</span></span>

> <span data-ttu-id="bb76c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bb76c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb76c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bb76c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bb76c-106">Atualize as propriedades na definição da [schemaExtension](../resources/schemaextension.md) especificada.</span><span class="sxs-lookup"><span data-stu-id="bb76c-106">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="bb76c-p102">A atualização se aplica a todos os recursos que estão incluídos na propriedade **targetTypes** da extensão. Esses recursos estão entre os [tipos de recurso de suporte](/graph/extensibility-overview#supported-resources).</span><span class="sxs-lookup"><span data-stu-id="bb76c-p102">The update applies to all the resources that are included in the **targetTypes** property of the extension. These resources are among the [supporting resource types](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="bb76c-p103">Somente o aplicativo que criou uma extensão de esquema (proprietário do aplicativo) pode fazer atualizações aditivas à extensão quando a extensão estiver com o status **InDevelopment** ou **Available**. Isso significa que o aplicativo não consegue remover propriedades personalizadas ou tipos de recursos de destino da definição. Porém, o aplicativo pode alterar a descrição da extensão.</span><span class="sxs-lookup"><span data-stu-id="bb76c-p103">Only the app that created a schema extension (owner app) can make additive updates to the extension when the extension is in the **InDevelopment** or **Available** status. That means the app cannot remove custom properties or target resource types from the definition. The app can, however, change the description of the extension.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb76c-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="bb76c-112">Permissions</span></span>

<span data-ttu-id="bb76c-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb76c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bb76c-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb76c-115">Permission type</span></span>      | <span data-ttu-id="bb76c-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bb76c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb76c-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb76c-117">Delegated (work or school account)</span></span> | <span data-ttu-id="bb76c-118">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bb76c-118">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bb76c-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb76c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb76c-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb76c-120">Not supported.</span></span>    |
|<span data-ttu-id="bb76c-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb76c-121">Application</span></span> | <span data-ttu-id="bb76c-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb76c-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb76c-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb76c-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="bb76c-124">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="bb76c-124">Optional request headers</span></span>

| <span data-ttu-id="bb76c-125">Nome</span><span class="sxs-lookup"><span data-stu-id="bb76c-125">Name</span></span>      |<span data-ttu-id="bb76c-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb76c-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bb76c-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb76c-127">Authorization</span></span>  | <span data-ttu-id="bb76c-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb76c-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bb76c-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bb76c-130">Content-Type</span></span>   | <span data-ttu-id="bb76c-131">application/json</span><span class="sxs-lookup"><span data-stu-id="bb76c-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb76c-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb76c-132">Request body</span></span>

<span data-ttu-id="bb76c-p106">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="bb76c-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bb76c-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb76c-136">Property</span></span>   | <span data-ttu-id="bb76c-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb76c-137">Type</span></span> |<span data-ttu-id="bb76c-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb76c-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb76c-139">description</span><span class="sxs-lookup"><span data-stu-id="bb76c-139">description</span></span>|<span data-ttu-id="bb76c-140">String</span><span class="sxs-lookup"><span data-stu-id="bb76c-140">String</span></span>|<span data-ttu-id="bb76c-141">Descrição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="bb76c-141">Description for the schema extension.</span></span>|
|<span data-ttu-id="bb76c-142">properties</span><span class="sxs-lookup"><span data-stu-id="bb76c-142">properties</span></span>|<span data-ttu-id="bb76c-143">Coleção [extensionSchemaProperty](../resources/extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="bb76c-143">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="bb76c-p107">A coleção de tipos e nomes de propriedades que compõem a definição da extensão de esquema. Somente as alterações aditivas são permitidas.</span><span class="sxs-lookup"><span data-stu-id="bb76c-p107">The collection of property names and types that make up the schema extension definition. Only additive changes are permitted.</span></span> |
|<span data-ttu-id="bb76c-146">status</span><span class="sxs-lookup"><span data-stu-id="bb76c-146">status</span></span>|<span data-ttu-id="bb76c-147">String</span><span class="sxs-lookup"><span data-stu-id="bb76c-147">String</span></span>|<span data-ttu-id="bb76c-148">O estado de ciclo de vida da extensão do esquema.</span><span class="sxs-lookup"><span data-stu-id="bb76c-148">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="bb76c-149">O estado inicial após a criação é **InDevelopment**.</span><span class="sxs-lookup"><span data-stu-id="bb76c-149">The initial state upon creation is **InDevelopment**.</span></span> <span data-ttu-id="bb76c-150">Transições de estados possíveis vão de **InDevelopment** a **disponível** e **disponível** para **obsoleto**.</span><span class="sxs-lookup"><span data-stu-id="bb76c-150">Possible states transitions are from **InDevelopment** to **Available** and **Available** to **Deprecated**.</span></span>|
|<span data-ttu-id="bb76c-151">targetTypes</span><span class="sxs-lookup"><span data-stu-id="bb76c-151">targetTypes</span></span>|<span data-ttu-id="bb76c-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb76c-152">String collection</span></span>|<span data-ttu-id="bb76c-p109">O conjunto de tipos do Microsoft Graph (que podem suportar extensões) ao qual a extensão de esquema pode ser aplicada.  Somente as alterações aditivas são permitidas.</span><span class="sxs-lookup"><span data-stu-id="bb76c-p109">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.  Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="bb76c-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb76c-155">Response</span></span>

<span data-ttu-id="bb76c-156">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bb76c-156">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bb76c-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb76c-157">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bb76c-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb76c-158">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="bb76c-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb76c-159">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="bb76c-160">Confira também</span><span class="sxs-lookup"><span data-stu-id="bb76c-160">See also</span></span>

- [<span data-ttu-id="bb76c-161">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="bb76c-161">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="bb76c-162">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="bb76c-162">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->