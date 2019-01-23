---
title: tipo de recurso vpnServer
description: Definição do servidor VPN.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0febdae5745f1295e9c690213d4a51b79d7d3bdb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406805"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="e01d3-103">tipo de recurso vpnServer</span><span class="sxs-lookup"><span data-stu-id="e01d3-103">vpnServer resource type</span></span>

> <span data-ttu-id="e01d3-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="e01d3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e01d3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e01d3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e01d3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e01d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e01d3-107">Definição do servidor VPN.</span><span class="sxs-lookup"><span data-stu-id="e01d3-107">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="e01d3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e01d3-108">Properties</span></span>
|<span data-ttu-id="e01d3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e01d3-109">Property</span></span>|<span data-ttu-id="e01d3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e01d3-110">Type</span></span>|<span data-ttu-id="e01d3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e01d3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e01d3-112">description</span><span class="sxs-lookup"><span data-stu-id="e01d3-112">description</span></span>|<span data-ttu-id="e01d3-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e01d3-113">String</span></span>|<span data-ttu-id="e01d3-114">Descrição.</span><span class="sxs-lookup"><span data-stu-id="e01d3-114">Description.</span></span>|
|<span data-ttu-id="e01d3-115">address</span><span class="sxs-lookup"><span data-stu-id="e01d3-115">address</span></span>|<span data-ttu-id="e01d3-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e01d3-116">String</span></span>|<span data-ttu-id="e01d3-117">Endereço (endereço IP, FQDN ou a URL)</span><span class="sxs-lookup"><span data-stu-id="e01d3-117">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="e01d3-118">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="e01d3-118">isDefaultServer</span></span>|<span data-ttu-id="e01d3-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="e01d3-119">Boolean</span></span>|<span data-ttu-id="e01d3-120">Servidor padrão.</span><span class="sxs-lookup"><span data-stu-id="e01d3-120">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e01d3-121">Relações</span><span class="sxs-lookup"><span data-stu-id="e01d3-121">Relationships</span></span>
<span data-ttu-id="e01d3-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e01d3-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e01d3-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e01d3-123">JSON Representation</span></span>
<span data-ttu-id="e01d3-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e01d3-124">Here is a JSON representation of the resource.</span></span>
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




