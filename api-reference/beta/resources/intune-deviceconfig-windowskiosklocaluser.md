---
title: tipo de recurso windowsKioskLocalUser
description: A classe usada para identificar uma conta local para a configuração do quiosque
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: daa1899e5cbb4215053dd84fc09b5c3b5b4730fc
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995410"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="c7b2b-103">tipo de recurso windowsKioskLocalUser</span><span class="sxs-lookup"><span data-stu-id="c7b2b-103">windowsKioskLocalUser resource type</span></span>

> <span data-ttu-id="c7b2b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c7b2b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7b2b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c7b2b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7b2b-106">A classe usada para identificar uma conta local para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="c7b2b-106">The class used to identify a local account for the kiosk configuration</span></span>


<span data-ttu-id="c7b2b-107">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="c7b2b-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c7b2b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7b2b-108">Properties</span></span>
|<span data-ttu-id="c7b2b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7b2b-109">Property</span></span>|<span data-ttu-id="c7b2b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7b2b-110">Type</span></span>|<span data-ttu-id="c7b2b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7b2b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7b2b-112">userName</span><span class="sxs-lookup"><span data-stu-id="c7b2b-112">userName</span></span>|<span data-ttu-id="c7b2b-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7b2b-113">String</span></span>|<span data-ttu-id="c7b2b-114">O usuário local que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="c7b2b-114">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7b2b-115">Relações</span><span class="sxs-lookup"><span data-stu-id="c7b2b-115">Relationships</span></span>
<span data-ttu-id="c7b2b-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c7b2b-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7b2b-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7b2b-117">JSON Representation</span></span>
<span data-ttu-id="c7b2b-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7b2b-118">Here is a JSON representation of the resource.</span></span>
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





