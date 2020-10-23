---
title: tipo de recurso macOSAssociatedDomainsItem
description: Um mapeamento de identificadores de aplicativo para domínios associados.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6fa40fda83eb6dd89fa0d8fd709a8bf744a8cc19
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736251"
---
# <a name="macosassociateddomainsitem-resource-type"></a><span data-ttu-id="eb0b7-103">tipo de recurso macOSAssociatedDomainsItem</span><span class="sxs-lookup"><span data-stu-id="eb0b7-103">macOSAssociatedDomainsItem resource type</span></span>

<span data-ttu-id="eb0b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb0b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eb0b7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eb0b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb0b7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eb0b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb0b7-107">Um mapeamento de identificadores de aplicativo para domínios associados.</span><span class="sxs-lookup"><span data-stu-id="eb0b7-107">A mapping of application identifiers to associated domains.</span></span>

## <a name="properties"></a><span data-ttu-id="eb0b7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb0b7-108">Properties</span></span>
|<span data-ttu-id="eb0b7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb0b7-109">Property</span></span>|<span data-ttu-id="eb0b7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb0b7-110">Type</span></span>|<span data-ttu-id="eb0b7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb0b7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb0b7-112">applicationIdentifier</span><span class="sxs-lookup"><span data-stu-id="eb0b7-112">applicationIdentifier</span></span>|<span data-ttu-id="eb0b7-113">String</span><span class="sxs-lookup"><span data-stu-id="eb0b7-113">String</span></span>|<span data-ttu-id="eb0b7-114">O identificador de aplicativo do aplicativo para o qual associar domínios.</span><span class="sxs-lookup"><span data-stu-id="eb0b7-114">The application identifier of the app to associate domains with.</span></span>|
|<span data-ttu-id="eb0b7-115">domínio</span><span class="sxs-lookup"><span data-stu-id="eb0b7-115">domains</span></span>|<span data-ttu-id="eb0b7-116">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb0b7-116">String collection</span></span>|<span data-ttu-id="eb0b7-117">A lista de domínios a serem associados.</span><span class="sxs-lookup"><span data-stu-id="eb0b7-117">The list of domains to associate.</span></span>|
|<span data-ttu-id="eb0b7-118">directDownloadsEnabled</span><span class="sxs-lookup"><span data-stu-id="eb0b7-118">directDownloadsEnabled</span></span>|<span data-ttu-id="eb0b7-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb0b7-119">Boolean</span></span>|<span data-ttu-id="eb0b7-120">Determina se os dados devem ser baixados diretamente ou por meio de uma CDN.</span><span class="sxs-lookup"><span data-stu-id="eb0b7-120">Determines whether data should be downloaded directly or via a CDN.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb0b7-121">Relações</span><span class="sxs-lookup"><span data-stu-id="eb0b7-121">Relationships</span></span>
<span data-ttu-id="eb0b7-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eb0b7-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb0b7-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb0b7-123">JSON Representation</span></span>
<span data-ttu-id="eb0b7-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb0b7-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSAssociatedDomainsItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSAssociatedDomainsItem",
  "applicationIdentifier": "String",
  "domains": [
    "String"
  ],
  "directDownloadsEnabled": true
}
```





