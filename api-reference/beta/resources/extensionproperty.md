---
title: Tipo de recurso extensionProperty
description: Representa uma extensão de diretório
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 4f88629c1b2044cf8c5f92ff90d1d334973f5db7
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161723"
---
# <a name="extensionproperty-resource-type"></a><span data-ttu-id="577d7-103">Tipo de recurso extensionProperty</span><span class="sxs-lookup"><span data-stu-id="577d7-103">extensionProperty resource type</span></span>

<span data-ttu-id="577d7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="577d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="577d7-105">Representa uma extensão de diretório que pode ser usada para adicionar uma propriedade personalizada a objetos de diretório sem a necessidade de um armazenamento de dados externos.</span><span class="sxs-lookup"><span data-stu-id="577d7-105">Represents a directory extension that can be used to add a custom property to directory objects without requiring an external data store.</span></span> <span data-ttu-id="577d7-106">Por exemplo, se uma organização tiver um aplicativo de linha de negócios (LOB) que exija uma ID do Skype para cada usuário no diretório, o Microsoft Graph poderá ser usado para registrar uma nova propriedade chamada skypeId no objeto User do diretório e gravar um valor na nova propriedade de um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="577d7-106">For example, if an organization has a line of business (LOB) application that requires a Skype ID for each user in the directory, Microsoft Graph can be used to register a new property named skypeId on the directory’s User object, and then write a value to the new property for a specific user.</span></span>

<span data-ttu-id="577d7-107">As extensões podem ser adicionadas ao [usuário,](user.md) [grupo,](group.md) [organização,](organization.md) [dispositivo,](device.md)recursos [do](application.md) aplicativo.</span><span class="sxs-lookup"><span data-stu-id="577d7-107">Extensions can be added to [user](user.md), [group](group.md), [organization](organization.md), [device](device.md), [application](application.md) resources.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="577d7-108">As extensões de esquema do Azure AD descritas aqui estão disponíveis no Microsoft Graph apenas por motivos de compatibilidade com compatibilidade com compatibilidade.</span><span class="sxs-lookup"><span data-stu-id="577d7-108">Azure AD schema extensions described here are available in Microsoft Graph for backwards compatibility reasons only.</span></span>
> <span data-ttu-id="577d7-109">Ele permite que você use o Microsoft Graph para continuar a gerenciar as propriedades de extensão adicionadas por meio do Azure AD Graph ou [do Azure AD Connect.](/azure/active-directory/hybrid/whatis-azure-ad-connect)</span><span class="sxs-lookup"><span data-stu-id="577d7-109">It allows you to use Microsoft Graph to continue to manage extension properties added through Azure AD Graph or [Azure AD Connect](/azure/active-directory/hybrid/whatis-azure-ad-connect).</span></span>
> <span data-ttu-id="577d7-110">Para novas extensões personalizadas, recomendamos que você use extensões de esquema do Microsoft Graph para [adicionar dados personalizados aos recursos.](/graph/extensibility-overview)</span><span class="sxs-lookup"><span data-stu-id="577d7-110">For new custom extensions, we recommend that you use Microsoft Graph schema extensions for [adding custom data to resources](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="577d7-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="577d7-111">Methods</span></span>

| <span data-ttu-id="577d7-112">Método</span><span class="sxs-lookup"><span data-stu-id="577d7-112">Method</span></span>       | <span data-ttu-id="577d7-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="577d7-113">Return Type</span></span> | <span data-ttu-id="577d7-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="577d7-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="577d7-115">Listar extensões</span><span class="sxs-lookup"><span data-stu-id="577d7-115">List extensions</span></span>](../api/application-list-extensionproperty.md) | <span data-ttu-id="577d7-116">Coleção [extensionProperty](extensionProperty.md)</span><span class="sxs-lookup"><span data-stu-id="577d7-116">[extensionProperty](extensionProperty.md) collection</span></span> | <span data-ttu-id="577d7-117">Listar propriedades de extensão em um objeto de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="577d7-117">List extension properties on an application object.</span></span> |
| [<span data-ttu-id="577d7-118">Criar extensão</span><span class="sxs-lookup"><span data-stu-id="577d7-118">Create extension</span></span>](../api/application-post-extensionproperty.md) | [<span data-ttu-id="577d7-119">extensionProperty</span><span class="sxs-lookup"><span data-stu-id="577d7-119">extensionProperty</span></span>](extensionProperty.md) | <span data-ttu-id="577d7-120">Criar uma propriedade de extensão em um objeto de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="577d7-120">Create an extension property on an application object.</span></span> |
| [<span data-ttu-id="577d7-121">Excluir extensão</span><span class="sxs-lookup"><span data-stu-id="577d7-121">Delete extension</span></span>](../api/application-delete-extensionproperty.md) | <span data-ttu-id="577d7-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="577d7-122">None</span></span> | <span data-ttu-id="577d7-123">Excluir uma propriedade de extensão de um objeto de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="577d7-123">Delete an extension property from an application object.</span></span> |

## <a name="properties"></a><span data-ttu-id="577d7-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="577d7-124">Properties</span></span>

| <span data-ttu-id="577d7-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="577d7-125">Property</span></span>     | <span data-ttu-id="577d7-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="577d7-126">Type</span></span>        | <span data-ttu-id="577d7-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="577d7-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="577d7-128">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="577d7-128">appDisplayName</span></span>|<span data-ttu-id="577d7-129">String</span><span class="sxs-lookup"><span data-stu-id="577d7-129">String</span></span>| <span data-ttu-id="577d7-130">Nome de exibição do objeto de aplicativo no qual essa propriedade de extensão está definida.</span><span class="sxs-lookup"><span data-stu-id="577d7-130">Display name of the application object on which this extension property is defined.</span></span> <span data-ttu-id="577d7-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="577d7-131">Read-only.</span></span> |
|<span data-ttu-id="577d7-132">dataType</span><span class="sxs-lookup"><span data-stu-id="577d7-132">dataType</span></span>|<span data-ttu-id="577d7-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="577d7-133">String</span></span>| <span data-ttu-id="577d7-134">Especifica o tipo de dados do valor que a propriedade de extensão pode conter.</span><span class="sxs-lookup"><span data-stu-id="577d7-134">Specifies the data type of the value the extension property can hold.</span></span> <span data-ttu-id="577d7-135">Os valores a seguir são suportados.</span><span class="sxs-lookup"><span data-stu-id="577d7-135">Following values are supported.</span></span> <span data-ttu-id="577d7-136">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="577d7-136">Not nullable.</span></span> <ul><li><span data-ttu-id="577d7-137">`Binary` - Máximo de 256 bytes</span><span class="sxs-lookup"><span data-stu-id="577d7-137">`Binary` - 256 bytes maximum</span></span></li><li>`Boolean`</li><li><span data-ttu-id="577d7-138">`DateTime` - Deve ser especificado no formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="577d7-138">`DateTime` - Must be specified in ISO 8601 format.</span></span> <span data-ttu-id="577d7-139">Serão armazenados no UTC.</span><span class="sxs-lookup"><span data-stu-id="577d7-139">Will be stored in UTC.</span></span></li><li><span data-ttu-id="577d7-140">`Integer` - Valor de 32 bits.</span><span class="sxs-lookup"><span data-stu-id="577d7-140">`Integer` - 32-bit value.</span></span></li><li><span data-ttu-id="577d7-141">`LargeInteger` - Valor de 64 bits.</span><span class="sxs-lookup"><span data-stu-id="577d7-141">`LargeInteger` - 64-bit value.</span></span></li><li><span data-ttu-id="577d7-142">`String` - Máximo de 256 caracteres</span><span class="sxs-lookup"><span data-stu-id="577d7-142">`String` - 256 characters maximum</span></span></li></ul>|
|<span data-ttu-id="577d7-143">isSyncedFromOnPremises</span><span class="sxs-lookup"><span data-stu-id="577d7-143">isSyncedFromOnPremises</span></span>|<span data-ttu-id="577d7-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="577d7-144">Boolean</span></span>| <span data-ttu-id="577d7-145">Indica se essa propriedade de extensão foi sycned do diretório onpremises usando o Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="577d7-145">Indicates if this extension property was sycned from onpremises directory using Azure AD Connect.</span></span> <span data-ttu-id="577d7-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="577d7-146">Read-only.</span></span> |
|<span data-ttu-id="577d7-147">name</span><span class="sxs-lookup"><span data-stu-id="577d7-147">name</span></span>|<span data-ttu-id="577d7-148">String</span><span class="sxs-lookup"><span data-stu-id="577d7-148">String</span></span>| <span data-ttu-id="577d7-149">Nome da propriedade de extensão.</span><span class="sxs-lookup"><span data-stu-id="577d7-149">Name of the extension property.</span></span> <span data-ttu-id="577d7-150">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="577d7-150">Not nullable.</span></span> |
|<span data-ttu-id="577d7-151">targetObjects</span><span class="sxs-lookup"><span data-stu-id="577d7-151">targetObjects</span></span>|<span data-ttu-id="577d7-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="577d7-152">String collection</span></span>| <span data-ttu-id="577d7-153">Os valores a seguir são suportados.</span><span class="sxs-lookup"><span data-stu-id="577d7-153">Following values are supported.</span></span> <span data-ttu-id="577d7-154">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="577d7-154">Not nullable.</span></span> <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|

## <a name="relationships"></a><span data-ttu-id="577d7-155">Relações</span><span class="sxs-lookup"><span data-stu-id="577d7-155">Relationships</span></span>

<span data-ttu-id="577d7-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="577d7-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="577d7-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="577d7-157">JSON representation</span></span>

<span data-ttu-id="577d7-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="577d7-158">The following is a JSON representation of the resource.</span></span>

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
