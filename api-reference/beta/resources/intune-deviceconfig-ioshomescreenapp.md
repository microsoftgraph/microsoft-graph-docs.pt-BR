---
title: Tipo de recurso iosHomeScreenApp
description: Representa um ícone de um aplicativo na tela inicial
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c26f1237061914e66653509cd22b734fef854f27
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993914"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="59270-103">Tipo de recurso iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="59270-103">iosHomeScreenApp resource type</span></span>

<span data-ttu-id="59270-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59270-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="59270-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="59270-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59270-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="59270-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59270-107">Representa um ícone de um aplicativo na tela inicial</span><span class="sxs-lookup"><span data-stu-id="59270-107">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="59270-108">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="59270-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="59270-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="59270-109">Properties</span></span>
|<span data-ttu-id="59270-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59270-110">Property</span></span>|<span data-ttu-id="59270-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="59270-111">Type</span></span>|<span data-ttu-id="59270-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="59270-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59270-113">displayName</span><span class="sxs-lookup"><span data-stu-id="59270-113">displayName</span></span>|<span data-ttu-id="59270-114">String</span><span class="sxs-lookup"><span data-stu-id="59270-114">String</span></span>|<span data-ttu-id="59270-115">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="59270-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="59270-116">bundleID</span><span class="sxs-lookup"><span data-stu-id="59270-116">bundleID</span></span>|<span data-ttu-id="59270-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59270-117">String</span></span>|<span data-ttu-id="59270-118">BundleID do aplicativo</span><span class="sxs-lookup"><span data-stu-id="59270-118">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="59270-119">Relações</span><span class="sxs-lookup"><span data-stu-id="59270-119">Relationships</span></span>
<span data-ttu-id="59270-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="59270-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="59270-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="59270-121">JSON Representation</span></span>
<span data-ttu-id="59270-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="59270-122">Here is a JSON representation of the resource.</span></span>
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






