---
title: Tipo de recurso appConfigurationSettingItem
description: Contém propriedades do item de configuração de Configuração do aplicativo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ddb7b503ff14e6499342fafc2d0cf5ab8e670138
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960333"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="2d1b3-103">Tipo de recurso appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="2d1b3-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="2d1b3-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2d1b3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d1b3-105">Contém propriedades do item de configuração de Configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2d1b3-105">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="2d1b3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2d1b3-106">Properties</span></span>
|<span data-ttu-id="2d1b3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d1b3-107">Property</span></span>|<span data-ttu-id="2d1b3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d1b3-108">Type</span></span>|<span data-ttu-id="2d1b3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d1b3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d1b3-110">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="2d1b3-110">appConfigKey</span></span>|<span data-ttu-id="2d1b3-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d1b3-111">String</span></span>|<span data-ttu-id="2d1b3-112">chave de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2d1b3-112">app configuration key.</span></span>|
|<span data-ttu-id="2d1b3-113">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="2d1b3-113">appConfigKeyType</span></span>|[<span data-ttu-id="2d1b3-114">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="2d1b3-114">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="2d1b3-115">tipo de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2d1b3-115">app configuration key type.</span></span> <span data-ttu-id="2d1b3-116">Os valores possíveis são: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="2d1b3-116">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="2d1b3-117">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="2d1b3-117">appConfigKeyValue</span></span>|<span data-ttu-id="2d1b3-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d1b3-118">String</span></span>|<span data-ttu-id="2d1b3-119">valor de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2d1b3-119">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d1b3-120">Relações</span><span class="sxs-lookup"><span data-stu-id="2d1b3-120">Relationships</span></span>
<span data-ttu-id="2d1b3-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2d1b3-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2d1b3-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2d1b3-122">JSON Representation</span></span>
<span data-ttu-id="2d1b3-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2d1b3-123">Here is a JSON representation of the resource.</span></span>
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



