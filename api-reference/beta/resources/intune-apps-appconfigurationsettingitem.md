---
title: Tipo de recurso appConfigurationSettingItem
description: Contém propriedades do item de configuração de Configuração do aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7f29e8780ad6c71eaf331f9fe1b1e32d383f0b17
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49284726"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="cebed-103">Tipo de recurso appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="cebed-103">appConfigurationSettingItem resource type</span></span>

<span data-ttu-id="cebed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cebed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cebed-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cebed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cebed-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cebed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cebed-107">Contém propriedades do item de configuração de Configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cebed-107">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="cebed-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cebed-108">Properties</span></span>
|<span data-ttu-id="cebed-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cebed-109">Property</span></span>|<span data-ttu-id="cebed-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cebed-110">Type</span></span>|<span data-ttu-id="cebed-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cebed-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cebed-112">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="cebed-112">appConfigKey</span></span>|<span data-ttu-id="cebed-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cebed-113">String</span></span>|<span data-ttu-id="cebed-114">chave de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cebed-114">app configuration key.</span></span>|
|<span data-ttu-id="cebed-115">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="cebed-115">appConfigKeyType</span></span>|[<span data-ttu-id="cebed-116">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="cebed-116">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="cebed-117">tipo de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cebed-117">app configuration key type.</span></span> <span data-ttu-id="cebed-118">Os valores possíveis são: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="cebed-118">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="cebed-119">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="cebed-119">appConfigKeyValue</span></span>|<span data-ttu-id="cebed-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cebed-120">String</span></span>|<span data-ttu-id="cebed-121">valor de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cebed-121">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cebed-122">Relações</span><span class="sxs-lookup"><span data-stu-id="cebed-122">Relationships</span></span>
<span data-ttu-id="cebed-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cebed-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cebed-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cebed-124">JSON Representation</span></span>
<span data-ttu-id="cebed-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cebed-125">Here is a JSON representation of the resource.</span></span>
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




