---
title: tipo de recurso vpnServer
description: Definição do servidor VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8281aaaec193b5a78e913af52ce51d8f327ce8cf
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279476"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="b09f1-103">tipo de recurso vpnServer</span><span class="sxs-lookup"><span data-stu-id="b09f1-103">vpnServer resource type</span></span>

<span data-ttu-id="b09f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b09f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b09f1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b09f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b09f1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b09f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b09f1-107">Definição do servidor VPN.</span><span class="sxs-lookup"><span data-stu-id="b09f1-107">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="b09f1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b09f1-108">Properties</span></span>
|<span data-ttu-id="b09f1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b09f1-109">Property</span></span>|<span data-ttu-id="b09f1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b09f1-110">Type</span></span>|<span data-ttu-id="b09f1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b09f1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b09f1-112">description</span><span class="sxs-lookup"><span data-stu-id="b09f1-112">description</span></span>|<span data-ttu-id="b09f1-113">String</span><span class="sxs-lookup"><span data-stu-id="b09f1-113">String</span></span>|<span data-ttu-id="b09f1-114">Descrição.</span><span class="sxs-lookup"><span data-stu-id="b09f1-114">Description.</span></span>|
|<span data-ttu-id="b09f1-115">address</span><span class="sxs-lookup"><span data-stu-id="b09f1-115">address</span></span>|<span data-ttu-id="b09f1-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b09f1-116">String</span></span>|<span data-ttu-id="b09f1-117">Endereço (endereço IP, FQDN ou URL)</span><span class="sxs-lookup"><span data-stu-id="b09f1-117">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="b09f1-118">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="b09f1-118">isDefaultServer</span></span>|<span data-ttu-id="b09f1-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="b09f1-119">Boolean</span></span>|<span data-ttu-id="b09f1-120">Servidor padrão.</span><span class="sxs-lookup"><span data-stu-id="b09f1-120">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b09f1-121">Relações</span><span class="sxs-lookup"><span data-stu-id="b09f1-121">Relationships</span></span>
<span data-ttu-id="b09f1-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b09f1-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b09f1-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b09f1-123">JSON Representation</span></span>
<span data-ttu-id="b09f1-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b09f1-124">Here is a JSON representation of the resource.</span></span>
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




