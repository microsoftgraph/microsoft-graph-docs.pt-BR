---
title: Criar schemaExtension
description: Criar uma nova definição schemaExtension para estender um tipo de recurso de suporte.
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 4cec2b0c62de094864efc92a8e75613c67c03382
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410595"
---
# <a name="create-schemaextension"></a><span data-ttu-id="885ca-103">Criar schemaExtension</span><span class="sxs-lookup"><span data-stu-id="885ca-103">Create schemaExtension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="885ca-104">Criar uma nova definição [schemaExtension](../resources/schemaextension.md) para estender um [tipo de recurso de suporte](/graph/extensibility-overview#supported-resources).</span><span class="sxs-lookup"><span data-stu-id="885ca-104">Create a new [schemaExtension](../resources/schemaextension.md) definition to extend a [supporting resource type](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="885ca-p101">As extensões de esquema permitem que você adicione dados personalizados fortemente tipados a um recurso. O aplicativo que cria uma extensão de esquema é o aplicativo proprietário. Dependendo do [estado](/graph/extensibility-overview#schema-extensions-lifecycle) da extensão, o aplicativo proprietário, e apenas o aplicativo proprietário, poderá atualizar ou excluir a extensão.</span><span class="sxs-lookup"><span data-stu-id="885ca-p101">Schema extensions let you add strongly-typed custom data to a resource. The app that creates a schema extension is the owner app. Depending on the [state](/graph/extensibility-overview#schema-extensions-lifecycle) of the extension, the owner app, and only the owner app, may update or delete the extension.</span></span> 

<span data-ttu-id="885ca-108">Veja exemplos de como [definir uma extensão de esquema que descreve um curso de treinamento](/graph/extensibility-schema-groups#2-register-a-schema-extension-definition-that-describes-a-training-course), usar a definição de extensão do esquema para [criar um novo grupo com dados do curso de treinamento](/graph/extensibility-schema-groups#3-create-a-new-group-with-extended-data) e [adicionar dados do curso de treinamento a um grupo existente](/graph/extensibility-schema-groups#4-add-update-or-remove-custom-data-in-an-existing-group).</span><span class="sxs-lookup"><span data-stu-id="885ca-108">See examples of how to [define a schema extension that describes a training course](/graph/extensibility-schema-groups#2-register-a-schema-extension-definition-that-describes-a-training-course), use the schema extension definition to [create a new group with training course data](/graph/extensibility-schema-groups#3-create-a-new-group-with-extended-data), and [add training course data to an existing group](/graph/extensibility-schema-groups#4-add-update-or-remove-custom-data-in-an-existing-group).</span></span>

## <a name="permissions"></a><span data-ttu-id="885ca-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="885ca-109">Permissions</span></span>
<span data-ttu-id="885ca-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="885ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="885ca-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="885ca-112">Permission type</span></span>      | <span data-ttu-id="885ca-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="885ca-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="885ca-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="885ca-114">Delegated (work or school account)</span></span> | <span data-ttu-id="885ca-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="885ca-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="885ca-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="885ca-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="885ca-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="885ca-117">Not supported.</span></span>    |
|<span data-ttu-id="885ca-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="885ca-118">Application</span></span> | <span data-ttu-id="885ca-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="885ca-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="885ca-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="885ca-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /schemaExtensions
```

## <a name="request-headers"></a><span data-ttu-id="885ca-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="885ca-121">Request headers</span></span>
| <span data-ttu-id="885ca-122">Nome</span><span class="sxs-lookup"><span data-stu-id="885ca-122">Name</span></span>       | <span data-ttu-id="885ca-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="885ca-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="885ca-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="885ca-124">Authorization</span></span>  | <span data-ttu-id="885ca-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="885ca-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="885ca-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="885ca-127">Content-Type</span></span>  | <span data-ttu-id="885ca-128">application/json</span><span class="sxs-lookup"><span data-stu-id="885ca-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="885ca-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="885ca-129">Request body</span></span>
<span data-ttu-id="885ca-130">No corpo da solicitação, forneça uma representação JSON de um objeto [schemaExtension](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="885ca-130">In the request body, supply a JSON representation of [schemaExtension](../resources/schemaextension.md) object.</span></span>

<span data-ttu-id="885ca-131">A tabela a seguir mostra as propriedades que estão disponíveis quando você cria uma extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="885ca-131">The following table shows the properties that are available when you create a schema extension.</span></span>

| <span data-ttu-id="885ca-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="885ca-132">Parameter</span></span> | <span data-ttu-id="885ca-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="885ca-133">Type</span></span> | <span data-ttu-id="885ca-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="885ca-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="885ca-135">description</span><span class="sxs-lookup"><span data-stu-id="885ca-135">description</span></span>|<span data-ttu-id="885ca-136">String</span><span class="sxs-lookup"><span data-stu-id="885ca-136">String</span></span>|<span data-ttu-id="885ca-137">Descrição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="885ca-137">Description for the schema extension.</span></span>|
|<span data-ttu-id="885ca-138">id</span><span class="sxs-lookup"><span data-stu-id="885ca-138">id</span></span>|<span data-ttu-id="885ca-139">String</span><span class="sxs-lookup"><span data-stu-id="885ca-139">String</span></span>|<span data-ttu-id="885ca-140">O identificador exclusivo da definição de extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="885ca-140">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="885ca-141">Você pode atribuir um valor em uma destas duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="885ca-141">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="885ca-142">Concatenar o nome de um de seus domínios verificados com um nome da extensão do esquema para formar uma cadeia de caracteres exclusiva neste formato, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span><span class="sxs-lookup"><span data-stu-id="885ca-142">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span></span> <span data-ttu-id="885ca-143">Como exemplo, `contoso_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="885ca-143">As an example, `contoso_mySchema`.</span></span> <span data-ttu-id="885ca-144">OBSERVAÇÃO: Apenas domínios verificados sob os seguintes domínios de nível superior têm suporte: `.com`,`.net`, `.gov`, `.edu` ou `.org`.</span><span class="sxs-lookup"><span data-stu-id="885ca-144">NOTE: Only verified domains under the following top-level domains are supported: `.com`,`.net`, `.gov`, `.edu` or `.org`.</span></span> </li><li><span data-ttu-id="885ca-p105">Forneça um nome de esquema e permita que o Microsoft Graph use esse nome de esquema para completar a atribuição de **id** neste formato: ext\{_&#65279;8-caracteres-alfanuméricos-aleatórios_\}\_\{_&#65279;nome-do-esquema_\}. Um exemplo seria `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="885ca-p105">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="885ca-147">Esta propriedade não pode ser alterada após a criação.</span><span class="sxs-lookup"><span data-stu-id="885ca-147">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="885ca-148">owner</span><span class="sxs-lookup"><span data-stu-id="885ca-148">owner</span></span>|<span data-ttu-id="885ca-149">String</span><span class="sxs-lookup"><span data-stu-id="885ca-149">String</span></span>|<span data-ttu-id="885ca-150">(Opcional) O `appId` do aplicativo que é o proprietário da extensão do esquema.</span><span class="sxs-lookup"><span data-stu-id="885ca-150">(Optional) The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="885ca-151">Essa propriedade pode ser fornecida na criação, para definir o proprietário.</span><span class="sxs-lookup"><span data-stu-id="885ca-151">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="885ca-152">Se não for fornecida, o aplicativo de chamada `appId` será definido como o proprietário.</span><span class="sxs-lookup"><span data-stu-id="885ca-152">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="885ca-153">Então, por exemplo, se criar uma nova definição de extensão do esquema usando o Explorador do Graph, você **deverá** fornecer a propriedade de proprietário.</span><span class="sxs-lookup"><span data-stu-id="885ca-153">So, for example, if creating a new schema extension definition using Graph Explorer, you **must** supply the owner property.</span></span> <span data-ttu-id="885ca-154">Uma vez definida, essa propriedade é somente leitura e não pode ser alterada.</span><span class="sxs-lookup"><span data-stu-id="885ca-154">Once set, this property is read-only and cannot be changed.</span></span>|
|<span data-ttu-id="885ca-155">properties</span><span class="sxs-lookup"><span data-stu-id="885ca-155">properties</span></span>|<span data-ttu-id="885ca-156">Coleção [extensionSchemaProperty](../resources/extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="885ca-156">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="885ca-157">A coleção de tipos e nomes de propriedades que compõem a definição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="885ca-157">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="885ca-158">targetTypes</span><span class="sxs-lookup"><span data-stu-id="885ca-158">targetTypes</span></span>|<span data-ttu-id="885ca-159">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="885ca-159">String collection</span></span>|<span data-ttu-id="885ca-160">O conjunto de tipos de recursos do Microsoft Graph (com suporte a extensões do esquema) ao qual esta extensão de esquema pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="885ca-160">Set of Microsoft Graph resource types (that support schema extensions) that this schema extension definition can be applied to.</span></span>|

## <a name="response"></a><span data-ttu-id="885ca-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="885ca-161">Response</span></span>

<span data-ttu-id="885ca-162">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [schemaExtension](../resources/schemaextension.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="885ca-162">If successful, this method returns `201 Created` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="885ca-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="885ca-163">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="885ca-164">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="885ca-164">Request 1</span></span>

<span data-ttu-id="885ca-p107">O primeiro exemplo mostra o uso de um nome de domínio verificado, `graphlearn` e um nome de esquema, `courses`, para formar uma cadeia de caracteres para a propriedade **id** da definição de extensão do esquema. A cadeia de caracteres exclusiva se baseia neste formato, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span><span class="sxs-lookup"><span data-stu-id="885ca-p107">The first example shows using a verified domain name, `graphlearn`, and a schema name, `courses`, to form a unique string for the **id** property of the schema extension definition. The unique string is based on this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span></span>

<span data-ttu-id="885ca-167">No corpo da solicitação, forneça uma representação JSON do objeto [schemaExtension](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="885ca-167">In the request body, supply a JSON representation of the [schemaExtension](../resources/schemaextension.md) object.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="885ca-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="885ca-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_1"
}-->
```http
POST https://graph.microsoft.com/beta/schemaExtensions
Content-type: application/json

{
    "id":"graphlearn_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="885ca-169">C#</span><span class="sxs-lookup"><span data-stu-id="885ca-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schemaextension-from-schemaextensions-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="885ca-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="885ca-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schemaextension-from-schemaextensions-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="885ca-171">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="885ca-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schemaextension-from-schemaextensions-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="885ca-172">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="885ca-172">Response 1</span></span>

<span data-ttu-id="885ca-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="885ca-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 420

{
    "id": "graphlearn_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "courseId",
            "type": "String"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

##### <a name="request-2"></a><span data-ttu-id="885ca-176">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="885ca-176">Request 2</span></span>

<span data-ttu-id="885ca-p109">O segundo exemplo mostra a especificação de apenas um nome de esquema, `courses`, na propriedade **id** na solicitação, junto com a representação JSON do resto das propriedades no objeto [schemaExtension](../resources/schemaextension.md). O Microsoft Graph atribuirá e retornará um valor exclusivo de cadeia de caracteres na resposta.</span><span class="sxs-lookup"><span data-stu-id="885ca-p109">The second example shows specifying just a schema name, `courses`, in the **id** property in the request, together with the JSON representation of the rest of the properties in the [schemaExtension](../resources/schemaextension.md) object. Microsoft Graph will assign and return a unique string value in the response.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="885ca-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="885ca-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_2"
}-->
```http
POST https://graph.microsoft.com/beta/schemaExtensions
Content-type: application/json

{
    "id":"courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="885ca-180">C#</span><span class="sxs-lookup"><span data-stu-id="885ca-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schemaextension-from-schemaextensions-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="885ca-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="885ca-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schemaextension-from-schemaextensions-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="885ca-182">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="885ca-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schemaextension-from-schemaextensions-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="885ca-183">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="885ca-183">Response 2</span></span>

<span data-ttu-id="885ca-p110">A resposta inclui uma cadeia de caracteres exclusiva na propriedade **id** com base no nome do esquema fornecido na solicitação, junto com o resto da definição de esquema recém-criada. O valor em **id** na resposta se baseia no formato, ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. Observação: O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="885ca-p110">The response includes a unique string in the **id** property that is based on the schema name provided in the request, together with the rest of the newly created schema definition. The value in **id** in the response is based on the format, ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 420

{
    "id": "extk9eruy7c_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "courseId",
            "type": "String"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```


## <a name="see-also"></a><span data-ttu-id="885ca-188">Confira também</span><span class="sxs-lookup"><span data-stu-id="885ca-188">See also</span></span>

- [<span data-ttu-id="885ca-189">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="885ca-189">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="885ca-190">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="885ca-190">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
