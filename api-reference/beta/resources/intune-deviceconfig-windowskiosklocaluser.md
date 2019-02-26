---
title: tipo de recurso windowsKioskLocalUser
description: A classe usada para identificar uma conta local para a configuração do quiosque
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 94b2397a8bb1a3825af97c5d22f273f622500359
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173196"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="d464b-103">tipo de recurso windowsKioskLocalUser</span><span class="sxs-lookup"><span data-stu-id="d464b-103">windowsKioskLocalUser resource type</span></span>

> <span data-ttu-id="d464b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d464b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d464b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d464b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d464b-106">A classe usada para identificar uma conta local para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="d464b-106">The class used to identify a local account for the kiosk configuration</span></span>


<span data-ttu-id="d464b-107">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="d464b-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d464b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d464b-108">Properties</span></span>
|<span data-ttu-id="d464b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d464b-109">Property</span></span>|<span data-ttu-id="d464b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d464b-110">Type</span></span>|<span data-ttu-id="d464b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d464b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d464b-112">userName</span><span class="sxs-lookup"><span data-stu-id="d464b-112">userName</span></span>|<span data-ttu-id="d464b-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d464b-113">String</span></span>|<span data-ttu-id="d464b-114">O usuário local que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="d464b-114">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="d464b-115">Relações</span><span class="sxs-lookup"><span data-stu-id="d464b-115">Relationships</span></span>
<span data-ttu-id="d464b-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d464b-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d464b-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d464b-117">JSON Representation</span></span>
<span data-ttu-id="d464b-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d464b-118">Here is a JSON representation of the resource.</span></span>
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




