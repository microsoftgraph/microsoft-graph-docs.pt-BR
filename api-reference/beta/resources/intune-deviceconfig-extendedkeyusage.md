---
title: tipo de recurso extendedKeyUsage
description: Definição de uso de chave estendida personalizada
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c4fe1818aca19053242882e45edd1da5bbc544e8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460032"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="9d406-103">tipo de recurso extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="9d406-103">extendedKeyUsage resource type</span></span>

<span data-ttu-id="9d406-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d406-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d406-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9d406-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d406-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9d406-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d406-107">Definição de uso de chave estendida personalizada</span><span class="sxs-lookup"><span data-stu-id="9d406-107">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="9d406-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d406-108">Properties</span></span>
|<span data-ttu-id="9d406-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d406-109">Property</span></span>|<span data-ttu-id="9d406-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d406-110">Type</span></span>|<span data-ttu-id="9d406-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d406-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d406-112">nome</span><span class="sxs-lookup"><span data-stu-id="9d406-112">name</span></span>|<span data-ttu-id="9d406-113">String</span><span class="sxs-lookup"><span data-stu-id="9d406-113">String</span></span>|<span data-ttu-id="9d406-114">Nome estendido do uso de chave</span><span class="sxs-lookup"><span data-stu-id="9d406-114">Extended Key Usage Name</span></span>|
|<span data-ttu-id="9d406-115">objectidentifier</span><span class="sxs-lookup"><span data-stu-id="9d406-115">objectIdentifier</span></span>|<span data-ttu-id="9d406-116">String</span><span class="sxs-lookup"><span data-stu-id="9d406-116">String</span></span>|<span data-ttu-id="9d406-117">Identificador de objeto de uso estendido de chave</span><span class="sxs-lookup"><span data-stu-id="9d406-117">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d406-118">Relações</span><span class="sxs-lookup"><span data-stu-id="9d406-118">Relationships</span></span>
<span data-ttu-id="9d406-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9d406-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d406-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d406-120">JSON Representation</span></span>
<span data-ttu-id="9d406-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9d406-121">Here is a JSON representation of the resource.</span></span>
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



