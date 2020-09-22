---
title: tipo de recurso windowsKioskLocalUser
description: A classe usada para identificar uma conta local para a configuração do quiosque
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 22db475ecb8cda48d4d73cba8ecb2145ae24a03a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061935"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="db5d0-103">tipo de recurso windowsKioskLocalUser</span><span class="sxs-lookup"><span data-stu-id="db5d0-103">windowsKioskLocalUser resource type</span></span>

<span data-ttu-id="db5d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db5d0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db5d0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="db5d0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db5d0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="db5d0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db5d0-107">A classe usada para identificar uma conta local para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="db5d0-107">The class used to identify a local account for the kiosk configuration</span></span>


<span data-ttu-id="db5d0-108">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="db5d0-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="db5d0-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="db5d0-109">Properties</span></span>
|<span data-ttu-id="db5d0-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db5d0-110">Property</span></span>|<span data-ttu-id="db5d0-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="db5d0-111">Type</span></span>|<span data-ttu-id="db5d0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="db5d0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db5d0-113">userName</span><span class="sxs-lookup"><span data-stu-id="db5d0-113">userName</span></span>|<span data-ttu-id="db5d0-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db5d0-114">String</span></span>|<span data-ttu-id="db5d0-115">O usuário local que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="db5d0-115">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="db5d0-116">Relações</span><span class="sxs-lookup"><span data-stu-id="db5d0-116">Relationships</span></span>
<span data-ttu-id="db5d0-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="db5d0-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="db5d0-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="db5d0-118">JSON Representation</span></span>
<span data-ttu-id="db5d0-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="db5d0-119">Here is a JSON representation of the resource.</span></span>
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






