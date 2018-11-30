---
title: Tipo de recurso educationTeacher
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `teacher`.
ms.openlocfilehash: 37fd46ee00f82b518d91969b1793147be859efdf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033137"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="4041f-103">Tipo de recurso educationTeacher</span><span class="sxs-lookup"><span data-stu-id="4041f-103">educationTeacher resource type</span></span>

> <span data-ttu-id="4041f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4041f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4041f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4041f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4041f-106">Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `teacher`.</span><span class="sxs-lookup"><span data-stu-id="4041f-106">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="4041f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4041f-107">Properties</span></span>
| <span data-ttu-id="4041f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4041f-108">Property</span></span>     | <span data-ttu-id="4041f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4041f-109">Type</span></span>   |<span data-ttu-id="4041f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4041f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4041f-111">externalId</span><span class="sxs-lookup"><span data-stu-id="4041f-111">externalId</span></span>|<span data-ttu-id="4041f-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4041f-112">String</span></span>| <span data-ttu-id="4041f-113">ID do professor no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="4041f-113">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="4041f-114">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="4041f-114">teacherNumber</span></span>|<span data-ttu-id="4041f-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4041f-115">String</span></span>|<span data-ttu-id="4041f-116">Número do professor.</span><span class="sxs-lookup"><span data-stu-id="4041f-116">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4041f-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4041f-117">JSON representation</span></span>

<span data-ttu-id="4041f-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4041f-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTeacher"
}-->

```json
{
  "externalId": "String",
  "teacherNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationTeacher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->