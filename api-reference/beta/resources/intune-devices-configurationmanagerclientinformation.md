---
title: tipo de recurso configurationManagerClientInformation
description: Informações do cliente do Configuration Manager sincronizadas a partir do SCCM
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 22844c063bb119d956740045c088be4fad59f89d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060633"
---
# <a name="configurationmanagerclientinformation-resource-type"></a><span data-ttu-id="7c2b7-103">tipo de recurso configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="7c2b7-103">configurationManagerClientInformation resource type</span></span>

<span data-ttu-id="7c2b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c2b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c2b7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7c2b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c2b7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7c2b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c2b7-107">Informações do cliente do Configuration Manager sincronizadas a partir do SCCM</span><span class="sxs-lookup"><span data-stu-id="7c2b7-107">Configuration Manager client information synced from SCCM</span></span>

## <a name="properties"></a><span data-ttu-id="7c2b7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7c2b7-108">Properties</span></span>
|<span data-ttu-id="7c2b7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c2b7-109">Property</span></span>|<span data-ttu-id="7c2b7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c2b7-110">Type</span></span>|<span data-ttu-id="7c2b7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c2b7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c2b7-112">clientIdentifier</span><span class="sxs-lookup"><span data-stu-id="7c2b7-112">clientIdentifier</span></span>|<span data-ttu-id="7c2b7-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c2b7-113">String</span></span>|<span data-ttu-id="7c2b7-114">ID do cliente do Gerenciador de configurações do SCCM</span><span class="sxs-lookup"><span data-stu-id="7c2b7-114">Configuration Manager Client Id from SCCM</span></span>|
|<span data-ttu-id="7c2b7-115">IsBlocked</span><span class="sxs-lookup"><span data-stu-id="7c2b7-115">isBlocked</span></span>|<span data-ttu-id="7c2b7-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="7c2b7-116">Boolean</span></span>|<span data-ttu-id="7c2b7-117">Status bloqueado do cliente do Gerenciador de configurações do SCCM</span><span class="sxs-lookup"><span data-stu-id="7c2b7-117">Configuration Manager Client blocked status from SCCM</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c2b7-118">Relações</span><span class="sxs-lookup"><span data-stu-id="7c2b7-118">Relationships</span></span>
<span data-ttu-id="7c2b7-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7c2b7-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c2b7-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7c2b7-120">JSON Representation</span></span>
<span data-ttu-id="7c2b7-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7c2b7-121">Here is a JSON representation of the resource.</span></span>
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






