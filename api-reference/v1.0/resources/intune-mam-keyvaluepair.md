---
title: Tipo de recurso keyValuePair
description: Par chave-valor para armazenar configurações personalizadas
ms.openlocfilehash: 803dd9e347ef06bc9d4a9fce13d2265c4fc969a3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006612"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="0e55e-103">Tipo de recurso keyValuePair</span><span class="sxs-lookup"><span data-stu-id="0e55e-103">keyValuePair resource type</span></span>

> <span data-ttu-id="0e55e-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0e55e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e55e-105">Par chave-valor para armazenar configurações personalizadas</span><span class="sxs-lookup"><span data-stu-id="0e55e-105">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="0e55e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0e55e-106">Properties</span></span>
|<span data-ttu-id="0e55e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e55e-107">Property</span></span>|<span data-ttu-id="0e55e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e55e-108">Type</span></span>|<span data-ttu-id="0e55e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e55e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e55e-110">name</span><span class="sxs-lookup"><span data-stu-id="0e55e-110">name</span></span>|<span data-ttu-id="0e55e-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e55e-111">String</span></span>|<span data-ttu-id="0e55e-112">Nome deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="0e55e-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="0e55e-113">valor</span><span class="sxs-lookup"><span data-stu-id="0e55e-113">value</span></span>|<span data-ttu-id="0e55e-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e55e-114">String</span></span>|<span data-ttu-id="0e55e-115">Valor deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="0e55e-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e55e-116">Relações</span><span class="sxs-lookup"><span data-stu-id="0e55e-116">Relationships</span></span>
<span data-ttu-id="0e55e-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0e55e-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0e55e-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0e55e-118">JSON Representation</span></span>
<span data-ttu-id="0e55e-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0e55e-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```



