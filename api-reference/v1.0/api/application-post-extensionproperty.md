---
title: Criar extensionproperty
description: Crie uma nova extensionproperty.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bb6ac47f3b33bb963181e71d7f5d7c83e2bf13b0
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939688"
---
# <a name="create-extensionproperty"></a><span data-ttu-id="2014c-103">Criar extensionproperty</span><span class="sxs-lookup"><span data-stu-id="2014c-103">Create extensionProperty</span></span>

<span data-ttu-id="2014c-104">Crie uma nova definição de [extensionproperty](../resources/extensionproperty.md) .</span><span class="sxs-lookup"><span data-stu-id="2014c-104">Create a new [extensionProperty](../resources/extensionproperty.md) definition.</span></span> <span data-ttu-id="2014c-105">Você pode usar essa operação para adicionar um valor de propriedade personalizada ao tipo de objeto de destino definido na **extensãoproperty**, usando solicitações de criação e de atualização padrão para o objeto de destino.</span><span class="sxs-lookup"><span data-stu-id="2014c-105">You can use this operation to add a custom property value to the targeted object type defined in the **extensionProperty**, using standard creation and update requests to the target object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2014c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2014c-106">Permissions</span></span>

<span data-ttu-id="2014c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2014c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2014c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2014c-109">Permission type</span></span>      | <span data-ttu-id="2014c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2014c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2014c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2014c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2014c-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2014c-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2014c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2014c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2014c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2014c-114">Not supported.</span></span>    |
|<span data-ttu-id="2014c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2014c-115">Application</span></span> | <span data-ttu-id="2014c-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2014c-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2014c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2014c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/extensionProperties
```

## <a name="request-headers"></a><span data-ttu-id="2014c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2014c-118">Request headers</span></span>
| <span data-ttu-id="2014c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2014c-119">Name</span></span>       | <span data-ttu-id="2014c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2014c-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="2014c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2014c-121">Authorization</span></span>  | <span data-ttu-id="2014c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2014c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2014c-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="2014c-124">Content-type</span></span> | <span data-ttu-id="2014c-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2014c-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2014c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2014c-127">Request body</span></span>

<span data-ttu-id="2014c-128">No corpo da solicitação, forneça um objeto [extensionproperty](../resources/extensionproperty.md) com as propriedades a seguir.</span><span class="sxs-lookup"><span data-stu-id="2014c-128">In the request body, provide an [extensionProperty](../resources/extensionproperty.md) object with the following properties.</span></span>


| <span data-ttu-id="2014c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2014c-129">Property</span></span>     | <span data-ttu-id="2014c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2014c-130">Type</span></span>        | <span data-ttu-id="2014c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2014c-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2014c-132">dataType</span><span class="sxs-lookup"><span data-stu-id="2014c-132">dataType</span></span>|<span data-ttu-id="2014c-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2014c-133">String</span></span>| <span data-ttu-id="2014c-134">Especifica o tipo de dados do valor que a Propriedade Extension pode armazenar.</span><span class="sxs-lookup"><span data-stu-id="2014c-134">Specifies the data type of the value the extension property can hold.</span></span> <span data-ttu-id="2014c-135">Os valores a seguir são suportados.</span><span class="sxs-lookup"><span data-stu-id="2014c-135">Following values are supported.</span></span> <span data-ttu-id="2014c-136">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="2014c-136">Not nullable.</span></span> <ul><li><span data-ttu-id="2014c-137">`Binary`-256 bytes máximo</span><span class="sxs-lookup"><span data-stu-id="2014c-137">`Binary` - 256 bytes maximum</span></span></li><li>`Boolean`</li><li><span data-ttu-id="2014c-138">`DateTime`-Deve ser especificado no formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="2014c-138">`DateTime` - Must be specified in ISO 8601 format.</span></span> <span data-ttu-id="2014c-139">Serão armazenados no UTC.</span><span class="sxs-lookup"><span data-stu-id="2014c-139">Will be stored in UTC.</span></span></li><li><span data-ttu-id="2014c-140">`Integer`-valor de 32-bit.</span><span class="sxs-lookup"><span data-stu-id="2014c-140">`Integer` - 32-bit value.</span></span></li><li><span data-ttu-id="2014c-141">`LargeInteger`-valor de 64-bit.</span><span class="sxs-lookup"><span data-stu-id="2014c-141">`LargeInteger` - 64-bit value.</span></span></li><li><span data-ttu-id="2014c-142">`String`-256 caracteres no máximo</span><span class="sxs-lookup"><span data-stu-id="2014c-142">`String` - 256 characters maximum</span></span></li></ul>|
|<span data-ttu-id="2014c-143">name</span><span class="sxs-lookup"><span data-stu-id="2014c-143">name</span></span>|<span data-ttu-id="2014c-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2014c-144">String</span></span>| <span data-ttu-id="2014c-145">Nome da propriedade de extensão.</span><span class="sxs-lookup"><span data-stu-id="2014c-145">Name of the extension property.</span></span> <span data-ttu-id="2014c-146">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="2014c-146">Not nullable.</span></span> |
|<span data-ttu-id="2014c-147">targetObjects</span><span class="sxs-lookup"><span data-stu-id="2014c-147">targetObjects</span></span>|<span data-ttu-id="2014c-148">String collection</span><span class="sxs-lookup"><span data-stu-id="2014c-148">String collection</span></span>| <span data-ttu-id="2014c-149">Os valores a seguir são suportados.</span><span class="sxs-lookup"><span data-stu-id="2014c-149">Following values are supported.</span></span> <span data-ttu-id="2014c-150">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="2014c-150">Not nullable.</span></span> <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|


## <a name="response"></a><span data-ttu-id="2014c-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="2014c-151">Response</span></span>

<span data-ttu-id="2014c-152">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [extensionproperty](../resources/extensionproperty.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2014c-152">If successful, this method returns a `201 Created` response code and a new [extensionProperty](../resources/extensionproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2014c-153">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2014c-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2014c-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2014c-154">Request</span></span>

<span data-ttu-id="2014c-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2014c-155">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2014c-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="2014c-156">Response</span></span>

<span data-ttu-id="2014c-157">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [extensionproperty](../resources/extensionProperty.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2014c-157">If successful, this method returns `201 Created` response code and [extensionProperty](../resources/extensionProperty.md) object in the response body.</span></span>

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
