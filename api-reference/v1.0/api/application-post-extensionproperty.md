---
title: Criar extensionProperty
description: Crie uma nova extensionProperty.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 7105cce50e231280d88f1cf96289fa7cbc0fca94
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135839"
---
# <a name="create-extensionproperty"></a><span data-ttu-id="286e0-103">Criar extensionProperty</span><span class="sxs-lookup"><span data-stu-id="286e0-103">Create extensionProperty</span></span>

<span data-ttu-id="286e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="286e0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="286e0-105">Crie uma nova [definição extensionProperty.](../resources/extensionproperty.md)</span><span class="sxs-lookup"><span data-stu-id="286e0-105">Create a new [extensionProperty](../resources/extensionproperty.md) definition.</span></span> <span data-ttu-id="286e0-106">Você pode usar essa operação para adicionar um valor de propriedade personalizado ao tipo de objeto de destino definido na **extensionProperty**, usando solicitações padrão de criação e atualização para o objeto de destino.</span><span class="sxs-lookup"><span data-stu-id="286e0-106">You can use this operation to add a custom property value to the targeted object type defined in the **extensionProperty**, using standard creation and update requests to the target object.</span></span>

## <a name="permissions"></a><span data-ttu-id="286e0-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="286e0-107">Permissions</span></span>

<span data-ttu-id="286e0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="286e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="286e0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="286e0-110">Permission type</span></span>      | <span data-ttu-id="286e0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="286e0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="286e0-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="286e0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="286e0-113">Application.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="286e0-113">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="286e0-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="286e0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="286e0-115">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="286e0-115">Application.ReadWrite.All</span></span> |
|<span data-ttu-id="286e0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="286e0-116">Application</span></span> | <span data-ttu-id="286e0-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="286e0-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="286e0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="286e0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/extensionProperties
```

## <a name="request-headers"></a><span data-ttu-id="286e0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="286e0-119">Request headers</span></span>
| <span data-ttu-id="286e0-120">Nome</span><span class="sxs-lookup"><span data-stu-id="286e0-120">Name</span></span>       | <span data-ttu-id="286e0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="286e0-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="286e0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="286e0-122">Authorization</span></span>  | <span data-ttu-id="286e0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="286e0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="286e0-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="286e0-125">Content-Type</span></span> | <span data-ttu-id="286e0-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="286e0-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="286e0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="286e0-128">Request body</span></span>

<span data-ttu-id="286e0-129">No corpo da solicitação, forneça [um objeto extensionProperty](../resources/extensionproperty.md) com as propriedades a seguir.</span><span class="sxs-lookup"><span data-stu-id="286e0-129">In the request body, provide an [extensionProperty](../resources/extensionproperty.md) object with the following properties.</span></span>


| <span data-ttu-id="286e0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="286e0-130">Property</span></span>     | <span data-ttu-id="286e0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="286e0-131">Type</span></span>        | <span data-ttu-id="286e0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="286e0-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="286e0-133">dataType</span><span class="sxs-lookup"><span data-stu-id="286e0-133">dataType</span></span>|<span data-ttu-id="286e0-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="286e0-134">String</span></span>| <span data-ttu-id="286e0-135">Especifica o tipo de dados do valor que a propriedade de extensão pode conter.</span><span class="sxs-lookup"><span data-stu-id="286e0-135">Specifies the data type of the value the extension property can hold.</span></span> <span data-ttu-id="286e0-136">Os valores a seguir são suportados.</span><span class="sxs-lookup"><span data-stu-id="286e0-136">Following values are supported.</span></span> <span data-ttu-id="286e0-137">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="286e0-137">Not nullable.</span></span> <ul><li><span data-ttu-id="286e0-138">`Binary` - Máximo de 256 bytes</span><span class="sxs-lookup"><span data-stu-id="286e0-138">`Binary` - 256 bytes maximum</span></span></li><li>`Boolean`</li><li><span data-ttu-id="286e0-139">`DateTime` - Deve ser especificado no formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="286e0-139">`DateTime` - Must be specified in ISO 8601 format.</span></span> <span data-ttu-id="286e0-140">Serão armazenados no UTC.</span><span class="sxs-lookup"><span data-stu-id="286e0-140">Will be stored in UTC.</span></span></li><li><span data-ttu-id="286e0-141">`Integer` - Valor de 32 bits.</span><span class="sxs-lookup"><span data-stu-id="286e0-141">`Integer` - 32-bit value.</span></span></li><li><span data-ttu-id="286e0-142">`LargeInteger` - Valor de 64 bits.</span><span class="sxs-lookup"><span data-stu-id="286e0-142">`LargeInteger` - 64-bit value.</span></span></li><li><span data-ttu-id="286e0-143">`String` - Máximo de 256 caracteres</span><span class="sxs-lookup"><span data-stu-id="286e0-143">`String` - 256 characters maximum</span></span></li></ul>|
|<span data-ttu-id="286e0-144">nome</span><span class="sxs-lookup"><span data-stu-id="286e0-144">name</span></span>|<span data-ttu-id="286e0-145">String</span><span class="sxs-lookup"><span data-stu-id="286e0-145">String</span></span>| <span data-ttu-id="286e0-146">Nome da propriedade de extensão.</span><span class="sxs-lookup"><span data-stu-id="286e0-146">Name of the extension property.</span></span> <span data-ttu-id="286e0-147">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="286e0-147">Not nullable.</span></span> |
|<span data-ttu-id="286e0-148">targetObjects</span><span class="sxs-lookup"><span data-stu-id="286e0-148">targetObjects</span></span>|<span data-ttu-id="286e0-149">String collection</span><span class="sxs-lookup"><span data-stu-id="286e0-149">String collection</span></span>| <span data-ttu-id="286e0-150">Os valores a seguir são suportados.</span><span class="sxs-lookup"><span data-stu-id="286e0-150">Following values are supported.</span></span> <span data-ttu-id="286e0-151">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="286e0-151">Not nullable.</span></span> <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|


## <a name="response"></a><span data-ttu-id="286e0-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="286e0-152">Response</span></span>

<span data-ttu-id="286e0-153">Se bem-sucedido, este método retorna um código de resposta e um novo objeto `201 Created` [extensionProperty](../resources/extensionproperty.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="286e0-153">If successful, this method returns a `201 Created` response code and a new [extensionProperty](../resources/extensionproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="286e0-154">Exemplos</span><span class="sxs-lookup"><span data-stu-id="286e0-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="286e0-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="286e0-155">Request</span></span>

<span data-ttu-id="286e0-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="286e0-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="286e0-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="286e0-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_extensionproperty_from_application"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/extensionProperties
Content-type: application/json

{
    "name": "extensionName",
    "dataType": "string",
    "targetObjects": [
        "Application"
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="286e0-158">C#</span><span class="sxs-lookup"><span data-stu-id="286e0-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-extensionproperty-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="286e0-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="286e0-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-extensionproperty-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="286e0-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="286e0-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-extensionproperty-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="286e0-161">Java</span><span class="sxs-lookup"><span data-stu-id="286e0-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-extensionproperty-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="286e0-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="286e0-162">Response</span></span>

<span data-ttu-id="286e0-163">Se bem-sucedido, este método retorna o código de resposta e o `201 Created` [objeto extensionProperty](../resources/extensionProperty.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="286e0-163">If successful, this method returns `201 Created` response code and [extensionProperty](../resources/extensionProperty.md) object in the response body.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.extensionProperty"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "a2c459db-f5dc-4328-ae9b-118e88d04d19",
    "deletedDateTime": null,
    "appDisplayName": "Display name",
    "name": "extension_b3efaf8f68a44275abcff28ef86b2ee3_extensionName",
    "dataType": "String",
    "isSyncedFromOnPremises": false,
    "targetObjects": [
        "Application"
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create extensionProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

