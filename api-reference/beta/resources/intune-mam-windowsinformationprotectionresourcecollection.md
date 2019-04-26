---
title: Tipo de recurso windowsInformationProtectionResourceCollection
description: Coleção de recursos da Proteção de Informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e5a303ad0b05813a4e44dc2208ff1b8692242d88
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561842"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="6b552-103">Tipo de recurso windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="6b552-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="6b552-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6b552-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b552-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6b552-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b552-106">Coleção de recursos da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="6b552-106">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="6b552-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b552-107">Properties</span></span>
|<span data-ttu-id="6b552-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b552-108">Property</span></span>|<span data-ttu-id="6b552-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b552-109">Type</span></span>|<span data-ttu-id="6b552-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b552-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b552-111">displayName</span><span class="sxs-lookup"><span data-stu-id="6b552-111">displayName</span></span>|<span data-ttu-id="6b552-112">String</span><span class="sxs-lookup"><span data-stu-id="6b552-112">String</span></span>|<span data-ttu-id="6b552-113">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="6b552-113">Display name</span></span>|
|<span data-ttu-id="6b552-114">recursos</span><span class="sxs-lookup"><span data-stu-id="6b552-114">resources</span></span>|<span data-ttu-id="6b552-115">String collection</span><span class="sxs-lookup"><span data-stu-id="6b552-115">String collection</span></span>|<span data-ttu-id="6b552-116">Coleção de recursos</span><span class="sxs-lookup"><span data-stu-id="6b552-116">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b552-117">Relações</span><span class="sxs-lookup"><span data-stu-id="6b552-117">Relationships</span></span>
<span data-ttu-id="6b552-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b552-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b552-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b552-119">JSON Representation</span></span>
<span data-ttu-id="6b552-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6b552-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```





