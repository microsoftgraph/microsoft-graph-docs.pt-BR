---
title: Tipo de recurso iosHomeScreenApp
description: Representa um ícone de um aplicativo na tela inicial
author: tfitzmac
ms.openlocfilehash: 68fe4e7b5a226422cc0aaf980ac7fb0421a9bfc0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350369"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="96a37-103">Tipo de recurso iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="96a37-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="96a37-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="96a37-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96a37-105">Representa um ícone de um aplicativo na tela inicial</span><span class="sxs-lookup"><span data-stu-id="96a37-105">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="96a37-106">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="96a37-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="96a37-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="96a37-107">Properties</span></span>
|<span data-ttu-id="96a37-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96a37-108">Property</span></span>|<span data-ttu-id="96a37-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="96a37-109">Type</span></span>|<span data-ttu-id="96a37-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="96a37-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96a37-111">displayName</span><span class="sxs-lookup"><span data-stu-id="96a37-111">displayName</span></span>|<span data-ttu-id="96a37-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96a37-112">String</span></span>|<span data-ttu-id="96a37-113">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="96a37-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="96a37-114">bundleID</span><span class="sxs-lookup"><span data-stu-id="96a37-114">bundleID</span></span>|<span data-ttu-id="96a37-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96a37-115">String</span></span>|<span data-ttu-id="96a37-116">BundleID do aplicativo</span><span class="sxs-lookup"><span data-stu-id="96a37-116">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="96a37-117">Relações</span><span class="sxs-lookup"><span data-stu-id="96a37-117">Relationships</span></span>
<span data-ttu-id="96a37-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96a37-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="96a37-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="96a37-119">JSON Representation</span></span>
<span data-ttu-id="96a37-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="96a37-120">Here is a JSON representation of the resource.</span></span>
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



