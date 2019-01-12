---
title: Tipo de recurso iosHomeScreenItem
description: Representa um item na tela inicial do iOS
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ff573a6f7ae0d78113a32514bc312c3920b216f1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987619"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="87ce8-103">Tipo de recurso iosHomeScreenItem</span><span class="sxs-lookup"><span data-stu-id="87ce8-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="87ce8-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="87ce8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87ce8-105">Representa um item na tela inicial do iOS</span><span class="sxs-lookup"><span data-stu-id="87ce8-105">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="87ce8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87ce8-106">Properties</span></span>
|<span data-ttu-id="87ce8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87ce8-107">Property</span></span>|<span data-ttu-id="87ce8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="87ce8-108">Type</span></span>|<span data-ttu-id="87ce8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="87ce8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87ce8-110">displayName</span><span class="sxs-lookup"><span data-stu-id="87ce8-110">displayName</span></span>|<span data-ttu-id="87ce8-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="87ce8-111">String</span></span>|<span data-ttu-id="87ce8-112">Nome do aplicativo</span><span class="sxs-lookup"><span data-stu-id="87ce8-112">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="87ce8-113">Relações</span><span class="sxs-lookup"><span data-stu-id="87ce8-113">Relationships</span></span>
<span data-ttu-id="87ce8-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="87ce8-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="87ce8-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87ce8-115">JSON Representation</span></span>
<span data-ttu-id="87ce8-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="87ce8-116">Here is a JSON representation of the resource.</span></span>
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



