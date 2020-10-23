---
title: Tipo de recurso appConfigurationSettingItem
description: Contém propriedades do item de configuração de Configuração do aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5b4d76284c5fbc099a24a4c848613302e0fd630f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727523"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="9ad3f-103">Tipo de recurso appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="9ad3f-103">appConfigurationSettingItem resource type</span></span>

<span data-ttu-id="9ad3f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ad3f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ad3f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9ad3f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ad3f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9ad3f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ad3f-107">Contém propriedades do item de configuração de Configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9ad3f-107">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="9ad3f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9ad3f-108">Properties</span></span>
|<span data-ttu-id="9ad3f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ad3f-109">Property</span></span>|<span data-ttu-id="9ad3f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ad3f-110">Type</span></span>|<span data-ttu-id="9ad3f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ad3f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ad3f-112">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="9ad3f-112">appConfigKey</span></span>|<span data-ttu-id="9ad3f-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ad3f-113">String</span></span>|<span data-ttu-id="9ad3f-114">chave de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9ad3f-114">app configuration key.</span></span>|
|<span data-ttu-id="9ad3f-115">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="9ad3f-115">appConfigKeyType</span></span>|[<span data-ttu-id="9ad3f-116">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="9ad3f-116">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="9ad3f-117">tipo de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9ad3f-117">app configuration key type.</span></span> <span data-ttu-id="9ad3f-118">Os valores possíveis são: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="9ad3f-118">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="9ad3f-119">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="9ad3f-119">appConfigKeyValue</span></span>|<span data-ttu-id="9ad3f-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ad3f-120">String</span></span>|<span data-ttu-id="9ad3f-121">valor de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9ad3f-121">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ad3f-122">Relações</span><span class="sxs-lookup"><span data-stu-id="9ad3f-122">Relationships</span></span>
<span data-ttu-id="9ad3f-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9ad3f-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ad3f-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ad3f-124">JSON Representation</span></span>
<span data-ttu-id="9ad3f-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9ad3f-125">Here is a JSON representation of the resource.</span></span>
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





