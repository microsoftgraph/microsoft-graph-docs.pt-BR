---
title: tipo de recurso de educationSynchronizationLicenseAssignment
description: Representa as informações de licença para atribuir às contas de usuário. O recurso será usado para configurar atribuições de licença ao criar novas contas de usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 757e080a8b2c6f3f01fa1663f10c9b0b98eaf4d3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948272"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="0505e-104">tipo de recurso de educationSynchronizationLicenseAssignment</span><span class="sxs-lookup"><span data-stu-id="0505e-104">educationSynchronizationLicenseAssignment resource type</span></span>

> <span data-ttu-id="0505e-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0505e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0505e-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0505e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0505e-107">Representa as informações de licença para atribuir às contas de usuário.</span><span class="sxs-lookup"><span data-stu-id="0505e-107">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="0505e-108">O recurso será usado para configurar atribuições de licença ao criar novas contas de usuário.</span><span class="sxs-lookup"><span data-stu-id="0505e-108">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="0505e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0505e-109">Properties</span></span>

| <span data-ttu-id="0505e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0505e-110">Property</span></span> | <span data-ttu-id="0505e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="0505e-111">Type</span></span> | <span data-ttu-id="0505e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0505e-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="0505e-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="0505e-113">**appliesTo**</span></span> | <span data-ttu-id="0505e-114">string</span><span class="sxs-lookup"><span data-stu-id="0505e-114">string</span></span> | <span data-ttu-id="0505e-115">O tipo de função de usuário para atribuir a licença.</span><span class="sxs-lookup"><span data-stu-id="0505e-115">The user role type to assign to license.</span></span> <span data-ttu-id="0505e-116">Os valores possíveis são: `student` e `teacher`.</span><span class="sxs-lookup"><span data-stu-id="0505e-116">Possible values are: `student`, `teacher`.</span></span>         |
| <span data-ttu-id="0505e-117">**skuIds**</span><span class="sxs-lookup"><span data-stu-id="0505e-117">**skuIds**</span></span> | <span data-ttu-id="0505e-118">coleção de sequências de caracteres</span><span class="sxs-lookup"><span data-stu-id="0505e-118">collection of strings</span></span> |  <span data-ttu-id="0505e-119">Representa os identificadores SKU das licenças para atribuir.</span><span class="sxs-lookup"><span data-stu-id="0505e-119">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="0505e-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0505e-120">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
    "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
    "skuIds": ["String"]
}
```
