---
title: tipo de recurso windowsKioskLocalUser
description: A classe usada para identificar uma conta local para a configuração do quiosque
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d3f46b47de9d3ce09c6a7d33a4b663cb64f506cc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969006"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="b797f-103">tipo de recurso windowsKioskLocalUser</span><span class="sxs-lookup"><span data-stu-id="b797f-103">windowsKioskLocalUser resource type</span></span>

> <span data-ttu-id="b797f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b797f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b797f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b797f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b797f-106">A classe usada para identificar uma conta local para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="b797f-106">The class used to identify a local account for the kiosk configuration</span></span>


<span data-ttu-id="b797f-107">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="b797f-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b797f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b797f-108">Properties</span></span>
|<span data-ttu-id="b797f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b797f-109">Property</span></span>|<span data-ttu-id="b797f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b797f-110">Type</span></span>|<span data-ttu-id="b797f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b797f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b797f-112">userName</span><span class="sxs-lookup"><span data-stu-id="b797f-112">userName</span></span>|<span data-ttu-id="b797f-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b797f-113">String</span></span>|<span data-ttu-id="b797f-114">O usuário local que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="b797f-114">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="b797f-115">Relações</span><span class="sxs-lookup"><span data-stu-id="b797f-115">Relationships</span></span>
<span data-ttu-id="b797f-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b797f-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b797f-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b797f-117">JSON Representation</span></span>
<span data-ttu-id="b797f-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b797f-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalUser",
  "userName": "String"
}
```





