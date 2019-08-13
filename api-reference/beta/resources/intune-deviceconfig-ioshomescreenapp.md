---
title: Tipo de recurso iosHomeScreenApp
description: Representa um ícone de um aplicativo na tela inicial
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1a491f6dc8dbbdce729bfebb732f94222ef2b03e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357030"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="d39c6-103">Tipo de recurso iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="d39c6-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="d39c6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d39c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d39c6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d39c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d39c6-106">Representa um ícone de um aplicativo na tela inicial</span><span class="sxs-lookup"><span data-stu-id="d39c6-106">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="d39c6-107">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="d39c6-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d39c6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d39c6-108">Properties</span></span>
|<span data-ttu-id="d39c6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d39c6-109">Property</span></span>|<span data-ttu-id="d39c6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d39c6-110">Type</span></span>|<span data-ttu-id="d39c6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d39c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d39c6-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d39c6-112">displayName</span></span>|<span data-ttu-id="d39c6-113">String</span><span class="sxs-lookup"><span data-stu-id="d39c6-113">String</span></span>|<span data-ttu-id="d39c6-114">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="d39c6-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="d39c6-115">bundleID</span><span class="sxs-lookup"><span data-stu-id="d39c6-115">bundleID</span></span>|<span data-ttu-id="d39c6-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d39c6-116">String</span></span>|<span data-ttu-id="d39c6-117">BundleID do aplicativo</span><span class="sxs-lookup"><span data-stu-id="d39c6-117">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="d39c6-118">Relações</span><span class="sxs-lookup"><span data-stu-id="d39c6-118">Relationships</span></span>
<span data-ttu-id="d39c6-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d39c6-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d39c6-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d39c6-120">JSON Representation</span></span>
<span data-ttu-id="d39c6-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d39c6-121">Here is a JSON representation of the resource.</span></span>
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



