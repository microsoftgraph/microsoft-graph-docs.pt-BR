---
title: tipo de recurso macOSSystemExtensionTypeMapping
description: Representa um mapeamento entre identificadores de equipe para extensões de sistema macOS e tipos de extensão de sistema.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3422cdac178ba22dee07aadb4700e2806eedc7ba
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44179387"
---
# <a name="macossystemextensiontypemapping-resource-type"></a><span data-ttu-id="20359-103">tipo de recurso macOSSystemExtensionTypeMapping</span><span class="sxs-lookup"><span data-stu-id="20359-103">macOSSystemExtensionTypeMapping resource type</span></span>

<span data-ttu-id="20359-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20359-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="20359-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="20359-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20359-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="20359-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20359-107">Representa um mapeamento entre identificadores de equipe para extensões de sistema macOS e tipos de extensão de sistema.</span><span class="sxs-lookup"><span data-stu-id="20359-107">Represents a mapping between team identifiers for macOS system extensions and system extension types.</span></span>

## <a name="properties"></a><span data-ttu-id="20359-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20359-108">Properties</span></span>
|<span data-ttu-id="20359-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20359-109">Property</span></span>|<span data-ttu-id="20359-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="20359-110">Type</span></span>|<span data-ttu-id="20359-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="20359-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20359-112">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="20359-112">teamIdentifier</span></span>|<span data-ttu-id="20359-113">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="20359-113">String</span></span>|<span data-ttu-id="20359-114">Obtém ou define o identificador de equipe usado para assinar a extensão do sistema.</span><span class="sxs-lookup"><span data-stu-id="20359-114">Gets or sets the team identifier used to sign the system extension.</span></span>|
|<span data-ttu-id="20359-115">allowedTypes</span><span class="sxs-lookup"><span data-stu-id="20359-115">allowedTypes</span></span>|[<span data-ttu-id="20359-116">macOSSystemExtensionType</span><span class="sxs-lookup"><span data-stu-id="20359-116">macOSSystemExtensionType</span></span>](../resources/intune-deviceconfig-macossystemextensiontype.md)|<span data-ttu-id="20359-117">Obtém ou define os tipos de extensões de sistema macOS permitidos.</span><span class="sxs-lookup"><span data-stu-id="20359-117">Gets or sets the allowed macOS system extension types.</span></span> <span data-ttu-id="20359-118">Os valores possíveis são: `driverExtensionsAllowed`, `networkExtensionsAllowed`, `endpointSecurityExtensionsAllowed`.</span><span class="sxs-lookup"><span data-stu-id="20359-118">Possible values are: `driverExtensionsAllowed`, `networkExtensionsAllowed`, `endpointSecurityExtensionsAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20359-119">Relações</span><span class="sxs-lookup"><span data-stu-id="20359-119">Relationships</span></span>
<span data-ttu-id="20359-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="20359-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="20359-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="20359-121">JSON Representation</span></span>
<span data-ttu-id="20359-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="20359-122">Here is a JSON representation of the resource.</span></span>
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



