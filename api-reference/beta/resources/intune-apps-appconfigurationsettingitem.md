---
title: Tipo de recurso appConfigurationSettingItem
description: Contém propriedades do item de configuração de Configuração do aplicativo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b7f5492c9b54c9414db6a8332e218a1d7f0a50b1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403760"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="5c7a1-103">Tipo de recurso appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="5c7a1-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="5c7a1-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="5c7a1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5c7a1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5c7a1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5c7a1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="5c7a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c7a1-107">Contém propriedades do item de configuração de Configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5c7a1-107">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="5c7a1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5c7a1-108">Properties</span></span>
|<span data-ttu-id="5c7a1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c7a1-109">Property</span></span>|<span data-ttu-id="5c7a1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c7a1-110">Type</span></span>|<span data-ttu-id="5c7a1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c7a1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c7a1-112">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="5c7a1-112">appConfigKey</span></span>|<span data-ttu-id="5c7a1-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c7a1-113">String</span></span>|<span data-ttu-id="5c7a1-114">chave de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5c7a1-114">app configuration key.</span></span>|
|<span data-ttu-id="5c7a1-115">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="5c7a1-115">appConfigKeyType</span></span>|[<span data-ttu-id="5c7a1-116">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="5c7a1-116">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="5c7a1-117">tipo de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5c7a1-117">app configuration key type.</span></span> <span data-ttu-id="5c7a1-118">Os valores possíveis são: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="5c7a1-118">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="5c7a1-119">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="5c7a1-119">appConfigKeyValue</span></span>|<span data-ttu-id="5c7a1-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c7a1-120">String</span></span>|<span data-ttu-id="5c7a1-121">valor de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5c7a1-121">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c7a1-122">Relações</span><span class="sxs-lookup"><span data-stu-id="5c7a1-122">Relationships</span></span>
<span data-ttu-id="5c7a1-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5c7a1-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c7a1-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5c7a1-124">JSON Representation</span></span>
<span data-ttu-id="5c7a1-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5c7a1-125">Here is a JSON representation of the resource.</span></span>
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




