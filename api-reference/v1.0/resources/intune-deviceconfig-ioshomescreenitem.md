---
title: Tipo de recurso iosHomeScreenItem
description: Representa um item na tela inicial do iOS
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8aecb99c036d3e8a5d89271afd6042ccb18b4fda
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554650"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="fea86-103">Tipo de recurso iosHomeScreenItem</span><span class="sxs-lookup"><span data-stu-id="fea86-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="fea86-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fea86-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fea86-105">Representa um item na tela inicial do iOS</span><span class="sxs-lookup"><span data-stu-id="fea86-105">Represents an item on the iOS Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="fea86-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fea86-106">Properties</span></span>
|<span data-ttu-id="fea86-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fea86-107">Property</span></span>|<span data-ttu-id="fea86-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fea86-108">Type</span></span>|<span data-ttu-id="fea86-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fea86-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fea86-110">displayName</span><span class="sxs-lookup"><span data-stu-id="fea86-110">displayName</span></span>|<span data-ttu-id="fea86-111">String</span><span class="sxs-lookup"><span data-stu-id="fea86-111">String</span></span>|<span data-ttu-id="fea86-112">Nome do aplicativo</span><span class="sxs-lookup"><span data-stu-id="fea86-112">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="fea86-113">Relações</span><span class="sxs-lookup"><span data-stu-id="fea86-113">Relationships</span></span>
<span data-ttu-id="fea86-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fea86-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fea86-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fea86-115">JSON Representation</span></span>
<span data-ttu-id="fea86-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fea86-116">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenItem",
  "displayName": "String"
}
```



