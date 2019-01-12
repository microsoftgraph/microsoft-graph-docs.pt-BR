---
title: tipo de recurso vpnServer
description: Definição do servidor VPN.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 61eaedb7ecca3f4a7074d079f2b10164dfe2ad76
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969545"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="b0200-103">tipo de recurso vpnServer</span><span class="sxs-lookup"><span data-stu-id="b0200-103">vpnServer resource type</span></span>

> <span data-ttu-id="b0200-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b0200-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0200-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b0200-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b0200-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b0200-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0200-107">Definição do servidor VPN.</span><span class="sxs-lookup"><span data-stu-id="b0200-107">VPN Server definition.</span></span>
## <a name="properties"></a><span data-ttu-id="b0200-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0200-108">Properties</span></span>
|<span data-ttu-id="b0200-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0200-109">Property</span></span>|<span data-ttu-id="b0200-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0200-110">Type</span></span>|<span data-ttu-id="b0200-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0200-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0200-112">description</span><span class="sxs-lookup"><span data-stu-id="b0200-112">description</span></span>|<span data-ttu-id="b0200-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0200-113">String</span></span>|<span data-ttu-id="b0200-114">Descrição.</span><span class="sxs-lookup"><span data-stu-id="b0200-114">Description.</span></span>|
|<span data-ttu-id="b0200-115">address</span><span class="sxs-lookup"><span data-stu-id="b0200-115">address</span></span>|<span data-ttu-id="b0200-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0200-116">String</span></span>|<span data-ttu-id="b0200-117">Endereço (endereço IP, FQDN ou a URL)</span><span class="sxs-lookup"><span data-stu-id="b0200-117">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="b0200-118">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="b0200-118">isDefaultServer</span></span>|<span data-ttu-id="b0200-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0200-119">Boolean</span></span>|<span data-ttu-id="b0200-120">Servidor padrão.</span><span class="sxs-lookup"><span data-stu-id="b0200-120">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0200-121">Relações</span><span class="sxs-lookup"><span data-stu-id="b0200-121">Relationships</span></span>
<span data-ttu-id="b0200-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b0200-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b0200-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0200-123">JSON Representation</span></span>
<span data-ttu-id="b0200-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0200-124">Here is a JSON representation of the resource.</span></span>
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





