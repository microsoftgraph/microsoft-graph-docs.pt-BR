---
title: Tipo de recurso iosHomeScreenItem
description: Representa um item na tela inicial do iOS
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b4685c62177dcb7d8cdf0f827d5af085d571d9b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521611"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="e027a-103">Tipo de recurso iosHomeScreenItem</span><span class="sxs-lookup"><span data-stu-id="e027a-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="e027a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e027a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e027a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e027a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e027a-106">Representa um item na tela inicial do iOS</span><span class="sxs-lookup"><span data-stu-id="e027a-106">Represents an item on the iOS Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="e027a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e027a-107">Properties</span></span>
|<span data-ttu-id="e027a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e027a-108">Property</span></span>|<span data-ttu-id="e027a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e027a-109">Type</span></span>|<span data-ttu-id="e027a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e027a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e027a-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e027a-111">displayName</span></span>|<span data-ttu-id="e027a-112">String</span><span class="sxs-lookup"><span data-stu-id="e027a-112">String</span></span>|<span data-ttu-id="e027a-113">Nome do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e027a-113">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="e027a-114">Relações</span><span class="sxs-lookup"><span data-stu-id="e027a-114">Relationships</span></span>
<span data-ttu-id="e027a-115">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e027a-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e027a-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e027a-116">JSON Representation</span></span>
<span data-ttu-id="e027a-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e027a-117">Here is a JSON representation of the resource.</span></span>
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





