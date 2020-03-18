---
title: tipo de recurso configurationManagerClientInformation
description: Informações do cliente do Configuration Manager sincronizadas a partir do SCCM
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c1c9e9b88677c925fb33c998af571b23090dcff5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785053"
---
# <a name="configurationmanagerclientinformation-resource-type"></a><span data-ttu-id="6dda4-103">tipo de recurso configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="6dda4-103">configurationManagerClientInformation resource type</span></span>

> <span data-ttu-id="6dda4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6dda4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6dda4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6dda4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6dda4-106">Informações do cliente do Configuration Manager sincronizadas a partir do SCCM</span><span class="sxs-lookup"><span data-stu-id="6dda4-106">Configuration Manager client information synced from SCCM</span></span>

## <a name="properties"></a><span data-ttu-id="6dda4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6dda4-107">Properties</span></span>
|<span data-ttu-id="6dda4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6dda4-108">Property</span></span>|<span data-ttu-id="6dda4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6dda4-109">Type</span></span>|<span data-ttu-id="6dda4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6dda4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dda4-111">clientIdentifier</span><span class="sxs-lookup"><span data-stu-id="6dda4-111">clientIdentifier</span></span>|<span data-ttu-id="6dda4-112">String</span><span class="sxs-lookup"><span data-stu-id="6dda4-112">String</span></span>|<span data-ttu-id="6dda4-113">ID do cliente do Gerenciador de configurações do SCCM</span><span class="sxs-lookup"><span data-stu-id="6dda4-113">Configuration Manager Client Id from SCCM</span></span>|
|<span data-ttu-id="6dda4-114">IsBlocked</span><span class="sxs-lookup"><span data-stu-id="6dda4-114">isBlocked</span></span>|<span data-ttu-id="6dda4-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="6dda4-115">Boolean</span></span>|<span data-ttu-id="6dda4-116">Status bloqueado do cliente do Gerenciador de configurações do SCCM</span><span class="sxs-lookup"><span data-stu-id="6dda4-116">Configuration Manager Client blocked status from SCCM</span></span>|

## <a name="relationships"></a><span data-ttu-id="6dda4-117">Relações</span><span class="sxs-lookup"><span data-stu-id="6dda4-117">Relationships</span></span>
<span data-ttu-id="6dda4-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6dda4-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6dda4-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6dda4-119">JSON Representation</span></span>
<span data-ttu-id="6dda4-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6dda4-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientInformation",
  "clientIdentifier": "String",
  "isBlocked": true
}
```



