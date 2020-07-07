---
title: tipo de recurso profileCardProperty
description: Usado para designar uma nova propriedade à superfície em uma experiência compartilhada, de pessoas ou uma que terá um nome de exibição ou uma anotação personalizada aplicada a ela. Um administrador pode definir uma cadeia de caracteres de nome para exibição padrão e um conjunto de traduções alternativas para os idiomas que eles dão suporte em sua organização.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 974e1e7af86133ef46c7d4360def1aef153ee3ec
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050991"
---
# <a name="profilecardproperty-resource-type"></a><span data-ttu-id="28dc7-104">tipo de recurso profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="28dc7-104">profileCardProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28dc7-105">Representa um atributo de um usuário no cartão de perfil do Microsoft 365 para uma organização apresentar uma experiência de pessoas compartilhada.</span><span class="sxs-lookup"><span data-stu-id="28dc7-105">Represents an attribute of a user on the Microsoft 365 profile card for an organization to surface in a shared, people experience.</span></span>

<span data-ttu-id="28dc7-106">O atributo pode ser um atributo interno do Azure Active Directory (Azure AD), como `Alias` ou `UserPrincipalName` , ou pode ser um atributo personalizado.</span><span class="sxs-lookup"><span data-stu-id="28dc7-106">The attribute can be an Azure Active Directory (Azure AD) built-in attribute, such as `Alias` or `UserPrincipalName`, or it can be a custom attribute.</span></span> <span data-ttu-id="28dc7-107">Para um atributo personalizado, um administrador pode definir uma `en-us` cadeia de caracteres de nome de exibição padrão e um conjunto de traduções alternativas para os idiomas que eles dão suporte em sua organização.</span><span class="sxs-lookup"><span data-stu-id="28dc7-107">For a custom attribute, an administrator can define an `en-us` default display name string and a set of alternative translations for the languages that they support in their organization.</span></span>

<span data-ttu-id="28dc7-108">Para obter mais informações sobre como adicionar propriedades ao cartão de perfil de uma organização, consulte Customize The Profile Card.</span><span class="sxs-lookup"><span data-stu-id="28dc7-108">For more information on adding properties to the profile card for an organization, see customize the profile card.</span></span>

## <a name="methods"></a><span data-ttu-id="28dc7-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="28dc7-109">Methods</span></span>

| <span data-ttu-id="28dc7-110">Método</span><span class="sxs-lookup"><span data-stu-id="28dc7-110">Method</span></span>       | <span data-ttu-id="28dc7-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="28dc7-111">Return Type</span></span> | <span data-ttu-id="28dc7-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="28dc7-112">Description</span></span> |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="28dc7-113">Listar</span><span class="sxs-lookup"><span data-stu-id="28dc7-113">List</span></span>](../api/organizationsettings-list-profilecardproperties.md) | [<span data-ttu-id="28dc7-114">profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="28dc7-114">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="28dc7-115">Leia as propriedades e os relacionamentos de um objeto **profileCardProperty** .</span><span class="sxs-lookup"><span data-stu-id="28dc7-115">Read the properties and relationships of a **profileCardProperty** object.</span></span> |
| [<span data-ttu-id="28dc7-116">Criar</span><span class="sxs-lookup"><span data-stu-id="28dc7-116">Create</span></span>](../api/organizationsettings-post-profilecardproperties.md) | [<span data-ttu-id="28dc7-117">profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="28dc7-117">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="28dc7-118">Leia as propriedades e os relacionamentos de um objeto **profileCardProperty** .</span><span class="sxs-lookup"><span data-stu-id="28dc7-118">Read the properties and relationships of a **profileCardProperty** object.</span></span> |
| [<span data-ttu-id="28dc7-119">Get</span><span class="sxs-lookup"><span data-stu-id="28dc7-119">Get</span></span>](../api/profilecardproperty-get.md) | [<span data-ttu-id="28dc7-120">profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="28dc7-120">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="28dc7-121">Leia as propriedades e os relacionamentos de um objeto **profileCardProperty** .</span><span class="sxs-lookup"><span data-stu-id="28dc7-121">Read the properties and relationships of a **profileCardProperty** object.</span></span> |
| [<span data-ttu-id="28dc7-122">Update</span><span class="sxs-lookup"><span data-stu-id="28dc7-122">Update</span></span>](../api/profilecardproperty-update.md)               | [<span data-ttu-id="28dc7-123">profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="28dc7-123">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="28dc7-124">Atualizar um objeto **profileCardProperty** .</span><span class="sxs-lookup"><span data-stu-id="28dc7-124">Update a **profileCardProperty** object.</span></span>                               |
| [<span data-ttu-id="28dc7-125">Delete</span><span class="sxs-lookup"><span data-stu-id="28dc7-125">Delete</span></span>](../api/profilecardproperty-delete.md)               | <span data-ttu-id="28dc7-126">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="28dc7-126">None</span></span>                                          | <span data-ttu-id="28dc7-127">Excluir um objeto **profileCardProperty** .</span><span class="sxs-lookup"><span data-stu-id="28dc7-127">Delete a **profileCardProperty** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="28dc7-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="28dc7-128">Properties</span></span>

| <span data-ttu-id="28dc7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28dc7-129">Property</span></span>             | <span data-ttu-id="28dc7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="28dc7-130">Type</span></span>                                                        | <span data-ttu-id="28dc7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="28dc7-131">Description</span></span> |
|:---------------------|:------------------------------------------------------------|:------------|
|<span data-ttu-id="28dc7-132">anotações</span><span class="sxs-lookup"><span data-stu-id="28dc7-132">annotations</span></span>           |<span data-ttu-id="28dc7-133">coleção [profileCardAnnotation](profilecardannotation.md)</span><span class="sxs-lookup"><span data-stu-id="28dc7-133">[profileCardAnnotation](profilecardannotation.md) collection</span></span> | <span data-ttu-id="28dc7-134">Permite que um administrador defina um rótulo de exibição personalizado para a propriedade Directory e o localize para os usuários em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="28dc7-134">Allows an administrator to set a custom display label for the directory property and localize it for the users in their tenant.</span></span>|
|<span data-ttu-id="28dc7-135">directoryPropertyName</span><span class="sxs-lookup"><span data-stu-id="28dc7-135">directoryPropertyName</span></span> |<span data-ttu-id="28dc7-136">String</span><span class="sxs-lookup"><span data-stu-id="28dc7-136">String</span></span>                                                       | <span data-ttu-id="28dc7-137">Identifica um recurso do **profileCardProperty** em operações [Get](../api/profilecardproperty-get.md), [Update](../api/profilecardproperty-update.md)ou [delete](../api/profilecardproperty-delete.md) .</span><span class="sxs-lookup"><span data-stu-id="28dc7-137">Identifies a **profileCardProperty** resource in [Get](../api/profilecardproperty-get.md), [Update](../api/profilecardproperty-update.md), or [Delete](../api/profilecardproperty-delete.md) operations.</span></span> <span data-ttu-id="28dc7-138">Permite que um administrador Surface as propriedades do Azure Active Directory (Azure AD) ocultas no cartão de perfil do Microsoft 365 dentro de seu locatário.</span><span class="sxs-lookup"><span data-stu-id="28dc7-138">Allows an administrator to surface hidden Azure Active Directory (Azure AD) properties on the Microsoft 365 profile card within their tenant.</span></span> <span data-ttu-id="28dc7-139">Quando presente, o campo do Azure AD mencionado neste campo ficará visível para todos os usuários em seu locatário no painel de contato do cartão de perfil.</span><span class="sxs-lookup"><span data-stu-id="28dc7-139">When present, the Azure AD field referenced in this field will be visible to all users in your tenant on the contact pane of the profile card.</span></span> <span data-ttu-id="28dc7-140">Os valores permitidos para este campo são:,,,,,,,,,, `UserPrincipalName` `Fax` `StreetAddress` `PostalCode` `StateOrProvince` `Alias` `CustomAttribute1` `CustomAttribute2` `CustomAttribute3` `CustomAttribute4` `CustomAttribute5` `CustomAttribute6` , `CustomAttribute7` , `CustomAttribute8` , `CustomAttribute9` , `CustomAttribute10` , `CustomAttribute11` , `CustomAttribute12` `CustomAttribute13` `CustomAttribute14` `CustomAttribute15` ,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="28dc7-140">Allowed values for this field are: `UserPrincipalName`, `Fax`, `StreetAddress`, `PostalCode`, `StateOrProvince`, `Alias`, `CustomAttribute1`,  `CustomAttribute2`, `CustomAttribute3`, `CustomAttribute4`, `CustomAttribute5`, `CustomAttribute6`, `CustomAttribute7`, `CustomAttribute8`, `CustomAttribute9`, `CustomAttribute10`, `CustomAttribute11`, `CustomAttribute12`, `CustomAttribute13`, `CustomAttribute14`, `CustomAttribute15`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="28dc7-141">Relações</span><span class="sxs-lookup"><span data-stu-id="28dc7-141">Relationships</span></span>

<span data-ttu-id="28dc7-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="28dc7-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="28dc7-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="28dc7-143">JSON representation</span></span>

<span data-ttu-id="28dc7-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="28dc7-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profileCardProperty",
  "baseType": ""
}-->

```json
{
  "annotations": [
    {
      "displayName": "String",
      "localizations": [
        {
          "languageTag": "String",
          "displayName": "String"
        }
      ]
    }
  ],
  "directoryPropertyName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profileCardProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->