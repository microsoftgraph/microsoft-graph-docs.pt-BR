---
title: tipo de recurso extensionproperty
description: Representa uma extensão de diretório
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 81bda27c0bee96fbac30e4f586e5ffb4a78bac09
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939499"
---
# <a name="extensionproperty-resource-type"></a><span data-ttu-id="2ee01-103">tipo de recurso extensionproperty</span><span class="sxs-lookup"><span data-stu-id="2ee01-103">extensionProperty resource type</span></span>

<span data-ttu-id="2ee01-104">Representa uma extensão de diretório que pode ser usada para adicionar uma propriedade personalizada a objetos de diretório sem exigir um repositório de dados externo.</span><span class="sxs-lookup"><span data-stu-id="2ee01-104">Represents a directory extension that can be used to add a custom property to directory objects without requiring an external data store.</span></span> <span data-ttu-id="2ee01-105">Por exemplo, se uma organização tem um aplicativo de linha de negócios (LOB) que requer uma ID do Skype para cada usuário no diretório, o Microsoft Graph pode ser usado para registrar uma nova propriedade denominada SkypeID no objeto de usuário do diretório e, em seguida, escrever um valor para a nova propriedade para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="2ee01-105">For example, if an organization has a line of business (LOB) application that requires a Skype ID for each user in the directory, Microsoft Graph can be used to register a new property named skypeId on the directory’s User object, and then write a value to the new property for a specific user.</span></span>

<span data-ttu-id="2ee01-106">As extensões podem ser adicionadas a [usuários](user.md), [grupos](group.md), [organizações](organization.md), [dispositivos](device.md)e recursos de [aplicativos](application.md) .</span><span class="sxs-lookup"><span data-stu-id="2ee01-106">Extensions can be added to [user](user.md), [group](group.md), [organization](organization.md), [device](device.md), [application](application.md) resources.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="2ee01-107">As extensões de esquema do Azure AD descritas aqui estão disponíveis no Microsoft Graph apenas para fins de compatibilidade com versões anteriores.</span><span class="sxs-lookup"><span data-stu-id="2ee01-107">Azure AD schema extensions described here are available in Microsoft Graph for backwards compatibility reasons only.</span></span>
> <span data-ttu-id="2ee01-108">Ele permite que você use o Microsoft Graph para continuar a gerenciar Propriedades de extensão adicionadas por meio do Azure AD Graph ou [do Azure ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-azure-ad-connect).</span><span class="sxs-lookup"><span data-stu-id="2ee01-108">It allows you to use Microsoft Graph to continue to manage extension properties added through Azure AD Graph or [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-azure-ad-connect).</span></span>
> <span data-ttu-id="2ee01-109">Para novas extensões personalizadas, recomendamos que você use as extensões de esquema do Microsoft Graph para [Adicionar dados personalizados a recursos](/graph/extensibility-overview).</span><span class="sxs-lookup"><span data-stu-id="2ee01-109">For new custom extensions, we recommend that you use Microsoft Graph schema extensions for [adding custom data to resources](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="2ee01-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="2ee01-110">Methods</span></span>

| <span data-ttu-id="2ee01-111">Método</span><span class="sxs-lookup"><span data-stu-id="2ee01-111">Method</span></span>       | <span data-ttu-id="2ee01-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2ee01-112">Return Type</span></span> | <span data-ttu-id="2ee01-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ee01-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2ee01-114">Criar extensão</span><span class="sxs-lookup"><span data-stu-id="2ee01-114">Create extension</span></span>](../api/application-post-extensionproperty.md) | [<span data-ttu-id="2ee01-115">extensionproperty</span><span class="sxs-lookup"><span data-stu-id="2ee01-115">extensionProperty</span></span>](extensionProperty.md) | <span data-ttu-id="2ee01-116">Criar uma propriedade de extensão em um objeto Application.</span><span class="sxs-lookup"><span data-stu-id="2ee01-116">Create an extension property on an application object.</span></span> |
| [<span data-ttu-id="2ee01-117">Listar extensões</span><span class="sxs-lookup"><span data-stu-id="2ee01-117">List extensions</span></span>](../api/application-list-extensionproperty.md) | <span data-ttu-id="2ee01-118">coleção [extensionproperty](extensionProperty.md)</span><span class="sxs-lookup"><span data-stu-id="2ee01-118">[extensionProperty](extensionProperty.md) collection</span></span> | <span data-ttu-id="2ee01-119">Listar Propriedades de extensão em um objeto Application.</span><span class="sxs-lookup"><span data-stu-id="2ee01-119">List extension properties on an application object.</span></span> |
| [<span data-ttu-id="2ee01-120">Excluir extensão</span><span class="sxs-lookup"><span data-stu-id="2ee01-120">Delete extension</span></span>](../api/application-delete-extensionproperty.md) | <span data-ttu-id="2ee01-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2ee01-121">None</span></span> | <span data-ttu-id="2ee01-122">Excluir uma propriedade de extensão de um objeto Application.</span><span class="sxs-lookup"><span data-stu-id="2ee01-122">Delete an extension property from an application object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2ee01-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ee01-123">Properties</span></span>

| <span data-ttu-id="2ee01-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ee01-124">Property</span></span>     | <span data-ttu-id="2ee01-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ee01-125">Type</span></span>        | <span data-ttu-id="2ee01-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ee01-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2ee01-127">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="2ee01-127">appDisplayName</span></span>|<span data-ttu-id="2ee01-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ee01-128">String</span></span>| <span data-ttu-id="2ee01-129">Nome de exibição do objeto de aplicativo no qual essa propriedade de extensão é definida.</span><span class="sxs-lookup"><span data-stu-id="2ee01-129">Display name of the application object on which this extension property is defined.</span></span> <span data-ttu-id="2ee01-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee01-130">Read-only.</span></span> |
|<span data-ttu-id="2ee01-131">dataType</span><span class="sxs-lookup"><span data-stu-id="2ee01-131">dataType</span></span>|<span data-ttu-id="2ee01-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ee01-132">String</span></span>| <span data-ttu-id="2ee01-133">Especifica o tipo de dados do valor que a Propriedade Extension pode armazenar.</span><span class="sxs-lookup"><span data-stu-id="2ee01-133">Specifies the data type of the value the extension property can hold.</span></span> <span data-ttu-id="2ee01-134">Os valores a seguir são suportados.</span><span class="sxs-lookup"><span data-stu-id="2ee01-134">Following values are supported.</span></span> <span data-ttu-id="2ee01-135">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="2ee01-135">Not nullable.</span></span> <ul><li><span data-ttu-id="2ee01-136">`Binary`-256 bytes máximo</span><span class="sxs-lookup"><span data-stu-id="2ee01-136">`Binary` - 256 bytes maximum</span></span></li><li>`Boolean`</li><li><span data-ttu-id="2ee01-137">`DateTime`-Deve ser especificado no formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="2ee01-137">`DateTime` - Must be specified in ISO 8601 format.</span></span> <span data-ttu-id="2ee01-138">Serão armazenados no UTC.</span><span class="sxs-lookup"><span data-stu-id="2ee01-138">Will be stored in UTC.</span></span></li><li><span data-ttu-id="2ee01-139">`Integer`-valor de 32-bit.</span><span class="sxs-lookup"><span data-stu-id="2ee01-139">`Integer` - 32-bit value.</span></span></li><li><span data-ttu-id="2ee01-140">`LargeInteger`-valor de 64-bit.</span><span class="sxs-lookup"><span data-stu-id="2ee01-140">`LargeInteger` - 64-bit value.</span></span></li><li><span data-ttu-id="2ee01-141">`String`-256 caracteres no máximo</span><span class="sxs-lookup"><span data-stu-id="2ee01-141">`String` - 256 characters maximum</span></span></li></ul>|
|<span data-ttu-id="2ee01-142">isSyncedFromOnPremises</span><span class="sxs-lookup"><span data-stu-id="2ee01-142">isSyncedFromOnPremises</span></span>|<span data-ttu-id="2ee01-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ee01-143">Boolean</span></span>| <span data-ttu-id="2ee01-144">Indica se esta propriedade de extensão foi sycned do diretório onlocal usando o Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="2ee01-144">Indicates if this extension property was sycned from onpremises directory using Azure AD Connect.</span></span> <span data-ttu-id="2ee01-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee01-145">Read-only.</span></span> |
|<span data-ttu-id="2ee01-146">name</span><span class="sxs-lookup"><span data-stu-id="2ee01-146">name</span></span>|<span data-ttu-id="2ee01-147">String</span><span class="sxs-lookup"><span data-stu-id="2ee01-147">String</span></span>| <span data-ttu-id="2ee01-148">Nome da propriedade de extensão.</span><span class="sxs-lookup"><span data-stu-id="2ee01-148">Name of the extension property.</span></span> <span data-ttu-id="2ee01-149">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="2ee01-149">Not nullable.</span></span> |
|<span data-ttu-id="2ee01-150">targetObjects</span><span class="sxs-lookup"><span data-stu-id="2ee01-150">targetObjects</span></span>|<span data-ttu-id="2ee01-151">String collection</span><span class="sxs-lookup"><span data-stu-id="2ee01-151">String collection</span></span>| <span data-ttu-id="2ee01-152">Os valores a seguir são suportados.</span><span class="sxs-lookup"><span data-stu-id="2ee01-152">Following values are supported.</span></span> <span data-ttu-id="2ee01-153">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="2ee01-153">Not nullable.</span></span> <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|

## <a name="relationships"></a><span data-ttu-id="2ee01-154">Relações</span><span class="sxs-lookup"><span data-stu-id="2ee01-154">Relationships</span></span>

<span data-ttu-id="2ee01-155">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2ee01-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ee01-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ee01-156">JSON representation</span></span>

<span data-ttu-id="2ee01-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ee01-157">The following is a JSON representation of the resource.</span></span>

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
