---
title: tipo de recurso vpnServer
description: Definição do servidor VPN.
ms.openlocfilehash: e89cc562c3fe0f6b353199ca7de639053177ab1f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036598"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="55e19-103">tipo de recurso vpnServer</span><span class="sxs-lookup"><span data-stu-id="55e19-103">vpnServer resource type</span></span>

> <span data-ttu-id="55e19-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="55e19-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55e19-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="55e19-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="55e19-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="55e19-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55e19-107">Definição do servidor VPN.</span><span class="sxs-lookup"><span data-stu-id="55e19-107">VPN Server definition.</span></span>
## <a name="properties"></a><span data-ttu-id="55e19-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="55e19-108">Properties</span></span>
|<span data-ttu-id="55e19-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55e19-109">Property</span></span>|<span data-ttu-id="55e19-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="55e19-110">Type</span></span>|<span data-ttu-id="55e19-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="55e19-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55e19-112">description</span><span class="sxs-lookup"><span data-stu-id="55e19-112">description</span></span>|<span data-ttu-id="55e19-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55e19-113">String</span></span>|<span data-ttu-id="55e19-114">Descrição.</span><span class="sxs-lookup"><span data-stu-id="55e19-114">Description.</span></span>|
|<span data-ttu-id="55e19-115">address</span><span class="sxs-lookup"><span data-stu-id="55e19-115">address</span></span>|<span data-ttu-id="55e19-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55e19-116">String</span></span>|<span data-ttu-id="55e19-117">Endereço (endereço IP, FQDN ou a URL)</span><span class="sxs-lookup"><span data-stu-id="55e19-117">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="55e19-118">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="55e19-118">isDefaultServer</span></span>|<span data-ttu-id="55e19-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="55e19-119">Boolean</span></span>|<span data-ttu-id="55e19-120">Servidor padrão.</span><span class="sxs-lookup"><span data-stu-id="55e19-120">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55e19-121">Relações</span><span class="sxs-lookup"><span data-stu-id="55e19-121">Relationships</span></span>
<span data-ttu-id="55e19-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="55e19-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="55e19-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="55e19-123">JSON Representation</span></span>
<span data-ttu-id="55e19-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="55e19-124">Here is a JSON representation of the resource.</span></span>
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





