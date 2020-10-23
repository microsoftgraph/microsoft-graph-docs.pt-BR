---
title: tipo de recurso macOSSystemExtension
description: Representa uma extensão de sistema macOS específica.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 45d6b8a86b3aafa8819dd889ac06acc40d498176
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690662"
---
# <a name="macossystemextension-resource-type"></a><span data-ttu-id="01f5b-103">tipo de recurso macOSSystemExtension</span><span class="sxs-lookup"><span data-stu-id="01f5b-103">macOSSystemExtension resource type</span></span>

<span data-ttu-id="01f5b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01f5b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01f5b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="01f5b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01f5b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="01f5b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01f5b-107">Representa uma extensão de sistema macOS específica.</span><span class="sxs-lookup"><span data-stu-id="01f5b-107">Represents a specific macOS system extension.</span></span>

## <a name="properties"></a><span data-ttu-id="01f5b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="01f5b-108">Properties</span></span>
|<span data-ttu-id="01f5b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01f5b-109">Property</span></span>|<span data-ttu-id="01f5b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="01f5b-110">Type</span></span>|<span data-ttu-id="01f5b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="01f5b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01f5b-112">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="01f5b-112">teamIdentifier</span></span>|<span data-ttu-id="01f5b-113">String</span><span class="sxs-lookup"><span data-stu-id="01f5b-113">String</span></span>|<span data-ttu-id="01f5b-114">Obtém ou define o identificador de equipe que foi usado para assinar a extensão do sistema.</span><span class="sxs-lookup"><span data-stu-id="01f5b-114">Gets or sets the team identifier that was used to sign the system extension.</span></span>|
|<span data-ttu-id="01f5b-115">bundleId</span><span class="sxs-lookup"><span data-stu-id="01f5b-115">bundleId</span></span>|<span data-ttu-id="01f5b-116">String</span><span class="sxs-lookup"><span data-stu-id="01f5b-116">String</span></span>|<span data-ttu-id="01f5b-117">Obtém ou define o identificador de pacote da extensão do sistema.</span><span class="sxs-lookup"><span data-stu-id="01f5b-117">Gets or sets the bundle identifier of the system extension.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01f5b-118">Relações</span><span class="sxs-lookup"><span data-stu-id="01f5b-118">Relationships</span></span>
<span data-ttu-id="01f5b-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="01f5b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="01f5b-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="01f5b-120">JSON Representation</span></span>
<span data-ttu-id="01f5b-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="01f5b-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSSystemExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSystemExtension",
  "teamIdentifier": "String",
  "bundleId": "String"
}
```





