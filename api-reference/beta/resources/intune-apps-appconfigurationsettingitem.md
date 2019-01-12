---
title: Tipo de recurso appConfigurationSettingItem
description: Contém propriedades do item de configuração de Configuração do aplicativo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ddd574ea19057fe31dbca5f258f8153071cd440c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927125"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="921cf-103">Tipo de recurso appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="921cf-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="921cf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="921cf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="921cf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="921cf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="921cf-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="921cf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="921cf-107">Contém propriedades do item de configuração de Configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="921cf-107">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="921cf-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="921cf-108">Properties</span></span>
|<span data-ttu-id="921cf-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="921cf-109">Property</span></span>|<span data-ttu-id="921cf-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="921cf-110">Type</span></span>|<span data-ttu-id="921cf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="921cf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="921cf-112">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="921cf-112">appConfigKey</span></span>|<span data-ttu-id="921cf-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="921cf-113">String</span></span>|<span data-ttu-id="921cf-114">chave de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="921cf-114">app configuration key.</span></span>|
|<span data-ttu-id="921cf-115">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="921cf-115">appConfigKeyType</span></span>|[<span data-ttu-id="921cf-116">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="921cf-116">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="921cf-117">tipo de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="921cf-117">app configuration key type.</span></span> <span data-ttu-id="921cf-118">Os valores possíveis são: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="921cf-118">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="921cf-119">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="921cf-119">appConfigKeyValue</span></span>|<span data-ttu-id="921cf-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="921cf-120">String</span></span>|<span data-ttu-id="921cf-121">valor de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="921cf-121">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="921cf-122">Relações</span><span class="sxs-lookup"><span data-stu-id="921cf-122">Relationships</span></span>
<span data-ttu-id="921cf-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="921cf-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="921cf-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="921cf-124">JSON Representation</span></span>
<span data-ttu-id="921cf-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="921cf-125">Here is a JSON representation of the resource.</span></span>
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





