---
title: Tipo de recurso appConfigurationSettingItem
description: Contém propriedades do item de configuração de Configuração do aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bdc552bc2dcaf04990999c9414d2723284a568f2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48045464"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="604b4-103">Tipo de recurso appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="604b4-103">appConfigurationSettingItem resource type</span></span>

<span data-ttu-id="604b4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="604b4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="604b4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="604b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="604b4-106">Contém propriedades do item de configuração de Configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="604b4-106">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="604b4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="604b4-107">Properties</span></span>
|<span data-ttu-id="604b4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="604b4-108">Property</span></span>|<span data-ttu-id="604b4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="604b4-109">Type</span></span>|<span data-ttu-id="604b4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="604b4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="604b4-111">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="604b4-111">appConfigKey</span></span>|<span data-ttu-id="604b4-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="604b4-112">String</span></span>|<span data-ttu-id="604b4-113">chave de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="604b4-113">app configuration key.</span></span>|
|<span data-ttu-id="604b4-114">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="604b4-114">appConfigKeyType</span></span>|[<span data-ttu-id="604b4-115">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="604b4-115">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="604b4-116">tipo de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="604b4-116">app configuration key type.</span></span> <span data-ttu-id="604b4-117">Os valores possíveis são: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="604b4-117">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="604b4-118">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="604b4-118">appConfigKeyValue</span></span>|<span data-ttu-id="604b4-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="604b4-119">String</span></span>|<span data-ttu-id="604b4-120">valor de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="604b4-120">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="604b4-121">Relações</span><span class="sxs-lookup"><span data-stu-id="604b4-121">Relationships</span></span>
<span data-ttu-id="604b4-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="604b4-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="604b4-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="604b4-123">JSON Representation</span></span>
<span data-ttu-id="604b4-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="604b4-124">Here is a JSON representation of the resource.</span></span>
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









