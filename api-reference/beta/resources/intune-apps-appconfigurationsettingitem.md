---
title: Tipo de recurso appConfigurationSettingItem
description: Contém propriedades do item de configuração de Configuração do aplicativo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f001a02a1e4e3ef2a15fe5e606687896775a6d26
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991258"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="493f2-103">Tipo de recurso appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="493f2-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="493f2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="493f2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="493f2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="493f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="493f2-106">Contém propriedades do item de configuração de Configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="493f2-106">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="493f2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="493f2-107">Properties</span></span>
|<span data-ttu-id="493f2-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="493f2-108">Property</span></span>|<span data-ttu-id="493f2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="493f2-109">Type</span></span>|<span data-ttu-id="493f2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="493f2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="493f2-111">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="493f2-111">appConfigKey</span></span>|<span data-ttu-id="493f2-112">String</span><span class="sxs-lookup"><span data-stu-id="493f2-112">String</span></span>|<span data-ttu-id="493f2-113">chave de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="493f2-113">app configuration key.</span></span>|
|<span data-ttu-id="493f2-114">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="493f2-114">appConfigKeyType</span></span>|[<span data-ttu-id="493f2-115">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="493f2-115">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="493f2-116">tipo de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="493f2-116">app configuration key type.</span></span> <span data-ttu-id="493f2-117">Os valores possíveis são: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="493f2-117">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="493f2-118">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="493f2-118">appConfigKeyValue</span></span>|<span data-ttu-id="493f2-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="493f2-119">String</span></span>|<span data-ttu-id="493f2-120">valor de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="493f2-120">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="493f2-121">Relações</span><span class="sxs-lookup"><span data-stu-id="493f2-121">Relationships</span></span>
<span data-ttu-id="493f2-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="493f2-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="493f2-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="493f2-123">JSON Representation</span></span>
<span data-ttu-id="493f2-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="493f2-124">Here is a JSON representation of the resource.</span></span>
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





