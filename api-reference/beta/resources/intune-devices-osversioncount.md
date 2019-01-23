---
title: tipo de recurso de osVersionCount
description: Contagem de dispositivos com malware para cada versão do sistema operacional
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cbe0d8ac149ad84ba4cd1286fb0f2303cdfb52a1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410459"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="1041c-103">tipo de recurso de osVersionCount</span><span class="sxs-lookup"><span data-stu-id="1041c-103">osVersionCount resource type</span></span>

> <span data-ttu-id="1041c-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="1041c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1041c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1041c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1041c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="1041c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1041c-107">Contagem de dispositivos com malware para cada versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="1041c-107">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="1041c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1041c-108">Properties</span></span>
|<span data-ttu-id="1041c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1041c-109">Property</span></span>|<span data-ttu-id="1041c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1041c-110">Type</span></span>|<span data-ttu-id="1041c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1041c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1041c-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="1041c-112">osVersion</span></span>|<span data-ttu-id="1041c-113">String</span><span class="sxs-lookup"><span data-stu-id="1041c-113">String</span></span>|<span data-ttu-id="1041c-114">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="1041c-114">OS version</span></span>|
|<span data-ttu-id="1041c-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="1041c-115">deviceCount</span></span>|<span data-ttu-id="1041c-116">Int32</span><span class="sxs-lookup"><span data-stu-id="1041c-116">Int32</span></span>|<span data-ttu-id="1041c-117">Contagem de dispositivos com malware para a versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="1041c-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="1041c-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="1041c-118">lastUpdateDateTime</span></span>|<span data-ttu-id="1041c-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1041c-119">DateTimeOffset</span></span>|<span data-ttu-id="1041c-120">O carimbo de hora da última atualização do dispositivo contar em UTC</span><span class="sxs-lookup"><span data-stu-id="1041c-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="1041c-121">Relações</span><span class="sxs-lookup"><span data-stu-id="1041c-121">Relationships</span></span>
<span data-ttu-id="1041c-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1041c-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1041c-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1041c-123">JSON Representation</span></span>
<span data-ttu-id="1041c-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1041c-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.osVersionCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.osVersionCount",
  "osVersion": "String",
  "deviceCount": 1024,
  "lastUpdateDateTime": "String (timestamp)"
}
```




