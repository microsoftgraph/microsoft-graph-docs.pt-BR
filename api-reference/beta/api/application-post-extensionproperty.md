---
title: Criar extensionproperty
description: Crie uma nova extensionproperty.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5194281dee925171f8834b7e8dde76cf60b17244
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006428"
---
# <a name="create-extensionproperty"></a><span data-ttu-id="7259f-103">Criar extensionproperty</span><span class="sxs-lookup"><span data-stu-id="7259f-103">Create extensionProperty</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7259f-104">Crie uma nova definição de [extensionproperty](../resources/extensionproperty.md) .</span><span class="sxs-lookup"><span data-stu-id="7259f-104">Create a new [extensionProperty](../resources/extensionproperty.md) definition.</span></span> <span data-ttu-id="7259f-105">Você pode usar essa operação para adicionar um valor de propriedade personalizada ao tipo de objeto de destino definido na extensãoproperty, usando solicitações de criação e de atualização padrão para o objeto de destino.</span><span class="sxs-lookup"><span data-stu-id="7259f-105">You can use this operation to add a custom property value to the targeted object type defined in the extensionProperty, using standard creation and update requests to the target object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7259f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7259f-106">Permissions</span></span>

<span data-ttu-id="7259f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7259f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7259f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7259f-109">Permission type</span></span>      | <span data-ttu-id="7259f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7259f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7259f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7259f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7259f-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7259f-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7259f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7259f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7259f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7259f-114">Not supported.</span></span>    |
|<span data-ttu-id="7259f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7259f-115">Application</span></span> | <span data-ttu-id="7259f-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7259f-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7259f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7259f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/extensionProperties
```

## <a name="request-headers"></a><span data-ttu-id="7259f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7259f-118">Request headers</span></span>
| <span data-ttu-id="7259f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7259f-119">Name</span></span>       | <span data-ttu-id="7259f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7259f-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="7259f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7259f-121">Authorization</span></span>  | <span data-ttu-id="7259f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7259f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7259f-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="7259f-124">Content-type</span></span> | <span data-ttu-id="7259f-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7259f-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7259f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7259f-127">Request body</span></span>

<span data-ttu-id="7259f-128">No corpo da solicitação, forneça um objeto [extensionproperty](../resources/extensionproperty.md) com as propriedades a seguir.</span><span class="sxs-lookup"><span data-stu-id="7259f-128">In the request body, provide an [extensionProperty](../resources/extensionproperty.md) object with the following properties.</span></span>


| <span data-ttu-id="7259f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7259f-129">Property</span></span>     | <span data-ttu-id="7259f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7259f-130">Type</span></span>        | <span data-ttu-id="7259f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7259f-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7259f-132">dataType</span><span class="sxs-lookup"><span data-stu-id="7259f-132">dataType</span></span>|<span data-ttu-id="7259f-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7259f-133">String</span></span>| <span data-ttu-id="7259f-134">Especifica o tipo de dados do valor que a Propriedade Extension pode armazenar.</span><span class="sxs-lookup"><span data-stu-id="7259f-134">Specifies the data type of the value the extension property can hold.</span></span> <span data-ttu-id="7259f-135">Os valores a seguir são suportados.</span><span class="sxs-lookup"><span data-stu-id="7259f-135">Following values are supported.</span></span> <span data-ttu-id="7259f-136">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="7259f-136">Not nullable.</span></span> <ul><li><span data-ttu-id="7259f-137">`Binary`-256 bytes máximo</span><span class="sxs-lookup"><span data-stu-id="7259f-137">`Binary` - 256 bytes maximum</span></span></li><li>`Boolean`</li><li><span data-ttu-id="7259f-138">`DateTime`-Deve ser especificado no formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="7259f-138">`DateTime` - Must be specified in ISO 8601 format.</span></span> <span data-ttu-id="7259f-139">Serão armazenados no UTC.</span><span class="sxs-lookup"><span data-stu-id="7259f-139">Will be stored in UTC.</span></span></li><li><span data-ttu-id="7259f-140">`Integer`-valor de 32-bit.</span><span class="sxs-lookup"><span data-stu-id="7259f-140">`Integer` - 32-bit value.</span></span></li><li><span data-ttu-id="7259f-141">`LargeInteger`-valor de 64-bit.</span><span class="sxs-lookup"><span data-stu-id="7259f-141">`LargeInteger` - 64-bit value.</span></span></li><li><span data-ttu-id="7259f-142">`String`-256 caracteres no máximo</span><span class="sxs-lookup"><span data-stu-id="7259f-142">`String` - 256 characters maximum</span></span></li></ul>|
|<span data-ttu-id="7259f-143">nome</span><span class="sxs-lookup"><span data-stu-id="7259f-143">name</span></span>|<span data-ttu-id="7259f-144">String</span><span class="sxs-lookup"><span data-stu-id="7259f-144">String</span></span>| <span data-ttu-id="7259f-145">Nome da propriedade de extensão.</span><span class="sxs-lookup"><span data-stu-id="7259f-145">Name of the extension property.</span></span> <span data-ttu-id="7259f-146">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="7259f-146">Not nullable.</span></span> |
|<span data-ttu-id="7259f-147">targetObjects</span><span class="sxs-lookup"><span data-stu-id="7259f-147">targetObjects</span></span>|<span data-ttu-id="7259f-148">String collection</span><span class="sxs-lookup"><span data-stu-id="7259f-148">String collection</span></span>| <span data-ttu-id="7259f-149">Os valores a seguir são suportados.</span><span class="sxs-lookup"><span data-stu-id="7259f-149">Following values are supported.</span></span> <span data-ttu-id="7259f-150">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="7259f-150">Not nullable.</span></span> <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|


## <a name="response"></a><span data-ttu-id="7259f-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="7259f-151">Response</span></span>

<span data-ttu-id="7259f-152">Se bem-sucedido, este método retorna `201, Created` um código de resposta e um novo objeto [extensionproperty](../resources/extensionproperty.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7259f-152">If successful, this method returns `201, Created` response code and a new [extensionProperty](../resources/extensionproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7259f-153">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7259f-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7259f-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7259f-154">Request</span></span>

<span data-ttu-id="7259f-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7259f-155">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7259f-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="7259f-156">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="7259f-157">C#</span><span class="sxs-lookup"><span data-stu-id="7259f-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-extensionproperty-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7259f-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7259f-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-extensionproperty-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7259f-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7259f-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-extensionproperty-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7259f-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="7259f-160">Response</span></span>

<span data-ttu-id="7259f-161">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [extensionproperty](../resources/extensionProperty.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7259f-161">If successful, this method returns a `201 Created` response code and an [extensionProperty](../resources/extensionProperty.md) object in the response body.</span></span>

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