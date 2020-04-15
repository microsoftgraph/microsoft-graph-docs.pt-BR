---
title: Tipo de recurso appConfigurationSettingItem
description: Contém propriedades do item de configuração de Configuração do aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 997779a53680042f16c0fb4a4337889dbba377d8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43397334"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="d8b50-103">Tipo de recurso appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="d8b50-103">appConfigurationSettingItem resource type</span></span>

<span data-ttu-id="d8b50-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8b50-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8b50-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d8b50-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8b50-106">Contém propriedades do item de configuração de Configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d8b50-106">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="d8b50-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8b50-107">Properties</span></span>
|<span data-ttu-id="d8b50-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8b50-108">Property</span></span>|<span data-ttu-id="d8b50-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8b50-109">Type</span></span>|<span data-ttu-id="d8b50-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8b50-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8b50-111">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="d8b50-111">appConfigKey</span></span>|<span data-ttu-id="d8b50-112">String</span><span class="sxs-lookup"><span data-stu-id="d8b50-112">String</span></span>|<span data-ttu-id="d8b50-113">chave de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d8b50-113">app configuration key.</span></span>|
|<span data-ttu-id="d8b50-114">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="d8b50-114">appConfigKeyType</span></span>|[<span data-ttu-id="d8b50-115">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="d8b50-115">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="d8b50-116">tipo de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d8b50-116">app configuration key type.</span></span> <span data-ttu-id="d8b50-117">Os valores possíveis são: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="d8b50-117">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="d8b50-118">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="d8b50-118">appConfigKeyValue</span></span>|<span data-ttu-id="d8b50-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8b50-119">String</span></span>|<span data-ttu-id="d8b50-120">valor de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d8b50-120">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8b50-121">Relações</span><span class="sxs-lookup"><span data-stu-id="d8b50-121">Relationships</span></span>
<span data-ttu-id="d8b50-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d8b50-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8b50-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8b50-123">JSON Representation</span></span>
<span data-ttu-id="d8b50-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d8b50-124">Here is a JSON representation of the resource.</span></span>
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







