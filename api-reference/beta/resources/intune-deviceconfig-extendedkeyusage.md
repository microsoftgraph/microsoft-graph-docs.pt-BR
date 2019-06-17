---
title: tipo de recurso extendedKeyUsage
description: Definição de uso de chave estendida personalizada
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9eb9a02c8f403bf4ee29fc28622ab06f592c870b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34982515"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="c27fe-103">tipo de recurso extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="c27fe-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="c27fe-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c27fe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c27fe-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c27fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c27fe-106">Definição de uso de chave estendida personalizada</span><span class="sxs-lookup"><span data-stu-id="c27fe-106">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="c27fe-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c27fe-107">Properties</span></span>
|<span data-ttu-id="c27fe-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c27fe-108">Property</span></span>|<span data-ttu-id="c27fe-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c27fe-109">Type</span></span>|<span data-ttu-id="c27fe-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c27fe-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c27fe-111">name</span><span class="sxs-lookup"><span data-stu-id="c27fe-111">name</span></span>|<span data-ttu-id="c27fe-112">String</span><span class="sxs-lookup"><span data-stu-id="c27fe-112">String</span></span>|<span data-ttu-id="c27fe-113">Nome estendido do uso de chave</span><span class="sxs-lookup"><span data-stu-id="c27fe-113">Extended Key Usage Name</span></span>|
|<span data-ttu-id="c27fe-114">objectidentifier</span><span class="sxs-lookup"><span data-stu-id="c27fe-114">objectIdentifier</span></span>|<span data-ttu-id="c27fe-115">String</span><span class="sxs-lookup"><span data-stu-id="c27fe-115">String</span></span>|<span data-ttu-id="c27fe-116">Identificador de objeto de uso estendido de chave</span><span class="sxs-lookup"><span data-stu-id="c27fe-116">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="c27fe-117">Relações</span><span class="sxs-lookup"><span data-stu-id="c27fe-117">Relationships</span></span>
<span data-ttu-id="c27fe-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c27fe-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c27fe-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c27fe-119">JSON Representation</span></span>
<span data-ttu-id="c27fe-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c27fe-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.extendedKeyUsage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extendedKeyUsage",
  "name": "String",
  "objectIdentifier": "String"
}
```





