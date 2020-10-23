---
title: tipo de recurso macOSSystemExtensionTypeMapping
description: Representa um mapeamento entre identificadores de equipe para extensões de sistema macOS e tipos de extensão de sistema.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8dc0aada94c3ab13cf488bb6cca6ba0f7057c1da
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735250"
---
# <a name="macossystemextensiontypemapping-resource-type"></a><span data-ttu-id="f7d67-103">tipo de recurso macOSSystemExtensionTypeMapping</span><span class="sxs-lookup"><span data-stu-id="f7d67-103">macOSSystemExtensionTypeMapping resource type</span></span>

<span data-ttu-id="f7d67-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7d67-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7d67-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f7d67-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7d67-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f7d67-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7d67-107">Representa um mapeamento entre identificadores de equipe para extensões de sistema macOS e tipos de extensão de sistema.</span><span class="sxs-lookup"><span data-stu-id="f7d67-107">Represents a mapping between team identifiers for macOS system extensions and system extension types.</span></span>

## <a name="properties"></a><span data-ttu-id="f7d67-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f7d67-108">Properties</span></span>
|<span data-ttu-id="f7d67-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7d67-109">Property</span></span>|<span data-ttu-id="f7d67-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7d67-110">Type</span></span>|<span data-ttu-id="f7d67-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7d67-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7d67-112">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="f7d67-112">teamIdentifier</span></span>|<span data-ttu-id="f7d67-113">String</span><span class="sxs-lookup"><span data-stu-id="f7d67-113">String</span></span>|<span data-ttu-id="f7d67-114">Obtém ou define o identificador de equipe usado para assinar a extensão do sistema.</span><span class="sxs-lookup"><span data-stu-id="f7d67-114">Gets or sets the team identifier used to sign the system extension.</span></span>|
|<span data-ttu-id="f7d67-115">allowedTypes</span><span class="sxs-lookup"><span data-stu-id="f7d67-115">allowedTypes</span></span>|[<span data-ttu-id="f7d67-116">macOSSystemExtensionType</span><span class="sxs-lookup"><span data-stu-id="f7d67-116">macOSSystemExtensionType</span></span>](../resources/intune-deviceconfig-macossystemextensiontype.md)|<span data-ttu-id="f7d67-117">Obtém ou define os tipos de extensões de sistema macOS permitidos.</span><span class="sxs-lookup"><span data-stu-id="f7d67-117">Gets or sets the allowed macOS system extension types.</span></span> <span data-ttu-id="f7d67-118">Os valores possíveis são: `driverExtensionsAllowed`, `networkExtensionsAllowed`, `endpointSecurityExtensionsAllowed`.</span><span class="sxs-lookup"><span data-stu-id="f7d67-118">Possible values are: `driverExtensionsAllowed`, `networkExtensionsAllowed`, `endpointSecurityExtensionsAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7d67-119">Relações</span><span class="sxs-lookup"><span data-stu-id="f7d67-119">Relationships</span></span>
<span data-ttu-id="f7d67-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f7d67-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7d67-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f7d67-121">JSON Representation</span></span>
<span data-ttu-id="f7d67-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f7d67-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSSystemExtensionTypeMapping"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSystemExtensionTypeMapping",
  "teamIdentifier": "String",
  "allowedTypes": "String"
}
```





