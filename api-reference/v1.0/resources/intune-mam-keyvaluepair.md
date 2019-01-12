---
title: Tipo de recurso keyValuePair
description: Par chave-valor para armazenar configurações personalizadas
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: db3e24c1c14cb208be66b7a2b0364ad12b162956
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926439"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="3a228-103">Tipo de recurso keyValuePair</span><span class="sxs-lookup"><span data-stu-id="3a228-103">keyValuePair resource type</span></span>

> <span data-ttu-id="3a228-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3a228-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a228-105">Par chave-valor para armazenar configurações personalizadas</span><span class="sxs-lookup"><span data-stu-id="3a228-105">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="3a228-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a228-106">Properties</span></span>
|<span data-ttu-id="3a228-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a228-107">Property</span></span>|<span data-ttu-id="3a228-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a228-108">Type</span></span>|<span data-ttu-id="3a228-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a228-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a228-110">name</span><span class="sxs-lookup"><span data-stu-id="3a228-110">name</span></span>|<span data-ttu-id="3a228-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a228-111">String</span></span>|<span data-ttu-id="3a228-112">Nome deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="3a228-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="3a228-113">valor</span><span class="sxs-lookup"><span data-stu-id="3a228-113">value</span></span>|<span data-ttu-id="3a228-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a228-114">String</span></span>|<span data-ttu-id="3a228-115">Valor deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="3a228-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a228-116">Relações</span><span class="sxs-lookup"><span data-stu-id="3a228-116">Relationships</span></span>
<span data-ttu-id="3a228-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3a228-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3a228-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a228-118">JSON Representation</span></span>
<span data-ttu-id="3a228-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a228-119">Here is a JSON representation of the resource.</span></span>
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



