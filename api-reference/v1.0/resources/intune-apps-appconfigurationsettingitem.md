---
title: Tipo de recurso appConfigurationSettingItem
description: Contém propriedades do item de configuração de Configuração do aplicativo.
ms.openlocfilehash: bd08b325fd04e8e4a742da515d052d453cfb58a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005247"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="17957-103">Tipo de recurso appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="17957-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="17957-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="17957-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17957-105">Contém propriedades do item de configuração de Configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="17957-105">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="17957-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="17957-106">Properties</span></span>
|<span data-ttu-id="17957-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17957-107">Property</span></span>|<span data-ttu-id="17957-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="17957-108">Type</span></span>|<span data-ttu-id="17957-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="17957-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17957-110">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="17957-110">appConfigKey</span></span>|<span data-ttu-id="17957-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17957-111">String</span></span>|<span data-ttu-id="17957-112">chave de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="17957-112">app configuration key.</span></span>|
|<span data-ttu-id="17957-113">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="17957-113">appConfigKeyType</span></span>|[<span data-ttu-id="17957-114">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="17957-114">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="17957-115">tipo de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="17957-115">app configuration key type.</span></span> <span data-ttu-id="17957-116">Os valores possíveis são: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="17957-116">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="17957-117">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="17957-117">appConfigKeyValue</span></span>|<span data-ttu-id="17957-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17957-118">String</span></span>|<span data-ttu-id="17957-119">valor de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="17957-119">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="17957-120">Relações</span><span class="sxs-lookup"><span data-stu-id="17957-120">Relationships</span></span>
<span data-ttu-id="17957-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="17957-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="17957-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="17957-122">JSON Representation</span></span>
<span data-ttu-id="17957-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="17957-123">Here is a JSON representation of the resource.</span></span>
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



