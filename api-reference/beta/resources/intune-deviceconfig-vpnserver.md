---
title: tipo de recurso vpnServer
description: Definição do servidor VPN.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 577b606ee4dc46cd5ed8f93c351f5b41e73fe973
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787317"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="a2d62-103">tipo de recurso vpnServer</span><span class="sxs-lookup"><span data-stu-id="a2d62-103">vpnServer resource type</span></span>

> <span data-ttu-id="a2d62-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a2d62-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2d62-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a2d62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2d62-106">Definição do servidor VPN.</span><span class="sxs-lookup"><span data-stu-id="a2d62-106">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="a2d62-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2d62-107">Properties</span></span>
|<span data-ttu-id="a2d62-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2d62-108">Property</span></span>|<span data-ttu-id="a2d62-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2d62-109">Type</span></span>|<span data-ttu-id="a2d62-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2d62-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2d62-111">description</span><span class="sxs-lookup"><span data-stu-id="a2d62-111">description</span></span>|<span data-ttu-id="a2d62-112">String</span><span class="sxs-lookup"><span data-stu-id="a2d62-112">String</span></span>|<span data-ttu-id="a2d62-113">Descrição.</span><span class="sxs-lookup"><span data-stu-id="a2d62-113">Description.</span></span>|
|<span data-ttu-id="a2d62-114">address</span><span class="sxs-lookup"><span data-stu-id="a2d62-114">address</span></span>|<span data-ttu-id="a2d62-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2d62-115">String</span></span>|<span data-ttu-id="a2d62-116">Endereço (endereço IP, FQDN ou URL)</span><span class="sxs-lookup"><span data-stu-id="a2d62-116">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="a2d62-117">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="a2d62-117">isDefaultServer</span></span>|<span data-ttu-id="a2d62-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2d62-118">Boolean</span></span>|<span data-ttu-id="a2d62-119">Servidor padrão.</span><span class="sxs-lookup"><span data-stu-id="a2d62-119">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2d62-120">Relações</span><span class="sxs-lookup"><span data-stu-id="a2d62-120">Relationships</span></span>
<span data-ttu-id="a2d62-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a2d62-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2d62-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2d62-122">JSON Representation</span></span>
<span data-ttu-id="a2d62-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a2d62-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnServer",
  "description": "String",
  "address": "String",
  "isDefaultServer": true
}
```



