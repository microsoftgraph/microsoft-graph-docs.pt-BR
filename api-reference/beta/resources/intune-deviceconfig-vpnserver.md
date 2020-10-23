---
title: tipo de recurso vpnServer
description: Definição do servidor VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c2fda07e416c43246a035b556e6ee23f36ff56a1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728311"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="9724d-103">tipo de recurso vpnServer</span><span class="sxs-lookup"><span data-stu-id="9724d-103">vpnServer resource type</span></span>

<span data-ttu-id="9724d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9724d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9724d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9724d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9724d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9724d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9724d-107">Definição do servidor VPN.</span><span class="sxs-lookup"><span data-stu-id="9724d-107">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="9724d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9724d-108">Properties</span></span>
|<span data-ttu-id="9724d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9724d-109">Property</span></span>|<span data-ttu-id="9724d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9724d-110">Type</span></span>|<span data-ttu-id="9724d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9724d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9724d-112">description</span><span class="sxs-lookup"><span data-stu-id="9724d-112">description</span></span>|<span data-ttu-id="9724d-113">String</span><span class="sxs-lookup"><span data-stu-id="9724d-113">String</span></span>|<span data-ttu-id="9724d-114">Descrição.</span><span class="sxs-lookup"><span data-stu-id="9724d-114">Description.</span></span>|
|<span data-ttu-id="9724d-115">address</span><span class="sxs-lookup"><span data-stu-id="9724d-115">address</span></span>|<span data-ttu-id="9724d-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9724d-116">String</span></span>|<span data-ttu-id="9724d-117">Endereço (endereço IP, FQDN ou URL)</span><span class="sxs-lookup"><span data-stu-id="9724d-117">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="9724d-118">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="9724d-118">isDefaultServer</span></span>|<span data-ttu-id="9724d-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="9724d-119">Boolean</span></span>|<span data-ttu-id="9724d-120">Servidor padrão.</span><span class="sxs-lookup"><span data-stu-id="9724d-120">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9724d-121">Relações</span><span class="sxs-lookup"><span data-stu-id="9724d-121">Relationships</span></span>
<span data-ttu-id="9724d-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9724d-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9724d-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9724d-123">JSON Representation</span></span>
<span data-ttu-id="9724d-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9724d-124">Here is a JSON representation of the resource.</span></span>
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





