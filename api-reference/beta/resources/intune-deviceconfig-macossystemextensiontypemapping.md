---
title: tipo de recurso macOSSystemExtensionTypeMapping
description: Representa um mapeamento entre identificadores de equipe para extensões de sistema macOS e tipos de extensão de sistema.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cd22cc58d3d949c1e560d62e672e27fb31ae913e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279777"
---
# <a name="macossystemextensiontypemapping-resource-type"></a><span data-ttu-id="7de9d-103">tipo de recurso macOSSystemExtensionTypeMapping</span><span class="sxs-lookup"><span data-stu-id="7de9d-103">macOSSystemExtensionTypeMapping resource type</span></span>

<span data-ttu-id="7de9d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7de9d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7de9d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7de9d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7de9d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7de9d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7de9d-107">Representa um mapeamento entre identificadores de equipe para extensões de sistema macOS e tipos de extensão de sistema.</span><span class="sxs-lookup"><span data-stu-id="7de9d-107">Represents a mapping between team identifiers for macOS system extensions and system extension types.</span></span>

## <a name="properties"></a><span data-ttu-id="7de9d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7de9d-108">Properties</span></span>
|<span data-ttu-id="7de9d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7de9d-109">Property</span></span>|<span data-ttu-id="7de9d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7de9d-110">Type</span></span>|<span data-ttu-id="7de9d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7de9d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7de9d-112">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="7de9d-112">teamIdentifier</span></span>|<span data-ttu-id="7de9d-113">String</span><span class="sxs-lookup"><span data-stu-id="7de9d-113">String</span></span>|<span data-ttu-id="7de9d-114">Obtém ou define o identificador de equipe usado para assinar a extensão do sistema.</span><span class="sxs-lookup"><span data-stu-id="7de9d-114">Gets or sets the team identifier used to sign the system extension.</span></span>|
|<span data-ttu-id="7de9d-115">allowedTypes</span><span class="sxs-lookup"><span data-stu-id="7de9d-115">allowedTypes</span></span>|[<span data-ttu-id="7de9d-116">macOSSystemExtensionType</span><span class="sxs-lookup"><span data-stu-id="7de9d-116">macOSSystemExtensionType</span></span>](../resources/intune-deviceconfig-macossystemextensiontype.md)|<span data-ttu-id="7de9d-117">Obtém ou define os tipos de extensões de sistema macOS permitidos.</span><span class="sxs-lookup"><span data-stu-id="7de9d-117">Gets or sets the allowed macOS system extension types.</span></span> <span data-ttu-id="7de9d-118">Os valores possíveis são: `driverExtensionsAllowed`, `networkExtensionsAllowed`, `endpointSecurityExtensionsAllowed`.</span><span class="sxs-lookup"><span data-stu-id="7de9d-118">Possible values are: `driverExtensionsAllowed`, `networkExtensionsAllowed`, `endpointSecurityExtensionsAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7de9d-119">Relações</span><span class="sxs-lookup"><span data-stu-id="7de9d-119">Relationships</span></span>
<span data-ttu-id="7de9d-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7de9d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7de9d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7de9d-121">JSON Representation</span></span>
<span data-ttu-id="7de9d-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7de9d-122">Here is a JSON representation of the resource.</span></span>
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




