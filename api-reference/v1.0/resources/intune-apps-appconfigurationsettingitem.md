---
title: Tipo de recurso appConfigurationSettingItem
description: Contém propriedades do item de configuração de Configuração do aplicativo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7b7145b7adf9aed622af8ebb3a6a55c6456d7e8a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356300"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="7a8fb-103">Tipo de recurso appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="7a8fb-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="7a8fb-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7a8fb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a8fb-105">Contém propriedades do item de configuração de Configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7a8fb-105">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="7a8fb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a8fb-106">Properties</span></span>
|<span data-ttu-id="7a8fb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a8fb-107">Property</span></span>|<span data-ttu-id="7a8fb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a8fb-108">Type</span></span>|<span data-ttu-id="7a8fb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a8fb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a8fb-110">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="7a8fb-110">appConfigKey</span></span>|<span data-ttu-id="7a8fb-111">String</span><span class="sxs-lookup"><span data-stu-id="7a8fb-111">String</span></span>|<span data-ttu-id="7a8fb-112">chave de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7a8fb-112">app configuration key.</span></span>|
|<span data-ttu-id="7a8fb-113">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="7a8fb-113">appConfigKeyType</span></span>|[<span data-ttu-id="7a8fb-114">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="7a8fb-114">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="7a8fb-115">tipo de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7a8fb-115">app configuration key type.</span></span> <span data-ttu-id="7a8fb-116">Os valores possíveis são: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="7a8fb-116">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="7a8fb-117">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="7a8fb-117">appConfigKeyValue</span></span>|<span data-ttu-id="7a8fb-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a8fb-118">String</span></span>|<span data-ttu-id="7a8fb-119">valor de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7a8fb-119">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a8fb-120">Relações</span><span class="sxs-lookup"><span data-stu-id="7a8fb-120">Relationships</span></span>
<span data-ttu-id="7a8fb-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7a8fb-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a8fb-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a8fb-122">JSON Representation</span></span>
<span data-ttu-id="7a8fb-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7a8fb-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConfigurationSettingItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConfigurationSettingItem",
  "appConfigKey": "String",
  "appConfigKeyType": "String",
  "appConfigKeyValue": "String"
}
```




