---
title: Tipo de recurso appConfigurationSettingItem
description: Contém propriedades do item de configuração de Configuração do aplicativo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0590a22178935e9e8a6b4eb0e279b55d4f984222
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842151"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="6b34b-103">Tipo de recurso appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="6b34b-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="6b34b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6b34b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b34b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6b34b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6b34b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6b34b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b34b-107">Contém propriedades do item de configuração de Configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6b34b-107">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="6b34b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b34b-108">Properties</span></span>
|<span data-ttu-id="6b34b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b34b-109">Property</span></span>|<span data-ttu-id="6b34b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b34b-110">Type</span></span>|<span data-ttu-id="6b34b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b34b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b34b-112">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="6b34b-112">appConfigKey</span></span>|<span data-ttu-id="6b34b-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b34b-113">String</span></span>|<span data-ttu-id="6b34b-114">chave de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6b34b-114">app configuration key.</span></span>|
|<span data-ttu-id="6b34b-115">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="6b34b-115">appConfigKeyType</span></span>|[<span data-ttu-id="6b34b-116">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="6b34b-116">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="6b34b-117">tipo de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6b34b-117">app configuration key type.</span></span> <span data-ttu-id="6b34b-118">Os valores possíveis são: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="6b34b-118">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="6b34b-119">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="6b34b-119">appConfigKeyValue</span></span>|<span data-ttu-id="6b34b-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b34b-120">String</span></span>|<span data-ttu-id="6b34b-121">valor de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6b34b-121">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b34b-122">Relações</span><span class="sxs-lookup"><span data-stu-id="6b34b-122">Relationships</span></span>
<span data-ttu-id="6b34b-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b34b-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6b34b-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b34b-124">JSON Representation</span></span>
<span data-ttu-id="6b34b-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6b34b-125">Here is a JSON representation of the resource.</span></span>
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





