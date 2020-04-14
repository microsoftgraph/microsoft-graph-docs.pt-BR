---
title: tipo de recurso vpnServer
description: Definição do servidor VPN.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f687167b62e6b3a56f1deb76e3ee90c6ea7c62b7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420267"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="b3acd-103">tipo de recurso vpnServer</span><span class="sxs-lookup"><span data-stu-id="b3acd-103">vpnServer resource type</span></span>

<span data-ttu-id="b3acd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3acd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3acd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b3acd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3acd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b3acd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3acd-107">Definição do servidor VPN.</span><span class="sxs-lookup"><span data-stu-id="b3acd-107">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="b3acd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b3acd-108">Properties</span></span>
|<span data-ttu-id="b3acd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3acd-109">Property</span></span>|<span data-ttu-id="b3acd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3acd-110">Type</span></span>|<span data-ttu-id="b3acd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3acd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3acd-112">description</span><span class="sxs-lookup"><span data-stu-id="b3acd-112">description</span></span>|<span data-ttu-id="b3acd-113">String</span><span class="sxs-lookup"><span data-stu-id="b3acd-113">String</span></span>|<span data-ttu-id="b3acd-114">Descrição.</span><span class="sxs-lookup"><span data-stu-id="b3acd-114">Description.</span></span>|
|<span data-ttu-id="b3acd-115">address</span><span class="sxs-lookup"><span data-stu-id="b3acd-115">address</span></span>|<span data-ttu-id="b3acd-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3acd-116">String</span></span>|<span data-ttu-id="b3acd-117">Endereço (endereço IP, FQDN ou URL)</span><span class="sxs-lookup"><span data-stu-id="b3acd-117">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="b3acd-118">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="b3acd-118">isDefaultServer</span></span>|<span data-ttu-id="b3acd-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3acd-119">Boolean</span></span>|<span data-ttu-id="b3acd-120">Servidor padrão.</span><span class="sxs-lookup"><span data-stu-id="b3acd-120">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3acd-121">Relações</span><span class="sxs-lookup"><span data-stu-id="b3acd-121">Relationships</span></span>
<span data-ttu-id="b3acd-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b3acd-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3acd-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b3acd-123">JSON Representation</span></span>
<span data-ttu-id="b3acd-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b3acd-124">Here is a JSON representation of the resource.</span></span>
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



