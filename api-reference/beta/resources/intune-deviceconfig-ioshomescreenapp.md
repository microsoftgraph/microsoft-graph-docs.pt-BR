---
title: Tipo de recurso iosHomeScreenApp
description: Representa um ícone de um aplicativo na tela inicial
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 39db8de19fbfc568f85c4930e8c3124ffea2dd57
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850593"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="ed278-103">Tipo de recurso iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="ed278-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="ed278-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ed278-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed278-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ed278-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed278-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ed278-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed278-107">Representa um ícone de um aplicativo na tela inicial</span><span class="sxs-lookup"><span data-stu-id="ed278-107">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="ed278-108">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="ed278-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ed278-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed278-109">Properties</span></span>
|<span data-ttu-id="ed278-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed278-110">Property</span></span>|<span data-ttu-id="ed278-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed278-111">Type</span></span>|<span data-ttu-id="ed278-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed278-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed278-113">displayName</span><span class="sxs-lookup"><span data-stu-id="ed278-113">displayName</span></span>|<span data-ttu-id="ed278-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed278-114">String</span></span>|<span data-ttu-id="ed278-115">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="ed278-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="ed278-116">bundleID</span><span class="sxs-lookup"><span data-stu-id="ed278-116">bundleID</span></span>|<span data-ttu-id="ed278-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed278-117">String</span></span>|<span data-ttu-id="ed278-118">BundleID do aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed278-118">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed278-119">Relações</span><span class="sxs-lookup"><span data-stu-id="ed278-119">Relationships</span></span>
<span data-ttu-id="ed278-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ed278-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ed278-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed278-121">JSON Representation</span></span>
<span data-ttu-id="ed278-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed278-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```





