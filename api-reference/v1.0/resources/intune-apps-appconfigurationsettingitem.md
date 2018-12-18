---
title: Tipo de recurso appConfigurationSettingItem
description: Contém propriedades do item de configuração de Configuração do aplicativo.
author: tfitzmac
ms.openlocfilehash: b75579e56602ad5359bc32d52312931342b42a6b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353575"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="d806e-103">Tipo de recurso appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="d806e-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="d806e-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d806e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d806e-105">Contém propriedades do item de configuração de Configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d806e-105">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="d806e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d806e-106">Properties</span></span>
|<span data-ttu-id="d806e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d806e-107">Property</span></span>|<span data-ttu-id="d806e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d806e-108">Type</span></span>|<span data-ttu-id="d806e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d806e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d806e-110">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="d806e-110">appConfigKey</span></span>|<span data-ttu-id="d806e-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d806e-111">String</span></span>|<span data-ttu-id="d806e-112">chave de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d806e-112">app configuration key.</span></span>|
|<span data-ttu-id="d806e-113">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="d806e-113">appConfigKeyType</span></span>|[<span data-ttu-id="d806e-114">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="d806e-114">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="d806e-115">tipo de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d806e-115">app configuration key type.</span></span> <span data-ttu-id="d806e-116">Os valores possíveis são: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="d806e-116">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="d806e-117">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="d806e-117">appConfigKeyValue</span></span>|<span data-ttu-id="d806e-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d806e-118">String</span></span>|<span data-ttu-id="d806e-119">valor de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d806e-119">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d806e-120">Relações</span><span class="sxs-lookup"><span data-stu-id="d806e-120">Relationships</span></span>
<span data-ttu-id="d806e-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d806e-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d806e-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d806e-122">JSON Representation</span></span>
<span data-ttu-id="d806e-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d806e-123">Here is a JSON representation of the resource.</span></span>
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



