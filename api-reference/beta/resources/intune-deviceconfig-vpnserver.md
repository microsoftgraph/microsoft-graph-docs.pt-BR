---
title: tipo de recurso vpnServer
description: Definição do servidor VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 67f0e91c0b2d024a07ab632a5e61e1106bbc65fa
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944520"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="343d8-103">tipo de recurso vpnServer</span><span class="sxs-lookup"><span data-stu-id="343d8-103">vpnServer resource type</span></span>

> <span data-ttu-id="343d8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="343d8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="343d8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="343d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="343d8-106">Definição do servidor VPN.</span><span class="sxs-lookup"><span data-stu-id="343d8-106">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="343d8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="343d8-107">Properties</span></span>
|<span data-ttu-id="343d8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="343d8-108">Property</span></span>|<span data-ttu-id="343d8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="343d8-109">Type</span></span>|<span data-ttu-id="343d8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="343d8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="343d8-111">description</span><span class="sxs-lookup"><span data-stu-id="343d8-111">description</span></span>|<span data-ttu-id="343d8-112">String</span><span class="sxs-lookup"><span data-stu-id="343d8-112">String</span></span>|<span data-ttu-id="343d8-113">Descrição.</span><span class="sxs-lookup"><span data-stu-id="343d8-113">Description.</span></span>|
|<span data-ttu-id="343d8-114">address</span><span class="sxs-lookup"><span data-stu-id="343d8-114">address</span></span>|<span data-ttu-id="343d8-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="343d8-115">String</span></span>|<span data-ttu-id="343d8-116">Endereço (endereço IP, FQDN ou URL)</span><span class="sxs-lookup"><span data-stu-id="343d8-116">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="343d8-117">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="343d8-117">isDefaultServer</span></span>|<span data-ttu-id="343d8-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="343d8-118">Boolean</span></span>|<span data-ttu-id="343d8-119">Servidor padrão.</span><span class="sxs-lookup"><span data-stu-id="343d8-119">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="343d8-120">Relações</span><span class="sxs-lookup"><span data-stu-id="343d8-120">Relationships</span></span>
<span data-ttu-id="343d8-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="343d8-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="343d8-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="343d8-122">JSON Representation</span></span>
<span data-ttu-id="343d8-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="343d8-123">Here is a JSON representation of the resource.</span></span>
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




