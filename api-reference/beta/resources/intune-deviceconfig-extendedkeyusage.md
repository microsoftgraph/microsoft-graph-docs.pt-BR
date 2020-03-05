---
title: tipo de recurso extendedKeyUsage
description: Definição de uso de chave estendida personalizada
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 91e3cc0beec0a5854eb6c77a6510062614646900
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526448"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="e4a4c-103">tipo de recurso extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="e4a4c-103">extendedKeyUsage resource type</span></span>

<span data-ttu-id="e4a4c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e4a4c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4a4c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e4a4c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4a4c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4a4c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4a4c-107">Definição de uso de chave estendida personalizada</span><span class="sxs-lookup"><span data-stu-id="e4a4c-107">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="e4a4c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e4a4c-108">Properties</span></span>
|<span data-ttu-id="e4a4c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e4a4c-109">Property</span></span>|<span data-ttu-id="e4a4c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4a4c-110">Type</span></span>|<span data-ttu-id="e4a4c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4a4c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4a4c-112">nome</span><span class="sxs-lookup"><span data-stu-id="e4a4c-112">name</span></span>|<span data-ttu-id="e4a4c-113">String</span><span class="sxs-lookup"><span data-stu-id="e4a4c-113">String</span></span>|<span data-ttu-id="e4a4c-114">Nome estendido do uso de chave</span><span class="sxs-lookup"><span data-stu-id="e4a4c-114">Extended Key Usage Name</span></span>|
|<span data-ttu-id="e4a4c-115">objectidentifier</span><span class="sxs-lookup"><span data-stu-id="e4a4c-115">objectIdentifier</span></span>|<span data-ttu-id="e4a4c-116">String</span><span class="sxs-lookup"><span data-stu-id="e4a4c-116">String</span></span>|<span data-ttu-id="e4a4c-117">Identificador de objeto de uso estendido de chave</span><span class="sxs-lookup"><span data-stu-id="e4a4c-117">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4a4c-118">Relações</span><span class="sxs-lookup"><span data-stu-id="e4a4c-118">Relationships</span></span>
<span data-ttu-id="e4a4c-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e4a4c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4a4c-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e4a4c-120">JSON Representation</span></span>
<span data-ttu-id="e4a4c-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e4a4c-121">Here is a JSON representation of the resource.</span></span>
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



