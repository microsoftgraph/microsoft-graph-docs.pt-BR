---
title: tipo de recurso configurationManagerClientInformation
description: Informações do cliente do Configuration Manager sincronizadas a partir do SCCM
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 67c1a4b4a9ac570b4acd71a1ce819f9705fd32e3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528673"
---
# <a name="configurationmanagerclientinformation-resource-type"></a><span data-ttu-id="efbaf-103">tipo de recurso configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="efbaf-103">configurationManagerClientInformation resource type</span></span>

<span data-ttu-id="efbaf-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="efbaf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="efbaf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="efbaf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efbaf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="efbaf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efbaf-107">Informações do cliente do Configuration Manager sincronizadas a partir do SCCM</span><span class="sxs-lookup"><span data-stu-id="efbaf-107">Configuration Manager client information synced from SCCM</span></span>

## <a name="properties"></a><span data-ttu-id="efbaf-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="efbaf-108">Properties</span></span>
|<span data-ttu-id="efbaf-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="efbaf-109">Property</span></span>|<span data-ttu-id="efbaf-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="efbaf-110">Type</span></span>|<span data-ttu-id="efbaf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="efbaf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efbaf-112">clientIdentifier</span><span class="sxs-lookup"><span data-stu-id="efbaf-112">clientIdentifier</span></span>|<span data-ttu-id="efbaf-113">String</span><span class="sxs-lookup"><span data-stu-id="efbaf-113">String</span></span>|<span data-ttu-id="efbaf-114">ID do cliente do Gerenciador de configurações do SCCM</span><span class="sxs-lookup"><span data-stu-id="efbaf-114">Configuration Manager Client Id from SCCM</span></span>|

## <a name="relationships"></a><span data-ttu-id="efbaf-115">Relações</span><span class="sxs-lookup"><span data-stu-id="efbaf-115">Relationships</span></span>
<span data-ttu-id="efbaf-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="efbaf-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="efbaf-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="efbaf-117">JSON Representation</span></span>
<span data-ttu-id="efbaf-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="efbaf-118">Here is a JSON representation of the resource.</span></span>
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



