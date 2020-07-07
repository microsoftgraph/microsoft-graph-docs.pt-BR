---
title: tipo de recurso organizationSettings
description: Contém configurações que se aplicam à organização ou aos objetos de usuário dentro dela.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 80b7272915cd6f9dbfc381aa93a32896e2eaf3f5
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050985"
---
# <a name="organizationsettings-resource-type"></a><span data-ttu-id="f3458-103">tipo de recurso organizationSettings</span><span class="sxs-lookup"><span data-stu-id="f3458-103">organizationSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3458-104">Contém configurações que se aplicam à [organização](organization.md) ou que devem ser aplicadas a objetos de [usuário](user.md) em uma organização.</span><span class="sxs-lookup"><span data-stu-id="f3458-104">Contains settings that are applicable to the [organization](organization.md) or that should be applied to [user](user.md) objects within an organization.</span></span>

## <a name="methods"></a><span data-ttu-id="f3458-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="f3458-105">Methods</span></span>

| <span data-ttu-id="f3458-106">Método</span><span class="sxs-lookup"><span data-stu-id="f3458-106">Method</span></span>       | <span data-ttu-id="f3458-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f3458-107">Return Type</span></span> | <span data-ttu-id="f3458-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3458-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f3458-109">Obter configurações da organização</span><span class="sxs-lookup"><span data-stu-id="f3458-109">Get organization settings</span></span>](../api/organizationsettings-get.md) | [<span data-ttu-id="f3458-110">organizationSettings</span><span class="sxs-lookup"><span data-stu-id="f3458-110">organizationSettings</span></span>](organizationsettings.md) | <span data-ttu-id="f3458-111">Leia o objeto de configurações da organização.</span><span class="sxs-lookup"><span data-stu-id="f3458-111">Read the organization settings object.</span></span> |
| [<span data-ttu-id="f3458-112">Criar profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="f3458-112">Create profileCardProperty</span></span>](../api/organizationsettings-post-profilecardproperties.md) | [<span data-ttu-id="f3458-113">profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="f3458-113">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="f3458-114">Crie um novo profileCardProperty postando na coleção profileCardProperties.</span><span class="sxs-lookup"><span data-stu-id="f3458-114">Create a new profileCardProperty by posting to the profileCardProperties collection.</span></span> |
| [<span data-ttu-id="f3458-115">Listar profileCardProperties</span><span class="sxs-lookup"><span data-stu-id="f3458-115">List profileCardProperties</span></span>](../api/organizationsettings-list-profilecardproperties.md) | <span data-ttu-id="f3458-116">coleção [profileCardProperty](profilecardproperty.md)</span><span class="sxs-lookup"><span data-stu-id="f3458-116">[profileCardProperty](profilecardproperty.md) collection</span></span> | <span data-ttu-id="f3458-117">Obtenha uma coleção de objetos profileCardProperty.</span><span class="sxs-lookup"><span data-stu-id="f3458-117">Get a profileCardProperty object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="f3458-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f3458-118">Properties</span></span>

<span data-ttu-id="f3458-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f3458-119">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="f3458-120">Relações</span><span class="sxs-lookup"><span data-stu-id="f3458-120">Relationships</span></span>

| <span data-ttu-id="f3458-121">Relação</span><span class="sxs-lookup"><span data-stu-id="f3458-121">Relationship</span></span> | <span data-ttu-id="f3458-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3458-122">Type</span></span>        | <span data-ttu-id="f3458-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3458-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f3458-124">id</span><span class="sxs-lookup"><span data-stu-id="f3458-124">id</span></span> |<span data-ttu-id="f3458-125">String</span><span class="sxs-lookup"><span data-stu-id="f3458-125">String</span></span>| <span data-ttu-id="f3458-126">ID do objeto de configurações da organização.</span><span class="sxs-lookup"><span data-stu-id="f3458-126">Id of the settings object for the organization.</span></span> |
|<span data-ttu-id="f3458-127">profileCardProperties</span><span class="sxs-lookup"><span data-stu-id="f3458-127">profileCardProperties</span></span>|<span data-ttu-id="f3458-128">coleção [profileCardProperty](profilecardproperty.md)</span><span class="sxs-lookup"><span data-stu-id="f3458-128">[profileCardProperty](profilecardproperty.md) collection</span></span>| <span data-ttu-id="f3458-129">Contém uma coleção das propriedades que um administrador definiu como visível no cartão de perfil do M365.</span><span class="sxs-lookup"><span data-stu-id="f3458-129">Contains a collection of the properties an administrator has defined as visible on the M365 Profile Card.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f3458-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f3458-130">JSON representation</span></span>

<span data-ttu-id="f3458-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f3458-131">The following is a JSON representation of the resource.</span></span>

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
