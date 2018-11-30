---
title: Tipo de recurso iosHomeScreenApp
description: Representa um ícone de um aplicativo na tela inicial
ms.openlocfilehash: ff749f7166da2d20bfd632e0c595b33f7b1e9fad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006182"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="8bbfd-103">Tipo de recurso iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="8bbfd-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="8bbfd-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8bbfd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8bbfd-105">Representa um ícone de um aplicativo na tela inicial</span><span class="sxs-lookup"><span data-stu-id="8bbfd-105">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="8bbfd-106">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="8bbfd-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8bbfd-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8bbfd-107">Properties</span></span>
|<span data-ttu-id="8bbfd-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8bbfd-108">Property</span></span>|<span data-ttu-id="8bbfd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8bbfd-109">Type</span></span>|<span data-ttu-id="8bbfd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bbfd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bbfd-111">displayName</span><span class="sxs-lookup"><span data-stu-id="8bbfd-111">displayName</span></span>|<span data-ttu-id="8bbfd-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8bbfd-112">String</span></span>|<span data-ttu-id="8bbfd-113">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="8bbfd-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="8bbfd-114">bundleID</span><span class="sxs-lookup"><span data-stu-id="8bbfd-114">bundleID</span></span>|<span data-ttu-id="8bbfd-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8bbfd-115">String</span></span>|<span data-ttu-id="8bbfd-116">BundleID do aplicativo</span><span class="sxs-lookup"><span data-stu-id="8bbfd-116">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="8bbfd-117">Relações</span><span class="sxs-lookup"><span data-stu-id="8bbfd-117">Relationships</span></span>
<span data-ttu-id="8bbfd-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8bbfd-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8bbfd-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8bbfd-119">JSON Representation</span></span>
<span data-ttu-id="8bbfd-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8bbfd-120">Here is a JSON representation of the resource.</span></span>
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



