---
title: tipo de recurso vpnServer
description: Definição do servidor VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 540741a6b3df349e5a096070e7973e3dadc2533e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987513"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="5f819-103">tipo de recurso vpnServer</span><span class="sxs-lookup"><span data-stu-id="5f819-103">vpnServer resource type</span></span>

> <span data-ttu-id="5f819-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5f819-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f819-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5f819-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f819-106">Definição do servidor VPN.</span><span class="sxs-lookup"><span data-stu-id="5f819-106">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="5f819-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5f819-107">Properties</span></span>
|<span data-ttu-id="5f819-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f819-108">Property</span></span>|<span data-ttu-id="5f819-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f819-109">Type</span></span>|<span data-ttu-id="5f819-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f819-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f819-111">description</span><span class="sxs-lookup"><span data-stu-id="5f819-111">description</span></span>|<span data-ttu-id="5f819-112">String</span><span class="sxs-lookup"><span data-stu-id="5f819-112">String</span></span>|<span data-ttu-id="5f819-113">Descrição.</span><span class="sxs-lookup"><span data-stu-id="5f819-113">Description.</span></span>|
|<span data-ttu-id="5f819-114">address</span><span class="sxs-lookup"><span data-stu-id="5f819-114">address</span></span>|<span data-ttu-id="5f819-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f819-115">String</span></span>|<span data-ttu-id="5f819-116">Endereço (endereço IP, FQDN ou URL)</span><span class="sxs-lookup"><span data-stu-id="5f819-116">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="5f819-117">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="5f819-117">isDefaultServer</span></span>|<span data-ttu-id="5f819-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="5f819-118">Boolean</span></span>|<span data-ttu-id="5f819-119">Servidor padrão.</span><span class="sxs-lookup"><span data-stu-id="5f819-119">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f819-120">Relações</span><span class="sxs-lookup"><span data-stu-id="5f819-120">Relationships</span></span>
<span data-ttu-id="5f819-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5f819-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f819-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5f819-122">JSON Representation</span></span>
<span data-ttu-id="5f819-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5f819-123">Here is a JSON representation of the resource.</span></span>
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





