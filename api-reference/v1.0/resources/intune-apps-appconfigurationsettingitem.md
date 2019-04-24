---
title: Tipo de recurso appConfigurationSettingItem
description: Contém propriedades do item de configuração de Configuração do aplicativo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 11ef3a964d166301c04c49730ac084b68e700b7c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503587"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="d99df-103">Tipo de recurso appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="d99df-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="d99df-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d99df-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d99df-105">Contém propriedades do item de configuração de Configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d99df-105">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="d99df-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d99df-106">Properties</span></span>
|<span data-ttu-id="d99df-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d99df-107">Property</span></span>|<span data-ttu-id="d99df-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d99df-108">Type</span></span>|<span data-ttu-id="d99df-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d99df-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d99df-110">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="d99df-110">appConfigKey</span></span>|<span data-ttu-id="d99df-111">String</span><span class="sxs-lookup"><span data-stu-id="d99df-111">String</span></span>|<span data-ttu-id="d99df-112">chave de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d99df-112">app configuration key.</span></span>|
|<span data-ttu-id="d99df-113">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="d99df-113">appConfigKeyType</span></span>|[<span data-ttu-id="d99df-114">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="d99df-114">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="d99df-115">tipo de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d99df-115">app configuration key type.</span></span> <span data-ttu-id="d99df-116">Os valores possíveis são: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="d99df-116">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="d99df-117">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="d99df-117">appConfigKeyValue</span></span>|<span data-ttu-id="d99df-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d99df-118">String</span></span>|<span data-ttu-id="d99df-119">valor de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d99df-119">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d99df-120">Relações</span><span class="sxs-lookup"><span data-stu-id="d99df-120">Relationships</span></span>
<span data-ttu-id="d99df-121">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d99df-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d99df-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d99df-122">JSON Representation</span></span>
<span data-ttu-id="d99df-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d99df-123">Here is a JSON representation of the resource.</span></span>
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



