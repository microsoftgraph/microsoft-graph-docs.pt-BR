---
title: Tipo de recurso appConfigurationSettingItem
description: Contém propriedades do item de configuração de Configuração do aplicativo.
author: tfitzmac
ms.openlocfilehash: 9a9020acc63c445d919564865c44d9c57a5ff57a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320941"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="9f96f-103">Tipo de recurso appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="9f96f-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="9f96f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9f96f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f96f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9f96f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f96f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9f96f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f96f-107">Contém propriedades do item de configuração de Configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9f96f-107">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="9f96f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9f96f-108">Properties</span></span>
|<span data-ttu-id="9f96f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f96f-109">Property</span></span>|<span data-ttu-id="9f96f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f96f-110">Type</span></span>|<span data-ttu-id="9f96f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f96f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f96f-112">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="9f96f-112">appConfigKey</span></span>|<span data-ttu-id="9f96f-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f96f-113">String</span></span>|<span data-ttu-id="9f96f-114">chave de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9f96f-114">app configuration key.</span></span>|
|<span data-ttu-id="9f96f-115">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="9f96f-115">appConfigKeyType</span></span>|[<span data-ttu-id="9f96f-116">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="9f96f-116">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="9f96f-117">tipo de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9f96f-117">app configuration key type.</span></span> <span data-ttu-id="9f96f-118">Os valores possíveis são: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="9f96f-118">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="9f96f-119">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="9f96f-119">appConfigKeyValue</span></span>|<span data-ttu-id="9f96f-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f96f-120">String</span></span>|<span data-ttu-id="9f96f-121">valor de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9f96f-121">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f96f-122">Relações</span><span class="sxs-lookup"><span data-stu-id="9f96f-122">Relationships</span></span>
<span data-ttu-id="9f96f-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9f96f-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9f96f-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9f96f-124">JSON Representation</span></span>
<span data-ttu-id="9f96f-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9f96f-125">Here is a JSON representation of the resource.</span></span>
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





