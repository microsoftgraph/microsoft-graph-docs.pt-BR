---
title: tipo de recurso organizationSettings
description: Contém configurações que se aplicam à organização ou aos objetos de usuário dentro dela.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 73171beee516c63f75649375b7f084c01bac543f
ms.sourcegitcommit: 20b951f8bd245bb3a2bc7d3f5533e8619e9db084
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/27/2020
ms.locfileid: "45427253"
---
# <a name="organizationsettings-resource-type"></a><span data-ttu-id="0fb3a-103">tipo de recurso organizationSettings</span><span class="sxs-lookup"><span data-stu-id="0fb3a-103">organizationSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fb3a-104">Contém configurações que se aplicam à [organização](organization.md) ou que devem ser aplicadas a objetos de [usuário](user.md) em uma organização.</span><span class="sxs-lookup"><span data-stu-id="0fb3a-104">Contains settings that are applicable to the [organization](organization.md) or that should be applied to [user](user.md) objects within an organization.</span></span>

## <a name="methods"></a><span data-ttu-id="0fb3a-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="0fb3a-105">Methods</span></span>

| <span data-ttu-id="0fb3a-106">Método</span><span class="sxs-lookup"><span data-stu-id="0fb3a-106">Method</span></span>       | <span data-ttu-id="0fb3a-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0fb3a-107">Return Type</span></span> | <span data-ttu-id="0fb3a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0fb3a-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0fb3a-109">Obter configurações da organização</span><span class="sxs-lookup"><span data-stu-id="0fb3a-109">Get organization settings</span></span>](../api/organizationsettings-get.md) | [<span data-ttu-id="0fb3a-110">organizationSettings</span><span class="sxs-lookup"><span data-stu-id="0fb3a-110">organizationSettings</span></span>](organizationsettings.md) | <span data-ttu-id="0fb3a-111">Leia o objeto de configurações da organização.</span><span class="sxs-lookup"><span data-stu-id="0fb3a-111">Read the organization settings object.</span></span> |
| [<span data-ttu-id="0fb3a-112">Criar profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="0fb3a-112">Create profileCardProperty</span></span>](../api/organizationsettings-post-profilecardproperties.md) | [<span data-ttu-id="0fb3a-113">profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="0fb3a-113">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="0fb3a-114">Crie um novo **profileCardProperty** postando na coleção de objetos **profileCardProperty** .</span><span class="sxs-lookup"><span data-stu-id="0fb3a-114">Create a new **profileCardProperty** by posting to the **profileCardProperty** object collection.</span></span> |
| [<span data-ttu-id="0fb3a-115">Listar profileCardProperties</span><span class="sxs-lookup"><span data-stu-id="0fb3a-115">List profileCardProperties</span></span>](../api/organizationsettings-list-profilecardproperties.md) | <span data-ttu-id="0fb3a-116">coleção [profileCardProperty](profilecardproperty.md)</span><span class="sxs-lookup"><span data-stu-id="0fb3a-116">[profileCardProperty](profilecardproperty.md) collection</span></span> | <span data-ttu-id="0fb3a-117">Obtenha uma coleção de objetos **profileCardProperty** .</span><span class="sxs-lookup"><span data-stu-id="0fb3a-117">Get a **profileCardProperty** object collection.</span></span> |
| [<span data-ttu-id="0fb3a-118">Obter itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="0fb3a-118">Get itemInsightsSettings</span></span>](../api/iteminsightssettings-get.md) | [<span data-ttu-id="0fb3a-119">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="0fb3a-119">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="0fb3a-120">Obter as propriedades de um objeto **itemInsightsSettings** .</span><span class="sxs-lookup"><span data-stu-id="0fb3a-120">Get the properties of an **itemInsightsSettings** object.</span></span> |
| [<span data-ttu-id="0fb3a-121">Atualizar itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="0fb3a-121">Update itemInsightsSettings</span></span>](../api/iteminsightssettings-update.md) | [<span data-ttu-id="0fb3a-122">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="0fb3a-122">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="0fb3a-123">Atualiza as propriedades do recurso **itemInsightsSettings** especificado.</span><span class="sxs-lookup"><span data-stu-id="0fb3a-123">Update the properties of the specified **itemInsightsSettings** resource.</span></span> |

## <a name="properties"></a><span data-ttu-id="0fb3a-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0fb3a-124">Properties</span></span>

<span data-ttu-id="0fb3a-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0fb3a-125">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="0fb3a-126">Relações</span><span class="sxs-lookup"><span data-stu-id="0fb3a-126">Relationships</span></span>

| <span data-ttu-id="0fb3a-127">Relação</span><span class="sxs-lookup"><span data-stu-id="0fb3a-127">Relationship</span></span> | <span data-ttu-id="0fb3a-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="0fb3a-128">Type</span></span>        | <span data-ttu-id="0fb3a-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="0fb3a-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0fb3a-130">id</span><span class="sxs-lookup"><span data-stu-id="0fb3a-130">id</span></span> |<span data-ttu-id="0fb3a-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0fb3a-131">String</span></span>| <span data-ttu-id="0fb3a-132">ID do objeto de configurações da organização.</span><span class="sxs-lookup"><span data-stu-id="0fb3a-132">Id of the settings object for the organization.</span></span> |
|<span data-ttu-id="0fb3a-133">profileCardProperties</span><span class="sxs-lookup"><span data-stu-id="0fb3a-133">profileCardProperties</span></span>|<span data-ttu-id="0fb3a-134">coleção [profileCardProperty](profilecardproperty.md)</span><span class="sxs-lookup"><span data-stu-id="0fb3a-134">[profileCardProperty](profilecardproperty.md) collection</span></span>| <span data-ttu-id="0fb3a-135">Contém uma coleção de propriedades que um administrador definiu como visível no cartão de perfil do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0fb3a-135">Contains a collection of the properties an administrator has defined as visible on the Microsoft 365 profile card.</span></span> <span data-ttu-id="0fb3a-136">[Obter configurações da organização](../api/organizationsettings-get.md) retorna as propriedades configuradas para cartões de perfil para a organização.</span><span class="sxs-lookup"><span data-stu-id="0fb3a-136">[Get organization settings](../api/organizationsettings-get.md) returns the properties configured for profile cards for the organization.</span></span>|
|<span data-ttu-id="0fb3a-137">Ideias</span><span class="sxs-lookup"><span data-stu-id="0fb3a-137">itemInsights</span></span>|[<span data-ttu-id="0fb3a-138">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="0fb3a-138">itemInsightsSettings</span></span>](iteminsightssettings.md)| <span data-ttu-id="0fb3a-139">Contém as propriedades que são configuradas por um administrador para a visibilidade das ideias derivadas do Microsoft Graph, entre um usuário e outros itens no Microsoft 365, como documentos ou sites.</span><span class="sxs-lookup"><span data-stu-id="0fb3a-139">Contains the properties that are configured by an administrator for the visibility of Microsoft Graph-derived insights, between a user and other items in Microsoft 365, such as documents or sites.</span></span> <span data-ttu-id="0fb3a-140">[Obtenha itemInsightsSettings](../api/iteminsightssettings-get.md) por meio dessa propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="0fb3a-140">[Get itemInsightsSettings](../api/iteminsightssettings-get.md) through this navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0fb3a-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0fb3a-141">JSON representation</span></span>

<span data-ttu-id="0fb3a-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0fb3a-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizationSettings",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "profileCardProperties": [{"@odata.type": "microsoft.graph.profileCardProperty"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organizationSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
