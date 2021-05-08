---
title: Tipo de recurso educationTeacher
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `teacher`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6e5e60f04af74cd09f893823e9544ba455b60113
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231840"
---
# <a name="teacher-resource-type"></a><span data-ttu-id="ccc24-103">Tipo de recurso professor</span><span class="sxs-lookup"><span data-stu-id="ccc24-103">Teacher resource type</span></span>

<span data-ttu-id="ccc24-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccc24-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ccc24-105">Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `teacher`.</span><span class="sxs-lookup"><span data-stu-id="ccc24-105">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>

## <a name="properties"></a><span data-ttu-id="ccc24-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ccc24-106">Properties</span></span>

| <span data-ttu-id="ccc24-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ccc24-107">Property</span></span>      | <span data-ttu-id="ccc24-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccc24-108">Type</span></span>   | <span data-ttu-id="ccc24-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccc24-109">Description</span></span>                             |
| :------------ | :----- | :-------------------------------------- |
| <span data-ttu-id="ccc24-110">externalId</span><span class="sxs-lookup"><span data-stu-id="ccc24-110">externalId</span></span>    | <span data-ttu-id="ccc24-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ccc24-111">String</span></span> | <span data-ttu-id="ccc24-112">ID do professor no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="ccc24-112">ID of the teacher in the source system.</span></span> |
| <span data-ttu-id="ccc24-113">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="ccc24-113">teacherNumber</span></span> | <span data-ttu-id="ccc24-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ccc24-114">String</span></span> | <span data-ttu-id="ccc24-115">Número do professor.</span><span class="sxs-lookup"><span data-stu-id="ccc24-115">Teacher number.</span></span>                         |

## <a name="relationships"></a><span data-ttu-id="ccc24-116">Relações</span><span class="sxs-lookup"><span data-stu-id="ccc24-116">Relationships</span></span>

<span data-ttu-id="ccc24-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ccc24-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ccc24-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ccc24-118">JSON representation</span></span>

<span data-ttu-id="ccc24-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ccc24-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationTeacher"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationTeacher",
  "teacherNumber": "String",
  "externalId": "String"
}
```
