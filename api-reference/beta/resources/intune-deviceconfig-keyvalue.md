---
title: tipo de recurso keyValue
description: Definição do valor da chave.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e3133962d9f6bfb5f5363dd6d6cbd4b5ef2ea202
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406812"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="188f5-103">tipo de recurso keyValue</span><span class="sxs-lookup"><span data-stu-id="188f5-103">keyValue resource type</span></span>

> <span data-ttu-id="188f5-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="188f5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="188f5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="188f5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="188f5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="188f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="188f5-107">Definição do valor da chave.</span><span class="sxs-lookup"><span data-stu-id="188f5-107">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="188f5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="188f5-108">Properties</span></span>
|<span data-ttu-id="188f5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="188f5-109">Property</span></span>|<span data-ttu-id="188f5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="188f5-110">Type</span></span>|<span data-ttu-id="188f5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="188f5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="188f5-112">key</span><span class="sxs-lookup"><span data-stu-id="188f5-112">key</span></span>|<span data-ttu-id="188f5-113">String</span><span class="sxs-lookup"><span data-stu-id="188f5-113">String</span></span>|<span data-ttu-id="188f5-114">Chave.</span><span class="sxs-lookup"><span data-stu-id="188f5-114">Key.</span></span>|
|<span data-ttu-id="188f5-115">valor</span><span class="sxs-lookup"><span data-stu-id="188f5-115">value</span></span>|<span data-ttu-id="188f5-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="188f5-116">String</span></span>|<span data-ttu-id="188f5-117">Valor.</span><span class="sxs-lookup"><span data-stu-id="188f5-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="188f5-118">Relações</span><span class="sxs-lookup"><span data-stu-id="188f5-118">Relationships</span></span>
<span data-ttu-id="188f5-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="188f5-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="188f5-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="188f5-120">JSON Representation</span></span>
<span data-ttu-id="188f5-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="188f5-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValue",
  "key": "String",
  "value": "String"
}
```




