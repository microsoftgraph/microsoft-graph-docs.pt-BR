---
title: tipo de recurso de educationSynchronizationLicenseAssignment
description: Representa as informações de licença para atribuir às contas de usuário. O recurso será usado para configurar atribuições de licença ao criar novas contas de usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c60b868ab8d973f6249d7e9ea2b30415d4b8a1b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409675"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="9b0b7-104">tipo de recurso de educationSynchronizationLicenseAssignment</span><span class="sxs-lookup"><span data-stu-id="9b0b7-104">educationSynchronizationLicenseAssignment resource type</span></span>

> <span data-ttu-id="9b0b7-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9b0b7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b0b7-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9b0b7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9b0b7-107">Representa as informações de licença para atribuir às contas de usuário.</span><span class="sxs-lookup"><span data-stu-id="9b0b7-107">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="9b0b7-108">O recurso será usado para configurar atribuições de licença ao criar novas contas de usuário.</span><span class="sxs-lookup"><span data-stu-id="9b0b7-108">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="9b0b7-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9b0b7-109">Properties</span></span>

| <span data-ttu-id="9b0b7-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b0b7-110">Property</span></span> | <span data-ttu-id="9b0b7-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b0b7-111">Type</span></span> | <span data-ttu-id="9b0b7-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b0b7-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="9b0b7-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="9b0b7-113">**appliesTo**</span></span> | <span data-ttu-id="9b0b7-114">string</span><span class="sxs-lookup"><span data-stu-id="9b0b7-114">string</span></span> | <span data-ttu-id="9b0b7-115">O tipo de função de usuário para atribuir a licença.</span><span class="sxs-lookup"><span data-stu-id="9b0b7-115">The user role type to assign to license.</span></span> <span data-ttu-id="9b0b7-116">Os valores possíveis são: `student` e `teacher`.</span><span class="sxs-lookup"><span data-stu-id="9b0b7-116">Possible values are: `student`, `teacher`.</span></span>         |
| <span data-ttu-id="9b0b7-117">**skuIds**</span><span class="sxs-lookup"><span data-stu-id="9b0b7-117">**skuIds**</span></span> | <span data-ttu-id="9b0b7-118">coleção de sequências de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b0b7-118">collection of strings</span></span> |  <span data-ttu-id="9b0b7-119">Representa os identificadores SKU das licenças para atribuir.</span><span class="sxs-lookup"><span data-stu-id="9b0b7-119">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="9b0b7-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9b0b7-120">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "skuIds": ["String"]
}
```
