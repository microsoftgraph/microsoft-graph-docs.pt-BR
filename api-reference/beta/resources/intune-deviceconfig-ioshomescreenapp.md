---
title: Tipo de recurso iosHomeScreenApp
description: Representa um ícone de um aplicativo na tela inicial
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 24c21b6260800250daa768df0684298f3bb142ae
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161821"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="3db6c-103">Tipo de recurso iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="3db6c-103">iosHomeScreenApp resource type</span></span>

<span data-ttu-id="3db6c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3db6c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3db6c-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3db6c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3db6c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3db6c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3db6c-107">Representa um ícone de um aplicativo na tela inicial</span><span class="sxs-lookup"><span data-stu-id="3db6c-107">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="3db6c-108">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="3db6c-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3db6c-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3db6c-109">Properties</span></span>
|<span data-ttu-id="3db6c-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3db6c-110">Property</span></span>|<span data-ttu-id="3db6c-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3db6c-111">Type</span></span>|<span data-ttu-id="3db6c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3db6c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3db6c-113">displayName</span><span class="sxs-lookup"><span data-stu-id="3db6c-113">displayName</span></span>|<span data-ttu-id="3db6c-114">String</span><span class="sxs-lookup"><span data-stu-id="3db6c-114">String</span></span>|<span data-ttu-id="3db6c-115">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="3db6c-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="3db6c-116">bundleID</span><span class="sxs-lookup"><span data-stu-id="3db6c-116">bundleID</span></span>|<span data-ttu-id="3db6c-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3db6c-117">String</span></span>|<span data-ttu-id="3db6c-118">BundleID do aplicativo se isWebClip for false ou a URL de um web clip se isWebClip for verdadeira.</span><span class="sxs-lookup"><span data-stu-id="3db6c-118">BundleID of the app if isWebClip is false or the URL of a web clip if isWebClip is true.</span></span>|
|<span data-ttu-id="3db6c-119">isWebClip</span><span class="sxs-lookup"><span data-stu-id="3db6c-119">isWebClip</span></span>|<span data-ttu-id="3db6c-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="3db6c-120">Boolean</span></span>|<span data-ttu-id="3db6c-121">Quando verdadeiro, a ID do pacote será tratada como uma URL para um web clip.</span><span class="sxs-lookup"><span data-stu-id="3db6c-121">When true, the bundle ID will be handled as a URL for a web clip.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3db6c-122">Relações</span><span class="sxs-lookup"><span data-stu-id="3db6c-122">Relationships</span></span>
<span data-ttu-id="3db6c-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3db6c-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3db6c-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3db6c-124">JSON Representation</span></span>
<span data-ttu-id="3db6c-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3db6c-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String",
  "isWebClip": true
}
```




