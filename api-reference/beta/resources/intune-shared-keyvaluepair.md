---
title: Tipo de recurso keyValuePair
description: Par chave-valor para armazenar configurações personalizadas
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 056dbe1f8504a89e3551402de7aa7ff7bc0ce866
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858440"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="0ada9-103">Tipo de recurso keyValuePair</span><span class="sxs-lookup"><span data-stu-id="0ada9-103">keyValuePair resource type</span></span>

> <span data-ttu-id="0ada9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0ada9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ada9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0ada9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ada9-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0ada9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ada9-107">Par chave-valor para armazenar configurações personalizadas</span><span class="sxs-lookup"><span data-stu-id="0ada9-107">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="0ada9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ada9-108">Properties</span></span>
|<span data-ttu-id="0ada9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ada9-109">Property</span></span>|<span data-ttu-id="0ada9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ada9-110">Type</span></span>|<span data-ttu-id="0ada9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ada9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ada9-112">name</span><span class="sxs-lookup"><span data-stu-id="0ada9-112">name</span></span>|<span data-ttu-id="0ada9-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ada9-113">String</span></span>|<span data-ttu-id="0ada9-114">Nome deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="0ada9-114">Name for this key-value pair</span></span>|
|<span data-ttu-id="0ada9-115">valor</span><span class="sxs-lookup"><span data-stu-id="0ada9-115">value</span></span>|<span data-ttu-id="0ada9-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ada9-116">String</span></span>|<span data-ttu-id="0ada9-117">Valor deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="0ada9-117">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ada9-118">Relações</span><span class="sxs-lookup"><span data-stu-id="0ada9-118">Relationships</span></span>
<span data-ttu-id="0ada9-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0ada9-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0ada9-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ada9-120">JSON Representation</span></span>
<span data-ttu-id="0ada9-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ada9-121">Here is a JSON representation of the resource.</span></span>
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





