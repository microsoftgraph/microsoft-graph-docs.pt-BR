---
title: Tipo de recurso iosHomeScreenApp
description: Representa um ícone de um aplicativo na tela inicial
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 858ce1825ab09709f412aeee978dc53a47a0d0af
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455166"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="5c31d-103">Tipo de recurso iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="5c31d-103">iosHomeScreenApp resource type</span></span>

<span data-ttu-id="5c31d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c31d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c31d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5c31d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c31d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5c31d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c31d-107">Representa um ícone de um aplicativo na tela inicial</span><span class="sxs-lookup"><span data-stu-id="5c31d-107">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="5c31d-108">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="5c31d-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5c31d-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5c31d-109">Properties</span></span>
|<span data-ttu-id="5c31d-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c31d-110">Property</span></span>|<span data-ttu-id="5c31d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c31d-111">Type</span></span>|<span data-ttu-id="5c31d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c31d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c31d-113">displayName</span><span class="sxs-lookup"><span data-stu-id="5c31d-113">displayName</span></span>|<span data-ttu-id="5c31d-114">String</span><span class="sxs-lookup"><span data-stu-id="5c31d-114">String</span></span>|<span data-ttu-id="5c31d-115">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="5c31d-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="5c31d-116">bundleID</span><span class="sxs-lookup"><span data-stu-id="5c31d-116">bundleID</span></span>|<span data-ttu-id="5c31d-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c31d-117">String</span></span>|<span data-ttu-id="5c31d-118">BundleID do aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c31d-118">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c31d-119">Relações</span><span class="sxs-lookup"><span data-stu-id="5c31d-119">Relationships</span></span>
<span data-ttu-id="5c31d-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5c31d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c31d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5c31d-121">JSON Representation</span></span>
<span data-ttu-id="5c31d-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5c31d-122">Here is a JSON representation of the resource.</span></span>
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



