---
title: Tipo de recurso extensionProperty
description: Representa uma extensão de diretório
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 33603d0d16cc44fd2f07177da4c6c6bb4208b082
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941782"
---
# <a name="extensionproperty-resource-type"></a><span data-ttu-id="9e5e1-103">Tipo de recurso extensionProperty</span><span class="sxs-lookup"><span data-stu-id="9e5e1-103">extensionProperty resource type</span></span>

<span data-ttu-id="9e5e1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e5e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e5e1-105">Representa uma extensão de diretório que pode ser usada para adicionar uma propriedade personalizada a objetos de diretório sem exigir um armazenamento de dados externo.</span><span class="sxs-lookup"><span data-stu-id="9e5e1-105">Represents a directory extension that can be used to add a custom property to directory objects without requiring an external data store.</span></span> <span data-ttu-id="9e5e1-106">Por exemplo, se uma organização tiver um aplicativo LOB (linha de negócios) que exija uma ID do Skype para cada usuário no diretório, o Microsoft Graph poderá ser usado para registrar uma nova propriedade chamada skypeId no objeto User do diretório e, em seguida, gravar um valor na nova propriedade para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="9e5e1-106">For example, if an organization has a line of business (LOB) application that requires a Skype ID for each user in the directory, Microsoft Graph can be used to register a new property named skypeId on the directory’s User object, and then write a value to the new property for a specific user.</span></span>

<span data-ttu-id="9e5e1-107">Extensões podem ser adicionadas ao [usuário,](user.md) [grupo,](group.md) [organização,](organization.md) [dispositivo,](device.md) [recursos de](application.md) aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e5e1-107">Extensions can be added to [user](user.md), [group](group.md), [organization](organization.md), [device](device.md), [application](application.md) resources.</span></span> <span data-ttu-id="9e5e1-108">Somente 100 valores de extensão, em todos *os* tipos e todos os aplicativos, podem ser gravados em qualquer único recurso do Azure AD. </span><span class="sxs-lookup"><span data-stu-id="9e5e1-108">Only 100 extension values, across *all* types and *all* applications, can be written to any single Azure AD resource.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9e5e1-109">As extensões de esquema do Azure AD descritas aqui estão disponíveis no Microsoft Graph apenas por motivos de compatibilidade com compatibilidade com vertidas.</span><span class="sxs-lookup"><span data-stu-id="9e5e1-109">Azure AD schema extensions described here are available in Microsoft Graph for backwards compatibility reasons only.</span></span>
> <span data-ttu-id="9e5e1-110">Ele permite que você use o Microsoft Graph para continuar a gerenciar propriedades de extensão adicionadas por meio do Azure AD Graph ou [do Azure AD Connect](/azure/active-directory/hybrid/whatis-azure-ad-connect).</span><span class="sxs-lookup"><span data-stu-id="9e5e1-110">It allows you to use Microsoft Graph to continue to manage extension properties added through Azure AD Graph or [Azure AD Connect](/azure/active-directory/hybrid/whatis-azure-ad-connect).</span></span>
> <span data-ttu-id="9e5e1-111">Para novas extensões personalizadas, recomendamos que você use extensões de esquema do Microsoft Graph para adicionar [dados personalizados aos recursos](/graph/extensibility-overview).</span><span class="sxs-lookup"><span data-stu-id="9e5e1-111">For new custom extensions, we recommend that you use Microsoft Graph schema extensions for [adding custom data to resources](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="9e5e1-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="9e5e1-112">Methods</span></span>

| <span data-ttu-id="9e5e1-113">Método</span><span class="sxs-lookup"><span data-stu-id="9e5e1-113">Method</span></span>       | <span data-ttu-id="9e5e1-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9e5e1-114">Return Type</span></span> | <span data-ttu-id="9e5e1-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e5e1-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9e5e1-116">Listar extensões</span><span class="sxs-lookup"><span data-stu-id="9e5e1-116">List extensions</span></span>](../api/application-list-extensionproperty.md) | <span data-ttu-id="9e5e1-117">Coleção [extensionProperty](extensionProperty.md)</span><span class="sxs-lookup"><span data-stu-id="9e5e1-117">[extensionProperty](extensionProperty.md) collection</span></span> | <span data-ttu-id="9e5e1-118">Listar propriedades de extensão em um objeto de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e5e1-118">List extension properties on an application object.</span></span> |
| [<span data-ttu-id="9e5e1-119">Criar extensão</span><span class="sxs-lookup"><span data-stu-id="9e5e1-119">Create extension</span></span>](../api/application-post-extensionproperty.md) | [<span data-ttu-id="9e5e1-120">extensionProperty</span><span class="sxs-lookup"><span data-stu-id="9e5e1-120">extensionProperty</span></span>](extensionProperty.md) | <span data-ttu-id="9e5e1-121">Criar uma propriedade de extensão em um objeto de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e5e1-121">Create an extension property on an application object.</span></span> |
| [<span data-ttu-id="9e5e1-122">Excluir extensão</span><span class="sxs-lookup"><span data-stu-id="9e5e1-122">Delete extension</span></span>](../api/application-delete-extensionproperty.md) | <span data-ttu-id="9e5e1-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9e5e1-123">None</span></span> | <span data-ttu-id="9e5e1-124">Excluir uma propriedade de extensão de um objeto de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e5e1-124">Delete an extension property from an application object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9e5e1-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9e5e1-125">Properties</span></span>

| <span data-ttu-id="9e5e1-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e5e1-126">Property</span></span>     | <span data-ttu-id="9e5e1-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e5e1-127">Type</span></span>        | <span data-ttu-id="9e5e1-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e5e1-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9e5e1-129">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="9e5e1-129">appDisplayName</span></span>|<span data-ttu-id="9e5e1-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e5e1-130">String</span></span>| <span data-ttu-id="9e5e1-131">Nome de exibição do objeto application no qual essa propriedade de extensão é definida.</span><span class="sxs-lookup"><span data-stu-id="9e5e1-131">Display name of the application object on which this extension property is defined.</span></span> <span data-ttu-id="9e5e1-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9e5e1-132">Read-only.</span></span> |
|<span data-ttu-id="9e5e1-133">dataType</span><span class="sxs-lookup"><span data-stu-id="9e5e1-133">dataType</span></span>|<span data-ttu-id="9e5e1-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e5e1-134">String</span></span>| <span data-ttu-id="9e5e1-135">Especifica o tipo de dados do valor que a propriedade extension pode manter.</span><span class="sxs-lookup"><span data-stu-id="9e5e1-135">Specifies the data type of the value the extension property can hold.</span></span> <span data-ttu-id="9e5e1-136">Os valores a seguir são suportados.</span><span class="sxs-lookup"><span data-stu-id="9e5e1-136">Following values are supported.</span></span> <span data-ttu-id="9e5e1-137">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="9e5e1-137">Not nullable.</span></span> <ul><li><span data-ttu-id="9e5e1-138">`Binary` - Máximo de 256 bytes</span><span class="sxs-lookup"><span data-stu-id="9e5e1-138">`Binary` - 256 bytes maximum</span></span></li><li>`Boolean`</li><li><span data-ttu-id="9e5e1-139">`DateTime` - Deve ser especificado no formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="9e5e1-139">`DateTime` - Must be specified in ISO 8601 format.</span></span> <span data-ttu-id="9e5e1-140">Serão armazenados no UTC.</span><span class="sxs-lookup"><span data-stu-id="9e5e1-140">Will be stored in UTC.</span></span></li><li><span data-ttu-id="9e5e1-141">`Integer` - Valor de 32 bits.</span><span class="sxs-lookup"><span data-stu-id="9e5e1-141">`Integer` - 32-bit value.</span></span></li><li><span data-ttu-id="9e5e1-142">`LargeInteger` - Valor de 64 bits.</span><span class="sxs-lookup"><span data-stu-id="9e5e1-142">`LargeInteger` - 64-bit value.</span></span></li><li><span data-ttu-id="9e5e1-143">`String` - Máximo de 256 caracteres</span><span class="sxs-lookup"><span data-stu-id="9e5e1-143">`String` - 256 characters maximum</span></span></li></ul>|
|<span data-ttu-id="9e5e1-144">isSyncedFromOnPremises</span><span class="sxs-lookup"><span data-stu-id="9e5e1-144">isSyncedFromOnPremises</span></span>|<span data-ttu-id="9e5e1-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="9e5e1-145">Boolean</span></span>| <span data-ttu-id="9e5e1-146">Indica se essa propriedade de extensão foi sycned do diretório onpremises usando o Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="9e5e1-146">Indicates if this extension property was sycned from onpremises directory using Azure AD Connect.</span></span> <span data-ttu-id="9e5e1-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9e5e1-147">Read-only.</span></span> |
|<span data-ttu-id="9e5e1-148">name</span><span class="sxs-lookup"><span data-stu-id="9e5e1-148">name</span></span>|<span data-ttu-id="9e5e1-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e5e1-149">String</span></span>| <span data-ttu-id="9e5e1-150">Nome da propriedade extension.</span><span class="sxs-lookup"><span data-stu-id="9e5e1-150">Name of the extension property.</span></span> <span data-ttu-id="9e5e1-151">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="9e5e1-151">Not nullable.</span></span> |
|<span data-ttu-id="9e5e1-152">targetObjects</span><span class="sxs-lookup"><span data-stu-id="9e5e1-152">targetObjects</span></span>|<span data-ttu-id="9e5e1-153">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e5e1-153">String collection</span></span>| <span data-ttu-id="9e5e1-154">Os valores a seguir são suportados.</span><span class="sxs-lookup"><span data-stu-id="9e5e1-154">Following values are supported.</span></span> <span data-ttu-id="9e5e1-155">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="9e5e1-155">Not nullable.</span></span> <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|

## <a name="relationships"></a><span data-ttu-id="9e5e1-156">Relações</span><span class="sxs-lookup"><span data-stu-id="9e5e1-156">Relationships</span></span>

<span data-ttu-id="9e5e1-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9e5e1-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e5e1-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9e5e1-158">JSON representation</span></span>

<span data-ttu-id="9e5e1-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9e5e1-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionProperty",
  "keyProperty": "id"
}-->

```json
{
  "appDisplayName": "String",
  "dataType": "String",
  "isSyncedFromOnPremises": true,
  "name": "String",
  "targetObjects": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extensionProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
