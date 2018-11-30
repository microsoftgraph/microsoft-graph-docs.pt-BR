---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: VersionAction
ms.openlocfilehash: f22761dd713b6d09d5e6fafb765d6d43bfc81bf9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035071"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="f341e-102">Tipo de recurso VersionAction</span><span class="sxs-lookup"><span data-stu-id="f341e-102">VersionAction resource type</span></span>

> <span data-ttu-id="f341e-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f341e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f341e-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f341e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f341e-105">A presença do recurso **VersionAction** em uma [**itemActivity**][activity] indica que a atividade fez uma nova versão a ser criada.</span><span class="sxs-lookup"><span data-stu-id="f341e-105">The presence of the **VersionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="f341e-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f341e-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.versionAction"
}-->

```json
{
  "newVersion": "string"
}
```

## <a name="properties"></a><span data-ttu-id="f341e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f341e-107">Properties</span></span>

| <span data-ttu-id="f341e-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="f341e-108">Property name</span></span> | <span data-ttu-id="f341e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f341e-109">Type</span></span>   | <span data-ttu-id="f341e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f341e-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="f341e-111">newVersion</span><span class="sxs-lookup"><span data-stu-id="f341e-111">newVersion</span></span>    | <span data-ttu-id="f341e-112">string</span><span class="sxs-lookup"><span data-stu-id="f341e-112">string</span></span> | <span data-ttu-id="f341e-113">O nome da nova versão que foi criada por esta ação.</span><span class="sxs-lookup"><span data-stu-id="f341e-113">The name of the new version that was created by this action.</span></span>

## <a name="remarks"></a><span data-ttu-id="f341e-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="f341e-114">Remarks</span></span>

<span data-ttu-id="f341e-115">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="f341e-115">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The VersionAction object provides information about an activity that resulted in a new item version.",
  "keywords": "activities,activity,action,version",
  "section": "documentation",
  "tocPath": "Resources/VersionAction"
} -->
