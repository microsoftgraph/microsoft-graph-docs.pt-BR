---
title: tipo de recurso de educationSynchronizationLicenseAssignment
description: Representa as informações de licença para atribuir às contas de usuário. O recurso será usado para configurar atribuições de licença ao criar novas contas de usuário.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 9100ba799c8981d5defdd74d6346a66859b2d53e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804904"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="bd9b2-104">tipo de recurso de educationSynchronizationLicenseAssignment</span><span class="sxs-lookup"><span data-stu-id="bd9b2-104">educationSynchronizationLicenseAssignment resource type</span></span>

> <span data-ttu-id="bd9b2-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bd9b2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd9b2-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bd9b2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bd9b2-107">Representa as informações de licença para atribuir às contas de usuário.</span><span class="sxs-lookup"><span data-stu-id="bd9b2-107">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="bd9b2-108">O recurso será usado para configurar atribuições de licença ao criar novas contas de usuário.</span><span class="sxs-lookup"><span data-stu-id="bd9b2-108">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="bd9b2-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bd9b2-109">Properties</span></span>

| <span data-ttu-id="bd9b2-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bd9b2-110">Property</span></span> | <span data-ttu-id="bd9b2-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd9b2-111">Type</span></span> | <span data-ttu-id="bd9b2-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd9b2-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="bd9b2-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="bd9b2-113">**appliesTo**</span></span> | <span data-ttu-id="bd9b2-114">string</span><span class="sxs-lookup"><span data-stu-id="bd9b2-114">string</span></span> | <span data-ttu-id="bd9b2-115">O tipo de função de usuário para atribuir a licença.</span><span class="sxs-lookup"><span data-stu-id="bd9b2-115">The user role type to assign to license.</span></span> <span data-ttu-id="bd9b2-116">Os valores possíveis são: `student` e `teacher`.</span><span class="sxs-lookup"><span data-stu-id="bd9b2-116">Possible values are: `student`, `teacher`.</span></span>         |
| <span data-ttu-id="bd9b2-117">**skuIds**</span><span class="sxs-lookup"><span data-stu-id="bd9b2-117">**skuIds**</span></span> | <span data-ttu-id="bd9b2-118">coleção de sequências de caracteres</span><span class="sxs-lookup"><span data-stu-id="bd9b2-118">collection of strings</span></span> |  <span data-ttu-id="bd9b2-119">Representa os identificadores SKU das licenças para atribuir.</span><span class="sxs-lookup"><span data-stu-id="bd9b2-119">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="bd9b2-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bd9b2-120">JSON representation</span></span>
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
