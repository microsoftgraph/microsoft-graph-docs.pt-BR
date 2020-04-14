---
title: tipo de recurso extensionproperty
description: Representa uma extensão de diretório
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3d6f6e89ca6e54e1c74e43c6201766aa199f454d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43423794"
---
# <a name="extensionproperty-resource-type"></a><span data-ttu-id="9ae85-103">tipo de recurso extensionproperty</span><span class="sxs-lookup"><span data-stu-id="9ae85-103">extensionProperty resource type</span></span>

<span data-ttu-id="9ae85-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ae85-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ae85-105">Representa uma extensão de diretório que pode ser usada para adicionar uma propriedade personalizada a objetos de diretório sem exigir um repositório de dados externo.</span><span class="sxs-lookup"><span data-stu-id="9ae85-105">Represents a directory extension that can be used to add a custom property to directory objects without requiring an external data store.</span></span> <span data-ttu-id="9ae85-106">Por exemplo, se uma organização tem um aplicativo de linha de negócios (LOB) que requer uma ID do Skype para cada usuário no diretório, o Microsoft Graph pode ser usado para registrar uma nova propriedade chamada SkypeID no objeto de usuário do diretório e, em seguida, escrever um valor para a nova propriedade de um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="9ae85-106">For example, if an organization has a line of business (LOB) application that requires a Skype ID for each user in the directory, Microsoft Graph can be used to register a new property named skypeId on the directory’s User object, and then write a value to the new property for a specific user.</span></span>

<span data-ttu-id="9ae85-107">As extensões podem ser adicionadas a [usuários](user.md), [grupos](group.md), [organizações](organization.md), [dispositivos](device.md)e recursos de [aplicativos](application.md) .</span><span class="sxs-lookup"><span data-stu-id="9ae85-107">Extensions can be added to [user](user.md), [group](group.md), [organization](organization.md), [device](device.md), [application](application.md) resources.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9ae85-108">As extensões de esquema do Azure AD descritas aqui estão disponíveis no Microsoft Graph apenas para fins de compatibilidade com versões anteriores.</span><span class="sxs-lookup"><span data-stu-id="9ae85-108">Azure AD schema extensions described here are available in Microsoft Graph for backwards compatibility reasons only.</span></span>
> <span data-ttu-id="9ae85-109">Ele permite que você use o Microsoft Graph para continuar a gerenciar Propriedades de extensão adicionadas por meio do Azure AD Graph ou [do Azure ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-azure-ad-connect).</span><span class="sxs-lookup"><span data-stu-id="9ae85-109">It allows you to use Microsoft Graph to continue to manage extension properties added through Azure AD Graph or [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-azure-ad-connect).</span></span>
> <span data-ttu-id="9ae85-110">Para novas extensões personalizadas, recomendamos que você use as extensões de esquema do Microsoft Graph para [Adicionar dados personalizados a recursos](/graph/extensibility-overview).</span><span class="sxs-lookup"><span data-stu-id="9ae85-110">For new custom extensions, we recommend that you use Microsoft Graph schema extensions for [adding custom data to resources](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="9ae85-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="9ae85-111">Methods</span></span>

| <span data-ttu-id="9ae85-112">Método</span><span class="sxs-lookup"><span data-stu-id="9ae85-112">Method</span></span>       | <span data-ttu-id="9ae85-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9ae85-113">Return Type</span></span> | <span data-ttu-id="9ae85-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ae85-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9ae85-115">Listar extensões</span><span class="sxs-lookup"><span data-stu-id="9ae85-115">List extensions</span></span>](../api/application-list-extensionproperty.md) | <span data-ttu-id="9ae85-116">Coleção [extensionProperty](extensionProperty.md)</span><span class="sxs-lookup"><span data-stu-id="9ae85-116">[extensionProperty](extensionProperty.md) collection</span></span> | <span data-ttu-id="9ae85-117">Listar propriedades de extensão em um objeto de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9ae85-117">List extension properties on an application object.</span></span> |
| [<span data-ttu-id="9ae85-118">Criar extensão</span><span class="sxs-lookup"><span data-stu-id="9ae85-118">Create extension</span></span>](../api/application-post-extensionproperty.md) | [<span data-ttu-id="9ae85-119">extensionProperty</span><span class="sxs-lookup"><span data-stu-id="9ae85-119">extensionProperty</span></span>](extensionProperty.md) | <span data-ttu-id="9ae85-120">Criar uma propriedade de extensão em um objeto de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9ae85-120">Create an extension property on an application object.</span></span> |
| [<span data-ttu-id="9ae85-121">Excluir extensão</span><span class="sxs-lookup"><span data-stu-id="9ae85-121">Delete extension</span></span>](../api/application-delete-extensionproperty.md) | <span data-ttu-id="9ae85-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9ae85-122">None</span></span> | <span data-ttu-id="9ae85-123">Excluir uma propriedade de extensão de um objeto de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9ae85-123">Delete an extension property from an application object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9ae85-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9ae85-124">Properties</span></span>

| <span data-ttu-id="9ae85-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ae85-125">Property</span></span>     | <span data-ttu-id="9ae85-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ae85-126">Type</span></span>        | <span data-ttu-id="9ae85-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ae85-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9ae85-128">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="9ae85-128">appDisplayName</span></span>|<span data-ttu-id="9ae85-129">String</span><span class="sxs-lookup"><span data-stu-id="9ae85-129">String</span></span>| <span data-ttu-id="9ae85-130">Nome de exibição do objeto de aplicativo no qual essa propriedade de extensão é definida.</span><span class="sxs-lookup"><span data-stu-id="9ae85-130">Display name of the application object on which this extension property is defined.</span></span> <span data-ttu-id="9ae85-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9ae85-131">Read-only.</span></span> |
|<span data-ttu-id="9ae85-132">dataType</span><span class="sxs-lookup"><span data-stu-id="9ae85-132">dataType</span></span>|<span data-ttu-id="9ae85-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ae85-133">String</span></span>| <span data-ttu-id="9ae85-134">Especifica o tipo de dados do valor que a Propriedade Extension pode armazenar.</span><span class="sxs-lookup"><span data-stu-id="9ae85-134">Specifies the data type of the value the extension property can hold.</span></span> <span data-ttu-id="9ae85-135">Os valores a seguir são suportados.</span><span class="sxs-lookup"><span data-stu-id="9ae85-135">Following values are supported.</span></span> <span data-ttu-id="9ae85-136">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="9ae85-136">Not nullable.</span></span> <ul><li><span data-ttu-id="9ae85-137">`Binary`-256 bytes máximo</span><span class="sxs-lookup"><span data-stu-id="9ae85-137">`Binary` - 256 bytes maximum</span></span></li><li>`Boolean`</li><li><span data-ttu-id="9ae85-138">`DateTime`-Deve ser especificado no formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="9ae85-138">`DateTime` - Must be specified in ISO 8601 format.</span></span> <span data-ttu-id="9ae85-139">Serão armazenados no UTC.</span><span class="sxs-lookup"><span data-stu-id="9ae85-139">Will be stored in UTC.</span></span></li><li><span data-ttu-id="9ae85-140">`Integer`-valor de 32-bit.</span><span class="sxs-lookup"><span data-stu-id="9ae85-140">`Integer` - 32-bit value.</span></span></li><li><span data-ttu-id="9ae85-141">`LargeInteger`-valor de 64-bit.</span><span class="sxs-lookup"><span data-stu-id="9ae85-141">`LargeInteger` - 64-bit value.</span></span></li><li><span data-ttu-id="9ae85-142">`String`-256 caracteres no máximo</span><span class="sxs-lookup"><span data-stu-id="9ae85-142">`String` - 256 characters maximum</span></span></li></ul>|
|<span data-ttu-id="9ae85-143">isSyncedFromOnPremises</span><span class="sxs-lookup"><span data-stu-id="9ae85-143">isSyncedFromOnPremises</span></span>|<span data-ttu-id="9ae85-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ae85-144">Boolean</span></span>| <span data-ttu-id="9ae85-145">Indica se esta propriedade de extensão foi sycned do diretório onlocal usando o Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="9ae85-145">Indicates if this extension property was sycned from onpremises directory using Azure AD Connect.</span></span> <span data-ttu-id="9ae85-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9ae85-146">Read-only.</span></span> |
|<span data-ttu-id="9ae85-147">name</span><span class="sxs-lookup"><span data-stu-id="9ae85-147">name</span></span>|<span data-ttu-id="9ae85-148">String</span><span class="sxs-lookup"><span data-stu-id="9ae85-148">String</span></span>| <span data-ttu-id="9ae85-149">Nome da propriedade de extensão.</span><span class="sxs-lookup"><span data-stu-id="9ae85-149">Name of the extension property.</span></span> <span data-ttu-id="9ae85-150">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="9ae85-150">Not nullable.</span></span> |
|<span data-ttu-id="9ae85-151">targetObjects</span><span class="sxs-lookup"><span data-stu-id="9ae85-151">targetObjects</span></span>|<span data-ttu-id="9ae85-152">Coleção String</span><span class="sxs-lookup"><span data-stu-id="9ae85-152">String collection</span></span>| <span data-ttu-id="9ae85-153">Os valores a seguir são suportados.</span><span class="sxs-lookup"><span data-stu-id="9ae85-153">Following values are supported.</span></span> <span data-ttu-id="9ae85-154">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="9ae85-154">Not nullable.</span></span> <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|

## <a name="relationships"></a><span data-ttu-id="9ae85-155">Relações</span><span class="sxs-lookup"><span data-stu-id="9ae85-155">Relationships</span></span>

<span data-ttu-id="9ae85-156">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="9ae85-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ae85-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ae85-157">JSON representation</span></span>

<span data-ttu-id="9ae85-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9ae85-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionProperty",
  "baseType": "",
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
