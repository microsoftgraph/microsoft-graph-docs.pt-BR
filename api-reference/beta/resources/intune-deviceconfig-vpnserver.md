---
title: tipo de recurso vpnServer
description: Definição do servidor VPN.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0bf45848059f7cbd74b408b4074b0ebc5c31b4e5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782832"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="bdabc-103">tipo de recurso vpnServer</span><span class="sxs-lookup"><span data-stu-id="bdabc-103">vpnServer resource type</span></span>

> <span data-ttu-id="bdabc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bdabc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bdabc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bdabc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdabc-106">Definição do servidor VPN.</span><span class="sxs-lookup"><span data-stu-id="bdabc-106">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="bdabc-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bdabc-107">Properties</span></span>
|<span data-ttu-id="bdabc-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bdabc-108">Property</span></span>|<span data-ttu-id="bdabc-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdabc-109">Type</span></span>|<span data-ttu-id="bdabc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdabc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdabc-111">description</span><span class="sxs-lookup"><span data-stu-id="bdabc-111">description</span></span>|<span data-ttu-id="bdabc-112">String</span><span class="sxs-lookup"><span data-stu-id="bdabc-112">String</span></span>|<span data-ttu-id="bdabc-113">Descrição.</span><span class="sxs-lookup"><span data-stu-id="bdabc-113">Description.</span></span>|
|<span data-ttu-id="bdabc-114">address</span><span class="sxs-lookup"><span data-stu-id="bdabc-114">address</span></span>|<span data-ttu-id="bdabc-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdabc-115">String</span></span>|<span data-ttu-id="bdabc-116">Endereço (endereço IP, FQDN ou URL)</span><span class="sxs-lookup"><span data-stu-id="bdabc-116">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="bdabc-117">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="bdabc-117">isDefaultServer</span></span>|<span data-ttu-id="bdabc-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="bdabc-118">Boolean</span></span>|<span data-ttu-id="bdabc-119">Servidor padrão.</span><span class="sxs-lookup"><span data-stu-id="bdabc-119">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdabc-120">Relações</span><span class="sxs-lookup"><span data-stu-id="bdabc-120">Relationships</span></span>
<span data-ttu-id="bdabc-121">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="bdabc-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bdabc-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bdabc-122">JSON Representation</span></span>
<span data-ttu-id="bdabc-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bdabc-123">Here is a JSON representation of the resource.</span></span>
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





