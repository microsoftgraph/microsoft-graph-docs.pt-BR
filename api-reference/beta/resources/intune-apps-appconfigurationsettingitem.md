---
title: Tipo de recurso appConfigurationSettingItem
description: Contém propriedades do item de configuração de Configuração do aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6e2ec0f05b7bb40d97458a7d9fa452edc9124451
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003994"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="58263-103">Tipo de recurso appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="58263-103">appConfigurationSettingItem resource type</span></span>

<span data-ttu-id="58263-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="58263-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58263-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="58263-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58263-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="58263-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58263-107">Contém propriedades do item de configuração de Configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="58263-107">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="58263-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="58263-108">Properties</span></span>
|<span data-ttu-id="58263-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58263-109">Property</span></span>|<span data-ttu-id="58263-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="58263-110">Type</span></span>|<span data-ttu-id="58263-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="58263-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58263-112">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="58263-112">appConfigKey</span></span>|<span data-ttu-id="58263-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58263-113">String</span></span>|<span data-ttu-id="58263-114">chave de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="58263-114">app configuration key.</span></span>|
|<span data-ttu-id="58263-115">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="58263-115">appConfigKeyType</span></span>|[<span data-ttu-id="58263-116">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="58263-116">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="58263-117">tipo de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="58263-117">app configuration key type.</span></span> <span data-ttu-id="58263-118">Os valores possíveis são: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="58263-118">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="58263-119">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="58263-119">appConfigKeyValue</span></span>|<span data-ttu-id="58263-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58263-120">String</span></span>|<span data-ttu-id="58263-121">valor de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="58263-121">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58263-122">Relações</span><span class="sxs-lookup"><span data-stu-id="58263-122">Relationships</span></span>
<span data-ttu-id="58263-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="58263-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58263-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="58263-124">JSON Representation</span></span>
<span data-ttu-id="58263-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="58263-125">Here is a JSON representation of the resource.</span></span>
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






