---
title: Tipo de recurso keyValuePair
description: Par chave-valor para armazenar configurações personalizadas
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f31e83c5e53ea4c2873fd2b425cc0e0c02678ea7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415779"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="65b3d-103">Tipo de recurso keyValuePair</span><span class="sxs-lookup"><span data-stu-id="65b3d-103">keyValuePair resource type</span></span>

> <span data-ttu-id="65b3d-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="65b3d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="65b3d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="65b3d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="65b3d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="65b3d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65b3d-107">Par chave-valor para armazenar configurações personalizadas</span><span class="sxs-lookup"><span data-stu-id="65b3d-107">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="65b3d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="65b3d-108">Properties</span></span>
|<span data-ttu-id="65b3d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65b3d-109">Property</span></span>|<span data-ttu-id="65b3d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="65b3d-110">Type</span></span>|<span data-ttu-id="65b3d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="65b3d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65b3d-112">name</span><span class="sxs-lookup"><span data-stu-id="65b3d-112">name</span></span>|<span data-ttu-id="65b3d-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65b3d-113">String</span></span>|<span data-ttu-id="65b3d-114">Nome deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="65b3d-114">Name for this key-value pair</span></span>|
|<span data-ttu-id="65b3d-115">valor</span><span class="sxs-lookup"><span data-stu-id="65b3d-115">value</span></span>|<span data-ttu-id="65b3d-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65b3d-116">String</span></span>|<span data-ttu-id="65b3d-117">Valor deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="65b3d-117">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="65b3d-118">Relações</span><span class="sxs-lookup"><span data-stu-id="65b3d-118">Relationships</span></span>
<span data-ttu-id="65b3d-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="65b3d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65b3d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="65b3d-120">JSON Representation</span></span>
<span data-ttu-id="65b3d-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="65b3d-121">Here is a JSON representation of the resource.</span></span>
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




