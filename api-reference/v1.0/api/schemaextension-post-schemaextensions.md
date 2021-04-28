---
title: Criar schemaExtension
description: Criar uma nova definição schemaExtension para estender um tipo de recurso de suporte.
localization_priority: Priority
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: a498b23cc29c806f24cd620110ce731598ba2582
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054473"
---
# <a name="create-schemaextension"></a><span data-ttu-id="89bf7-103">Criar schemaExtension</span><span class="sxs-lookup"><span data-stu-id="89bf7-103">Create schemaExtension</span></span>

<span data-ttu-id="89bf7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89bf7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="89bf7-105">Criar uma nova definição [schemaExtension](../resources/schemaextension.md) para estender um [tipo de recurso de suporte](/graph/extensibility-overview#supported-resources).</span><span class="sxs-lookup"><span data-stu-id="89bf7-105">Create a new [schemaExtension](../resources/schemaextension.md) definition to extend a [supporting resource type](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="89bf7-p101">As extensões de esquema permitem que você adicione dados personalizados fortemente tipados a um recurso. O aplicativo que cria uma extensão de esquema é o aplicativo proprietário. Dependendo do [estado](/graph/extensibility-overview#schema-extensions-lifecycle) da extensão, o aplicativo proprietário, e apenas o aplicativo proprietário, poderá atualizar ou excluir a extensão.</span><span class="sxs-lookup"><span data-stu-id="89bf7-p101">Schema extensions let you add strongly-typed custom data to a resource. The app that creates a schema extension is the owner app. Depending on the [state](/graph/extensibility-overview#schema-extensions-lifecycle) of the extension, the owner app, and only the owner app, may update or delete the extension.</span></span> 

<span data-ttu-id="89bf7-109">Veja exemplos de como [definir uma extensão de esquema que descreve um curso de treinamento](/graph/extensibility-schema-groups#2-register-a-schema-extension-definition-that-describes-a-training-course), usar a definição de extensão do esquema para [criar um novo grupo com dados do curso de treinamento](/graph/extensibility-schema-groups#3-create-a-new-group-with-extended-data) e [adicionar dados do curso de treinamento a um grupo existente](/graph/extensibility-schema-groups#4-add-update-or-remove-custom-data-in-an-existing-group).</span><span class="sxs-lookup"><span data-stu-id="89bf7-109">See examples of how to [define a schema extension that describes a training course](/graph/extensibility-schema-groups#2-register-a-schema-extension-definition-that-describes-a-training-course), use the schema extension definition to [create a new group with training course data](/graph/extensibility-schema-groups#3-create-a-new-group-with-extended-data), and [add training course data to an existing group](/graph/extensibility-schema-groups#4-add-update-or-remove-custom-data-in-an-existing-group).</span></span>

## <a name="permissions"></a><span data-ttu-id="89bf7-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="89bf7-110">Permissions</span></span>
<span data-ttu-id="89bf7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89bf7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="89bf7-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89bf7-113">Permission type</span></span>      | <span data-ttu-id="89bf7-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="89bf7-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89bf7-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89bf7-115">Delegated (work or school account)</span></span> | <span data-ttu-id="89bf7-116">Application.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="89bf7-116">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="89bf7-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89bf7-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89bf7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89bf7-118">Not supported.</span></span>    |
|<span data-ttu-id="89bf7-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89bf7-119">Application</span></span> | <span data-ttu-id="89bf7-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89bf7-120">Not supported.</span></span> |

> [!NOTE]
> <span data-ttu-id="89bf7-121">Além disso, para o fluxo delegado, o usuário conectado deve ser o proprietário do aplicativo de chamada OU o proprietário do (aplicativo com a)`appId` usada para definir a propriedade **proprietário**.</span><span class="sxs-lookup"><span data-stu-id="89bf7-121">Additionally for the delegated flow, the signed-in user must be the owner of the calling application OR the owner of the (application with the) `appId` used to set the **owner** property.</span></span>

## <a name="http-request"></a><span data-ttu-id="89bf7-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89bf7-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /schemaExtensions
```

## <a name="request-headers"></a><span data-ttu-id="89bf7-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89bf7-123">Request headers</span></span>
| <span data-ttu-id="89bf7-124">Nome</span><span class="sxs-lookup"><span data-stu-id="89bf7-124">Name</span></span>       | <span data-ttu-id="89bf7-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="89bf7-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="89bf7-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="89bf7-126">Authorization</span></span>  | <span data-ttu-id="89bf7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89bf7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="89bf7-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="89bf7-129">Content-Type</span></span>  | <span data-ttu-id="89bf7-130">application/json</span><span class="sxs-lookup"><span data-stu-id="89bf7-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="89bf7-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89bf7-131">Request body</span></span>
<span data-ttu-id="89bf7-132">No corpo da solicitação, forneça uma representação JSON de um objeto [schemaExtension](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="89bf7-132">In the request body, supply a JSON representation of [schemaExtension](../resources/schemaextension.md) object.</span></span>

<span data-ttu-id="89bf7-133">A tabela a seguir mostra as propriedades que são necessárias ao criar uma extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="89bf7-133">The following table shows the properties that are required when you create a schema extension.</span></span>

| <span data-ttu-id="89bf7-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="89bf7-134">Parameter</span></span> | <span data-ttu-id="89bf7-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="89bf7-135">Type</span></span> | <span data-ttu-id="89bf7-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="89bf7-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89bf7-137">description</span><span class="sxs-lookup"><span data-stu-id="89bf7-137">description</span></span>|<span data-ttu-id="89bf7-138">String</span><span class="sxs-lookup"><span data-stu-id="89bf7-138">String</span></span>|<span data-ttu-id="89bf7-139">Descrição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="89bf7-139">Description for the schema extension.</span></span>|
|<span data-ttu-id="89bf7-140">id</span><span class="sxs-lookup"><span data-stu-id="89bf7-140">id</span></span>|<span data-ttu-id="89bf7-141">String</span><span class="sxs-lookup"><span data-stu-id="89bf7-141">String</span></span>|<span data-ttu-id="89bf7-142">O identificador exclusivo da definição de extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="89bf7-142">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="89bf7-143">Você pode atribuir um valor em uma destas duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="89bf7-143">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="89bf7-144">Concatenar o nome de um de seus domínios verificados com um nome da extensão do esquema para formar uma cadeia de caracteres exclusiva neste formato, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span><span class="sxs-lookup"><span data-stu-id="89bf7-144">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span></span> <span data-ttu-id="89bf7-145">Como exemplo, `contoso_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="89bf7-145">As an example, `contoso_mySchema`.</span></span> <span data-ttu-id="89bf7-146">OBSERVAÇÃO: Apenas domínios verificados sob os seguintes domínios de nível superior têm suporte: `.com`,`.net`, `.gov`, `.edu` ou `.org`.</span><span class="sxs-lookup"><span data-stu-id="89bf7-146">NOTE: Only verified domains under the following top-level domains are supported: `.com`,`.net`, `.gov`, `.edu` or `.org`.</span></span> </li><li><span data-ttu-id="89bf7-p105">Forneça um nome de esquema e permita que o Microsoft Graph use esse nome de esquema para completar a atribuição de **id** neste formato: ext\{_&#65279;8-caracteres-alfanuméricos-aleatórios_\}\_\{_&#65279;nome-do-esquema_\}. Um exemplo seria `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="89bf7-p105">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="89bf7-149">Esta propriedade não pode ser alterada após a criação.</span><span class="sxs-lookup"><span data-stu-id="89bf7-149">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="89bf7-150">owner</span><span class="sxs-lookup"><span data-stu-id="89bf7-150">owner</span></span>|<span data-ttu-id="89bf7-151">String</span><span class="sxs-lookup"><span data-stu-id="89bf7-151">String</span></span>|<span data-ttu-id="89bf7-152">(Opcional) O `appId` do aplicativo que é o proprietário da extensão do esquema.</span><span class="sxs-lookup"><span data-stu-id="89bf7-152">(Optional) The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="89bf7-153">Por padrão, a `appId` dos aplicativos de chamada será definida como proprietário.</span><span class="sxs-lookup"><span data-stu-id="89bf7-153">By default, the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="89bf7-154">No entanto, a propriedade pode ser fornecida na criação, para definir a appId do proprietário como algo diferente do aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="89bf7-154">However, the property may be supplied on creation, to set the owner appId to something different from the calling app.</span></span> <span data-ttu-id="89bf7-155">Em todos os casos, no fluxo delegado, o usuário conectado **deve** ser o proprietário do aplicativo definido como o proprietário da extensão do esquema.</span><span class="sxs-lookup"><span data-stu-id="89bf7-155">In all cases, in the delegated flow, the signed-in user **must** be the owner of the application being set as the schema extension's owner.</span></span> <span data-ttu-id="89bf7-156">Assim, por exemplo, se você criar uma nova definição da extensão de esquema usando o Graph Explorer, você **deverá** fornecer a propriedade do proprietário, para uma appId que você possui.</span><span class="sxs-lookup"><span data-stu-id="89bf7-156">So, for example, if creating a new schema extension definition using Graph Explorer, you **must** supply the owner property, for an appId you own.</span></span> <span data-ttu-id="89bf7-157">Uma vez definida, essa propriedade é somente leitura e não pode ser alterada.</span><span class="sxs-lookup"><span data-stu-id="89bf7-157">Once set, this property is read-only and cannot be changed.</span></span>|
|<span data-ttu-id="89bf7-158">properties</span><span class="sxs-lookup"><span data-stu-id="89bf7-158">properties</span></span>|<span data-ttu-id="89bf7-159">Coleção [extensionSchemaProperty](../resources/extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="89bf7-159">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="89bf7-160">A coleção de tipos e nomes de propriedades que compõem a definição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="89bf7-160">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="89bf7-161">targetTypes</span><span class="sxs-lookup"><span data-stu-id="89bf7-161">targetTypes</span></span>|<span data-ttu-id="89bf7-162">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="89bf7-162">String collection</span></span>|<span data-ttu-id="89bf7-163">O conjunto de tipos de recursos do Microsoft Graph (com suporte a extensões do esquema) ao qual esta extensão de esquema pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="89bf7-163">Set of Microsoft Graph resource types (that support schema extensions) that this schema extension definition can be applied to.</span></span>|

## <a name="response"></a><span data-ttu-id="89bf7-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="89bf7-164">Response</span></span>

<span data-ttu-id="89bf7-165">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [schemaExtension](../resources/schemaextension.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89bf7-165">If successful, this method returns `201 Created` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89bf7-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89bf7-166">Example</span></span>

### <a name="example-1-creating-a-schema-extension-using-a-verified-domain"></a><span data-ttu-id="89bf7-167">Exemplo 1: Criar uma extensão de esquema usando um domínio verificado</span><span class="sxs-lookup"><span data-stu-id="89bf7-167">Example 1: Creating a schema extension using a verified domain</span></span>

#### <a name="request"></a><span data-ttu-id="89bf7-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89bf7-168">Request</span></span>

<span data-ttu-id="89bf7-169">Este exemplo mostra como usar um nome de domínio verificado, `graphlearn` e um nome de esquema, `courses`, para formar uma cadeia de caracteres exclusiva para a propriedade **id** da definição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="89bf7-169">This example shows using a verified domain name, `graphlearn`, and a schema name, `courses`, to form a unique string for the **id** property of the schema extension definition.</span></span> <span data-ttu-id="89bf7-170">A cadeia de caracteres exclusiva é baseada neste formato,\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span><span class="sxs-lookup"><span data-stu-id="89bf7-170">The unique string is based on this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span></span>

# <a name="http"></a>[<span data-ttu-id="89bf7-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="89bf7-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_1"
}-->
```http
POST https://graph.microsoft.com/v1.0/schemaExtensions
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
# <a name="c"></a>[<span data-ttu-id="89bf7-172">C#</span><span class="sxs-lookup"><span data-stu-id="89bf7-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schemaextension-from-schemaextensions-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89bf7-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89bf7-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schemaextension-from-schemaextensions-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89bf7-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89bf7-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schemaextension-from-schemaextensions-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89bf7-175">Java</span><span class="sxs-lookup"><span data-stu-id="89bf7-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-schemaextension-from-schemaextensions-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="89bf7-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="89bf7-176">Response</span></span>

<span data-ttu-id="89bf7-177">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89bf7-177">Here is an example of the response.</span></span> <span data-ttu-id="89bf7-178">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="89bf7-178">Note: The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-creating-a-schema-extension-using-just-a-name"></a><span data-ttu-id="89bf7-179">Exemplo 2: Criar uma extensão de esquema usando apenas um nome</span><span class="sxs-lookup"><span data-stu-id="89bf7-179">Example 2: Creating a schema extension using just a name</span></span>

#### <a name="request"></a><span data-ttu-id="89bf7-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89bf7-180">Request</span></span>

<span data-ttu-id="89bf7-181">Este exemplo mostra a especificação de apenas um nome de esquema, `courses`, na propriedade **id** da solicitação, juntamente com a representação JSON do restante das propriedades no objeto [schemaExtension](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="89bf7-181">This example shows specifying just a schema name, `courses`, in the **id** property in the request, together with the JSON representation of the rest of the properties in the [schemaExtension](../resources/schemaextension.md) object.</span></span> <span data-ttu-id="89bf7-182">O Microsoft Graph atribuirá e retornará um valor de cadeia de caracteres exclusivo na resposta.</span><span class="sxs-lookup"><span data-stu-id="89bf7-182">Microsoft Graph will assign and return a unique string value in the response.</span></span>


# <a name="http"></a>[<span data-ttu-id="89bf7-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="89bf7-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/schemaExtensions
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
# <a name="c"></a>[<span data-ttu-id="89bf7-184">C#</span><span class="sxs-lookup"><span data-stu-id="89bf7-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schemaextension-from-schemaextensions-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89bf7-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89bf7-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schemaextension-from-schemaextensions-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89bf7-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89bf7-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schemaextension-from-schemaextensions-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89bf7-187">Java</span><span class="sxs-lookup"><span data-stu-id="89bf7-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-schemaextension-from-schemaextensions-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="89bf7-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="89bf7-188">Response</span></span>

<span data-ttu-id="89bf7-189">A resposta inclui uma cadeia de caracteres exclusiva na propriedade **id** com base no nome do esquema fornecido na solicitação, junto com o resto da definição de esquema recém-criada.</span><span class="sxs-lookup"><span data-stu-id="89bf7-189">The response includes a unique string in the **id** property that is based on the schema name provided in the request, together with the rest of the newly created schema definition.</span></span> <span data-ttu-id="89bf7-190">O valor em **id** na resposta se baseia no formato, ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}.</span><span class="sxs-lookup"><span data-stu-id="89bf7-190">The value in **id** in the response is based on the format, ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}.</span></span> <span data-ttu-id="89bf7-191">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="89bf7-191">Note: The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-3-creating-a-schema-extension-setting-the-owner"></a><span data-ttu-id="89bf7-192">Exemplo 3: Criação de uma extensão de esquema definindo o proprietário</span><span class="sxs-lookup"><span data-stu-id="89bf7-192">Example 3: Creating a schema extension setting the owner</span></span>

#### <a name="request"></a><span data-ttu-id="89bf7-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89bf7-193">Request</span></span>

<span data-ttu-id="89bf7-194">Este exemplo mostra como criar uma extensão de esquema configurando o **proprietário**.</span><span class="sxs-lookup"><span data-stu-id="89bf7-194">This example shows how to create a schema extension setting the **owner**.</span></span>  <span data-ttu-id="89bf7-195">Neste cenário, o usuário do aplicativo pode não ser o proprietário do aplicativo (por exemplo, se você estiver usando o Microsoft Graph Explorer).</span><span class="sxs-lookup"><span data-stu-id="89bf7-195">In this scenario, the user of the application might not be the owner of the application (for example if you are using Microsoft Graph Explorer).</span></span>  <span data-ttu-id="89bf7-196">Neste caso, você deve definir a propriedade do **proprietário** como a **appId** de um aplicativo que você possui, caso contrário, você não terá autorização para criar uma extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="89bf7-196">In this case you should set the **owner** property to the **appId** of an application you own, otherwise you won't be authorized to create a schema extension.</span></span> <span data-ttu-id="89bf7-197">Defina a propriedade **proprietário** na solicitação, juntamente com a representação JSON do restante das propriedades no objeto [schemaExtension](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="89bf7-197">Set the **owner** property in the request, together with the JSON representation of the rest of the properties in the [schemaExtension](../resources/schemaextension.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="89bf7-198">HTTP</span><span class="sxs-lookup"><span data-stu-id="89bf7-198">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_3"
}-->

```http
POST https://graph.microsoft.com/v1.0/schemaExtensions
Content-type: application/json

{
    "id":"courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "owner": "50897f70-a455-4adf-87bc-4cf17091d5ac",
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
# <a name="c"></a>[<span data-ttu-id="89bf7-199">C#</span><span class="sxs-lookup"><span data-stu-id="89bf7-199">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schemaextension-from-schemaextensions-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89bf7-200">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89bf7-200">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schemaextension-from-schemaextensions-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89bf7-201">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89bf7-201">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schemaextension-from-schemaextensions-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89bf7-202">Java</span><span class="sxs-lookup"><span data-stu-id="89bf7-202">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-schemaextension-from-schemaextensions-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="89bf7-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="89bf7-203">Response</span></span>

<span data-ttu-id="89bf7-204">A resposta inclui o **proprietário** definido como o valor fornecido na solicitação.</span><span class="sxs-lookup"><span data-stu-id="89bf7-204">The response includes the **owner** set to the supplied value in the request.</span></span> <span data-ttu-id="89bf7-205">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="89bf7-205">Note: The response object shown here might be shortened for readability.</span></span>
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
    "owner": "50897f70-a455-4adf-87bc-4cf17091d5ac",
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

## <a name="see-also"></a><span data-ttu-id="89bf7-206">Confira também</span><span class="sxs-lookup"><span data-stu-id="89bf7-206">See also</span></span>

- [<span data-ttu-id="89bf7-207">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="89bf7-207">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="89bf7-208">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="89bf7-208">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

