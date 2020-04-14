---
title: tipo de recurso configurationManagerClientInformation
description: Informações do cliente do Configuration Manager sincronizadas a partir do SCCM
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 725847d0150a886ed11ce6d68cd49138711ede0f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465019"
---
# <a name="configurationmanagerclientinformation-resource-type"></a><span data-ttu-id="50e3e-103">tipo de recurso configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="50e3e-103">configurationManagerClientInformation resource type</span></span>

<span data-ttu-id="50e3e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50e3e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50e3e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="50e3e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50e3e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50e3e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50e3e-107">Informações do cliente do Configuration Manager sincronizadas a partir do SCCM</span><span class="sxs-lookup"><span data-stu-id="50e3e-107">Configuration Manager client information synced from SCCM</span></span>

## <a name="properties"></a><span data-ttu-id="50e3e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50e3e-108">Properties</span></span>
|<span data-ttu-id="50e3e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50e3e-109">Property</span></span>|<span data-ttu-id="50e3e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="50e3e-110">Type</span></span>|<span data-ttu-id="50e3e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="50e3e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50e3e-112">clientIdentifier</span><span class="sxs-lookup"><span data-stu-id="50e3e-112">clientIdentifier</span></span>|<span data-ttu-id="50e3e-113">String</span><span class="sxs-lookup"><span data-stu-id="50e3e-113">String</span></span>|<span data-ttu-id="50e3e-114">ID do cliente do Gerenciador de configurações do SCCM</span><span class="sxs-lookup"><span data-stu-id="50e3e-114">Configuration Manager Client Id from SCCM</span></span>|
|<span data-ttu-id="50e3e-115">IsBlocked</span><span class="sxs-lookup"><span data-stu-id="50e3e-115">isBlocked</span></span>|<span data-ttu-id="50e3e-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="50e3e-116">Boolean</span></span>|<span data-ttu-id="50e3e-117">Status bloqueado do cliente do Gerenciador de configurações do SCCM</span><span class="sxs-lookup"><span data-stu-id="50e3e-117">Configuration Manager Client blocked status from SCCM</span></span>|

## <a name="relationships"></a><span data-ttu-id="50e3e-118">Relações</span><span class="sxs-lookup"><span data-stu-id="50e3e-118">Relationships</span></span>
<span data-ttu-id="50e3e-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="50e3e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50e3e-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50e3e-120">JSON Representation</span></span>
<span data-ttu-id="50e3e-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="50e3e-121">Here is a JSON representation of the resource.</span></span>
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



