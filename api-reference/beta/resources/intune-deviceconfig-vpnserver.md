---
title: tipo de recurso vpnServer
description: Definição do servidor VPN.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0bf45848059f7cbd74b408b4074b0ebc5c31b4e5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573470"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="4b79c-103">tipo de recurso vpnServer</span><span class="sxs-lookup"><span data-stu-id="4b79c-103">vpnServer resource type</span></span>

> <span data-ttu-id="4b79c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4b79c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b79c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4b79c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b79c-106">Definição do servidor VPN.</span><span class="sxs-lookup"><span data-stu-id="4b79c-106">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="4b79c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4b79c-107">Properties</span></span>
|<span data-ttu-id="4b79c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b79c-108">Property</span></span>|<span data-ttu-id="4b79c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b79c-109">Type</span></span>|<span data-ttu-id="4b79c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b79c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b79c-111">description</span><span class="sxs-lookup"><span data-stu-id="4b79c-111">description</span></span>|<span data-ttu-id="4b79c-112">String</span><span class="sxs-lookup"><span data-stu-id="4b79c-112">String</span></span>|<span data-ttu-id="4b79c-113">Descrição.</span><span class="sxs-lookup"><span data-stu-id="4b79c-113">Description.</span></span>|
|<span data-ttu-id="4b79c-114">address</span><span class="sxs-lookup"><span data-stu-id="4b79c-114">address</span></span>|<span data-ttu-id="4b79c-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b79c-115">String</span></span>|<span data-ttu-id="4b79c-116">Endereço (endereço IP, FQDN ou URL)</span><span class="sxs-lookup"><span data-stu-id="4b79c-116">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="4b79c-117">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="4b79c-117">isDefaultServer</span></span>|<span data-ttu-id="4b79c-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="4b79c-118">Boolean</span></span>|<span data-ttu-id="4b79c-119">Servidor padrão.</span><span class="sxs-lookup"><span data-stu-id="4b79c-119">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b79c-120">Relações</span><span class="sxs-lookup"><span data-stu-id="4b79c-120">Relationships</span></span>
<span data-ttu-id="4b79c-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4b79c-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b79c-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4b79c-122">JSON Representation</span></span>
<span data-ttu-id="4b79c-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4b79c-123">Here is a JSON representation of the resource.</span></span>
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





