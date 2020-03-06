---
title: Tipo de recurso appConfigurationSettingItem
description: Contém propriedades do item de configuração de Configuração do aplicativo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cb207355a6f637cc1f5c0e3031422f639e2bf357
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531247"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="7f543-103">Tipo de recurso appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="7f543-103">appConfigurationSettingItem resource type</span></span>

<span data-ttu-id="7f543-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f543-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f543-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7f543-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f543-106">Contém propriedades do item de configuração de Configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7f543-106">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="7f543-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7f543-107">Properties</span></span>
|<span data-ttu-id="7f543-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f543-108">Property</span></span>|<span data-ttu-id="7f543-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f543-109">Type</span></span>|<span data-ttu-id="7f543-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f543-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f543-111">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="7f543-111">appConfigKey</span></span>|<span data-ttu-id="7f543-112">String</span><span class="sxs-lookup"><span data-stu-id="7f543-112">String</span></span>|<span data-ttu-id="7f543-113">chave de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7f543-113">app configuration key.</span></span>|
|<span data-ttu-id="7f543-114">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="7f543-114">appConfigKeyType</span></span>|[<span data-ttu-id="7f543-115">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="7f543-115">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="7f543-116">tipo de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7f543-116">app configuration key type.</span></span> <span data-ttu-id="7f543-117">Os valores possíveis são: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="7f543-117">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="7f543-118">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="7f543-118">appConfigKeyValue</span></span>|<span data-ttu-id="7f543-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f543-119">String</span></span>|<span data-ttu-id="7f543-120">valor de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7f543-120">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f543-121">Relações</span><span class="sxs-lookup"><span data-stu-id="7f543-121">Relationships</span></span>
<span data-ttu-id="7f543-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7f543-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f543-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f543-123">JSON Representation</span></span>
<span data-ttu-id="7f543-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7f543-124">Here is a JSON representation of the resource.</span></span>
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




