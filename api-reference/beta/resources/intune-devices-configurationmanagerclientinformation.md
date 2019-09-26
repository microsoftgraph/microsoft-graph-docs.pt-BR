---
title: tipo de recurso configurationManagerClientInformation
description: Informações do cliente do Configuration Manager sincronizadas a partir do SCCM
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b329d017aaf9f7d26d76f74198b2c5508e97ae2c
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196977"
---
# <a name="configurationmanagerclientinformation-resource-type"></a><span data-ttu-id="5f548-103">tipo de recurso configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="5f548-103">configurationManagerClientInformation resource type</span></span>

> <span data-ttu-id="5f548-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5f548-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f548-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5f548-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f548-106">Informações do cliente do Configuration Manager sincronizadas a partir do SCCM</span><span class="sxs-lookup"><span data-stu-id="5f548-106">Configuration Manager client information synced from SCCM</span></span>

## <a name="properties"></a><span data-ttu-id="5f548-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5f548-107">Properties</span></span>
|<span data-ttu-id="5f548-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f548-108">Property</span></span>|<span data-ttu-id="5f548-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f548-109">Type</span></span>|<span data-ttu-id="5f548-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f548-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f548-111">clientIdentifier</span><span class="sxs-lookup"><span data-stu-id="5f548-111">clientIdentifier</span></span>|<span data-ttu-id="5f548-112">String</span><span class="sxs-lookup"><span data-stu-id="5f548-112">String</span></span>|<span data-ttu-id="5f548-113">ID do cliente do Gerenciador de configurações do SCCM</span><span class="sxs-lookup"><span data-stu-id="5f548-113">Configuration Manager Client Id from SCCM</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f548-114">Relações</span><span class="sxs-lookup"><span data-stu-id="5f548-114">Relationships</span></span>
<span data-ttu-id="5f548-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5f548-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f548-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5f548-116">JSON Representation</span></span>
<span data-ttu-id="5f548-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5f548-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientInformation",
  "clientIdentifier": "String"
}
```



