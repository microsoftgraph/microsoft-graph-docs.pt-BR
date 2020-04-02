---
title: Criar extensionproperty
description: Crie uma nova extensionproperty.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 53c80299f0cbc85eddf1eab6b1cce1f5b37a290e
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107084"
---
# <a name="create-extensionproperty"></a><span data-ttu-id="87d0e-103">Criar extensionproperty</span><span class="sxs-lookup"><span data-stu-id="87d0e-103">Create extensionProperty</span></span>

<span data-ttu-id="87d0e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87d0e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87d0e-105">Crie uma nova definição de [extensionproperty](../resources/extensionproperty.md) .</span><span class="sxs-lookup"><span data-stu-id="87d0e-105">Create a new [extensionProperty](../resources/extensionproperty.md) definition.</span></span> <span data-ttu-id="87d0e-106">Você pode usar essa operação para adicionar um valor de propriedade personalizada ao tipo de objeto de destino definido na extensãoproperty, usando solicitações de criação e de atualização padrão para o objeto de destino.</span><span class="sxs-lookup"><span data-stu-id="87d0e-106">You can use this operation to add a custom property value to the targeted object type defined in the extensionProperty, using standard creation and update requests to the target object.</span></span>

## <a name="permissions"></a><span data-ttu-id="87d0e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="87d0e-107">Permissions</span></span>

<span data-ttu-id="87d0e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87d0e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87d0e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87d0e-110">Permission type</span></span>      | <span data-ttu-id="87d0e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="87d0e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87d0e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87d0e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="87d0e-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="87d0e-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="87d0e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87d0e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87d0e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87d0e-115">Not supported.</span></span>    |
|<span data-ttu-id="87d0e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87d0e-116">Application</span></span> | <span data-ttu-id="87d0e-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87d0e-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="87d0e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87d0e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/extensionProperties
```

## <a name="request-headers"></a><span data-ttu-id="87d0e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87d0e-119">Request headers</span></span>
| <span data-ttu-id="87d0e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="87d0e-120">Name</span></span>       | <span data-ttu-id="87d0e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="87d0e-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="87d0e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="87d0e-122">Authorization</span></span>  | <span data-ttu-id="87d0e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87d0e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="87d0e-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="87d0e-125">Content-type</span></span> | <span data-ttu-id="87d0e-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87d0e-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87d0e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87d0e-128">Request body</span></span>

<span data-ttu-id="87d0e-129">No corpo da solicitação, forneça um objeto [extensionproperty](../resources/extensionproperty.md) com as propriedades a seguir.</span><span class="sxs-lookup"><span data-stu-id="87d0e-129">In the request body, provide an [extensionProperty](../resources/extensionproperty.md) object with the following properties.</span></span>


| <span data-ttu-id="87d0e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87d0e-130">Property</span></span>     | <span data-ttu-id="87d0e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="87d0e-131">Type</span></span>        | <span data-ttu-id="87d0e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="87d0e-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="87d0e-133">dataType</span><span class="sxs-lookup"><span data-stu-id="87d0e-133">dataType</span></span>|<span data-ttu-id="87d0e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="87d0e-134">String</span></span>| <span data-ttu-id="87d0e-135">Especifica o tipo de dados do valor que a Propriedade Extension pode armazenar.</span><span class="sxs-lookup"><span data-stu-id="87d0e-135">Specifies the data type of the value the extension property can hold.</span></span> <span data-ttu-id="87d0e-136">Os valores a seguir são suportados.</span><span class="sxs-lookup"><span data-stu-id="87d0e-136">Following values are supported.</span></span> <span data-ttu-id="87d0e-137">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="87d0e-137">Not nullable.</span></span> <ul><li><span data-ttu-id="87d0e-138">`Binary`-256 bytes máximo</span><span class="sxs-lookup"><span data-stu-id="87d0e-138">`Binary` - 256 bytes maximum</span></span></li><li>`Boolean`</li><li><span data-ttu-id="87d0e-139">`DateTime`-Deve ser especificado no formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="87d0e-139">`DateTime` - Must be specified in ISO 8601 format.</span></span> <span data-ttu-id="87d0e-140">Serão armazenados no UTC.</span><span class="sxs-lookup"><span data-stu-id="87d0e-140">Will be stored in UTC.</span></span></li><li><span data-ttu-id="87d0e-141">`Integer`-valor de 32-bit.</span><span class="sxs-lookup"><span data-stu-id="87d0e-141">`Integer` - 32-bit value.</span></span></li><li><span data-ttu-id="87d0e-142">`LargeInteger`-valor de 64-bit.</span><span class="sxs-lookup"><span data-stu-id="87d0e-142">`LargeInteger` - 64-bit value.</span></span></li><li><span data-ttu-id="87d0e-143">`String`-256 caracteres no máximo</span><span class="sxs-lookup"><span data-stu-id="87d0e-143">`String` - 256 characters maximum</span></span></li></ul>|
|<span data-ttu-id="87d0e-144">name</span><span class="sxs-lookup"><span data-stu-id="87d0e-144">name</span></span>|<span data-ttu-id="87d0e-145">String</span><span class="sxs-lookup"><span data-stu-id="87d0e-145">String</span></span>| <span data-ttu-id="87d0e-146">Nome da propriedade de extensão.</span><span class="sxs-lookup"><span data-stu-id="87d0e-146">Name of the extension property.</span></span> <span data-ttu-id="87d0e-147">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="87d0e-147">Not nullable.</span></span> |
|<span data-ttu-id="87d0e-148">targetObjects</span><span class="sxs-lookup"><span data-stu-id="87d0e-148">targetObjects</span></span>|<span data-ttu-id="87d0e-149">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="87d0e-149">String collection</span></span>| <span data-ttu-id="87d0e-150">Os valores a seguir são suportados.</span><span class="sxs-lookup"><span data-stu-id="87d0e-150">Following values are supported.</span></span> <span data-ttu-id="87d0e-151">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="87d0e-151">Not nullable.</span></span> <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|


## <a name="response"></a><span data-ttu-id="87d0e-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="87d0e-152">Response</span></span>

<span data-ttu-id="87d0e-153">Se bem-sucedido, este método retorna `201, Created` um código de resposta e um novo objeto [extensionproperty](../resources/extensionproperty.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87d0e-153">If successful, this method returns `201, Created` response code and a new [extensionProperty](../resources/extensionproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="87d0e-154">Exemplos</span><span class="sxs-lookup"><span data-stu-id="87d0e-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="87d0e-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87d0e-155">Request</span></span>

<span data-ttu-id="87d0e-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="87d0e-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="87d0e-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="87d0e-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_extensionproperty_from_application"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/extensionProperties
Content-type: application/json

{
    "name": "extensionName",
    "dataType": "string",
    "targetObjects": [
        "Application"
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="87d0e-158">C#</span><span class="sxs-lookup"><span data-stu-id="87d0e-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-extensionproperty-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="87d0e-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87d0e-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-extensionproperty-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="87d0e-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87d0e-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-extensionproperty-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="87d0e-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="87d0e-161">Response</span></span>

<span data-ttu-id="87d0e-162">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [extensionproperty](../resources/extensionProperty.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87d0e-162">If successful, this method returns a `201 Created` response code and an [extensionProperty](../resources/extensionProperty.md) object in the response body.</span></span>

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
