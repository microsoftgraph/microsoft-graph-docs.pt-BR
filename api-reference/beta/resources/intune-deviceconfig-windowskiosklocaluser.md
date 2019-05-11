---
title: tipo de recurso windowsKioskLocalUser
description: A classe usada para identificar uma conta local para a configuração do quiosque
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0356d07d92c7189efb6907a6cc767972ed42c48c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943806"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="de2b7-103">tipo de recurso windowsKioskLocalUser</span><span class="sxs-lookup"><span data-stu-id="de2b7-103">windowsKioskLocalUser resource type</span></span>

> <span data-ttu-id="de2b7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="de2b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de2b7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="de2b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de2b7-106">A classe usada para identificar uma conta local para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="de2b7-106">The class used to identify a local account for the kiosk configuration</span></span>


<span data-ttu-id="de2b7-107">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="de2b7-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="de2b7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="de2b7-108">Properties</span></span>
|<span data-ttu-id="de2b7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de2b7-109">Property</span></span>|<span data-ttu-id="de2b7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="de2b7-110">Type</span></span>|<span data-ttu-id="de2b7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="de2b7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de2b7-112">userName</span><span class="sxs-lookup"><span data-stu-id="de2b7-112">userName</span></span>|<span data-ttu-id="de2b7-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de2b7-113">String</span></span>|<span data-ttu-id="de2b7-114">O usuário local que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="de2b7-114">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="de2b7-115">Relações</span><span class="sxs-lookup"><span data-stu-id="de2b7-115">Relationships</span></span>
<span data-ttu-id="de2b7-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="de2b7-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="de2b7-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="de2b7-117">JSON Representation</span></span>
<span data-ttu-id="de2b7-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="de2b7-118">Here is a JSON representation of the resource.</span></span>
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




