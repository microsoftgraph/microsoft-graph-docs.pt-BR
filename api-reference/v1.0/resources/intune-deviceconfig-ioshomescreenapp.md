---
title: Tipo de recurso iosHomeScreenApp
description: Representa um ícone de um aplicativo na tela inicial
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bb63950229f88fb9987e75f42abfbe39793864ad
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845693"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="0df66-103">Tipo de recurso iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="0df66-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="0df66-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0df66-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0df66-105">Representa um ícone de um aplicativo na tela inicial</span><span class="sxs-lookup"><span data-stu-id="0df66-105">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="0df66-106">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="0df66-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0df66-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0df66-107">Properties</span></span>
|<span data-ttu-id="0df66-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0df66-108">Property</span></span>|<span data-ttu-id="0df66-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0df66-109">Type</span></span>|<span data-ttu-id="0df66-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0df66-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0df66-111">displayName</span><span class="sxs-lookup"><span data-stu-id="0df66-111">displayName</span></span>|<span data-ttu-id="0df66-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0df66-112">String</span></span>|<span data-ttu-id="0df66-113">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="0df66-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="0df66-114">bundleID</span><span class="sxs-lookup"><span data-stu-id="0df66-114">bundleID</span></span>|<span data-ttu-id="0df66-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0df66-115">String</span></span>|<span data-ttu-id="0df66-116">BundleID do aplicativo</span><span class="sxs-lookup"><span data-stu-id="0df66-116">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="0df66-117">Relações</span><span class="sxs-lookup"><span data-stu-id="0df66-117">Relationships</span></span>
<span data-ttu-id="0df66-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0df66-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0df66-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0df66-119">JSON Representation</span></span>
<span data-ttu-id="0df66-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0df66-120">Here is a JSON representation of the resource.</span></span>
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



