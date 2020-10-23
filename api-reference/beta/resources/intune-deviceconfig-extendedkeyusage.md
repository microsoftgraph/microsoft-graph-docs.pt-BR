---
title: tipo de recurso extendedKeyUsage
description: Definição de uso de chave estendida personalizada
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 89b97b7061e34fbb83b33c7ec0a9e626d7eb5a5e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696171"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="9c96f-103">tipo de recurso extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="9c96f-103">extendedKeyUsage resource type</span></span>

<span data-ttu-id="9c96f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c96f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c96f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9c96f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c96f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9c96f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c96f-107">Definição de uso de chave estendida personalizada</span><span class="sxs-lookup"><span data-stu-id="9c96f-107">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="9c96f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c96f-108">Properties</span></span>
|<span data-ttu-id="9c96f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c96f-109">Property</span></span>|<span data-ttu-id="9c96f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c96f-110">Type</span></span>|<span data-ttu-id="9c96f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c96f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c96f-112">nome</span><span class="sxs-lookup"><span data-stu-id="9c96f-112">name</span></span>|<span data-ttu-id="9c96f-113">String</span><span class="sxs-lookup"><span data-stu-id="9c96f-113">String</span></span>|<span data-ttu-id="9c96f-114">Nome estendido do uso de chave</span><span class="sxs-lookup"><span data-stu-id="9c96f-114">Extended Key Usage Name</span></span>|
|<span data-ttu-id="9c96f-115">objectidentifier</span><span class="sxs-lookup"><span data-stu-id="9c96f-115">objectIdentifier</span></span>|<span data-ttu-id="9c96f-116">String</span><span class="sxs-lookup"><span data-stu-id="9c96f-116">String</span></span>|<span data-ttu-id="9c96f-117">Identificador de objeto de uso estendido de chave</span><span class="sxs-lookup"><span data-stu-id="9c96f-117">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c96f-118">Relações</span><span class="sxs-lookup"><span data-stu-id="9c96f-118">Relationships</span></span>
<span data-ttu-id="9c96f-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9c96f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c96f-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c96f-120">JSON Representation</span></span>
<span data-ttu-id="9c96f-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c96f-121">Here is a JSON representation of the resource.</span></span>
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





