---
title: Tipo de recurso iosHomeScreenItem
description: Representa um item na tela inicial do iOS
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 477be5c509ab4d062a695c4b8df7eb00af6f51fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962601"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="886d6-103">Tipo de recurso iosHomeScreenItem</span><span class="sxs-lookup"><span data-stu-id="886d6-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="886d6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="886d6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="886d6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="886d6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="886d6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="886d6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="886d6-107">Representa um item na tela inicial do iOS</span><span class="sxs-lookup"><span data-stu-id="886d6-107">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="886d6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="886d6-108">Properties</span></span>
|<span data-ttu-id="886d6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="886d6-109">Property</span></span>|<span data-ttu-id="886d6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="886d6-110">Type</span></span>|<span data-ttu-id="886d6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="886d6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="886d6-112">displayName</span><span class="sxs-lookup"><span data-stu-id="886d6-112">displayName</span></span>|<span data-ttu-id="886d6-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="886d6-113">String</span></span>|<span data-ttu-id="886d6-114">Nome do aplicativo</span><span class="sxs-lookup"><span data-stu-id="886d6-114">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="886d6-115">Relações</span><span class="sxs-lookup"><span data-stu-id="886d6-115">Relationships</span></span>
<span data-ttu-id="886d6-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="886d6-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="886d6-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="886d6-117">JSON Representation</span></span>
<span data-ttu-id="886d6-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="886d6-118">Here is a JSON representation of the resource.</span></span>
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





