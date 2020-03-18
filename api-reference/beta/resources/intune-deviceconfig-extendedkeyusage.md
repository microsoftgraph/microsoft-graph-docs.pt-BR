---
title: tipo de recurso extendedKeyUsage
description: Definição de uso de chave estendida personalizada
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 19cf790f692d624d926485fdc26feed1f69c73b7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791769"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="af5bf-103">tipo de recurso extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="af5bf-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="af5bf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="af5bf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af5bf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="af5bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af5bf-106">Definição de uso de chave estendida personalizada</span><span class="sxs-lookup"><span data-stu-id="af5bf-106">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="af5bf-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="af5bf-107">Properties</span></span>
|<span data-ttu-id="af5bf-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af5bf-108">Property</span></span>|<span data-ttu-id="af5bf-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="af5bf-109">Type</span></span>|<span data-ttu-id="af5bf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="af5bf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af5bf-111">nome</span><span class="sxs-lookup"><span data-stu-id="af5bf-111">name</span></span>|<span data-ttu-id="af5bf-112">String</span><span class="sxs-lookup"><span data-stu-id="af5bf-112">String</span></span>|<span data-ttu-id="af5bf-113">Nome estendido do uso de chave</span><span class="sxs-lookup"><span data-stu-id="af5bf-113">Extended Key Usage Name</span></span>|
|<span data-ttu-id="af5bf-114">objectidentifier</span><span class="sxs-lookup"><span data-stu-id="af5bf-114">objectIdentifier</span></span>|<span data-ttu-id="af5bf-115">String</span><span class="sxs-lookup"><span data-stu-id="af5bf-115">String</span></span>|<span data-ttu-id="af5bf-116">Identificador de objeto de uso estendido de chave</span><span class="sxs-lookup"><span data-stu-id="af5bf-116">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="af5bf-117">Relações</span><span class="sxs-lookup"><span data-stu-id="af5bf-117">Relationships</span></span>
<span data-ttu-id="af5bf-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="af5bf-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="af5bf-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="af5bf-119">JSON Representation</span></span>
<span data-ttu-id="af5bf-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="af5bf-120">Here is a JSON representation of the resource.</span></span>
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



