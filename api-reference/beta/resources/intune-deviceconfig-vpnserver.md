---
title: tipo de recurso vpnServer
description: Definição do servidor VPN.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b48daa95cc2227f6d1691902a75614446c93a10a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889870"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="d358f-103">tipo de recurso vpnServer</span><span class="sxs-lookup"><span data-stu-id="d358f-103">vpnServer resource type</span></span>

> <span data-ttu-id="d358f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d358f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d358f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d358f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d358f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d358f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d358f-107">Definição do servidor VPN.</span><span class="sxs-lookup"><span data-stu-id="d358f-107">VPN Server definition.</span></span>
## <a name="properties"></a><span data-ttu-id="d358f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d358f-108">Properties</span></span>
|<span data-ttu-id="d358f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d358f-109">Property</span></span>|<span data-ttu-id="d358f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d358f-110">Type</span></span>|<span data-ttu-id="d358f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d358f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d358f-112">description</span><span class="sxs-lookup"><span data-stu-id="d358f-112">description</span></span>|<span data-ttu-id="d358f-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d358f-113">String</span></span>|<span data-ttu-id="d358f-114">Descrição.</span><span class="sxs-lookup"><span data-stu-id="d358f-114">Description.</span></span>|
|<span data-ttu-id="d358f-115">address</span><span class="sxs-lookup"><span data-stu-id="d358f-115">address</span></span>|<span data-ttu-id="d358f-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d358f-116">String</span></span>|<span data-ttu-id="d358f-117">Endereço (endereço IP, FQDN ou a URL)</span><span class="sxs-lookup"><span data-stu-id="d358f-117">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="d358f-118">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="d358f-118">isDefaultServer</span></span>|<span data-ttu-id="d358f-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="d358f-119">Boolean</span></span>|<span data-ttu-id="d358f-120">Servidor padrão.</span><span class="sxs-lookup"><span data-stu-id="d358f-120">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d358f-121">Relações</span><span class="sxs-lookup"><span data-stu-id="d358f-121">Relationships</span></span>
<span data-ttu-id="d358f-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d358f-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d358f-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d358f-123">JSON Representation</span></span>
<span data-ttu-id="d358f-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d358f-124">Here is a JSON representation of the resource.</span></span>
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





