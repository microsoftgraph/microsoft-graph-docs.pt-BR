---
title: tipo de recurso de vpnProxyServer
description: Servidor de Proxy VPN.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 727d26af7f2c1801cd06fc98949109efec267f27
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955349"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="1fbc7-103">tipo de recurso de vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="1fbc7-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="1fbc7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1fbc7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1fbc7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1fbc7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1fbc7-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1fbc7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1fbc7-107">Servidor de Proxy VPN.</span><span class="sxs-lookup"><span data-stu-id="1fbc7-107">VPN Proxy Server.</span></span>
## <a name="properties"></a><span data-ttu-id="1fbc7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1fbc7-108">Properties</span></span>
|<span data-ttu-id="1fbc7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1fbc7-109">Property</span></span>|<span data-ttu-id="1fbc7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fbc7-110">Type</span></span>|<span data-ttu-id="1fbc7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fbc7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fbc7-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="1fbc7-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="1fbc7-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1fbc7-113">String</span></span>|<span data-ttu-id="1fbc7-114">Url de script de configuração automática do proxy.</span><span class="sxs-lookup"><span data-stu-id="1fbc7-114">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="1fbc7-115">address</span><span class="sxs-lookup"><span data-stu-id="1fbc7-115">address</span></span>|<span data-ttu-id="1fbc7-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1fbc7-116">String</span></span>|<span data-ttu-id="1fbc7-117">Endereço.</span><span class="sxs-lookup"><span data-stu-id="1fbc7-117">Address.</span></span>|
|<span data-ttu-id="1fbc7-118">porta</span><span class="sxs-lookup"><span data-stu-id="1fbc7-118">port</span></span>|<span data-ttu-id="1fbc7-119">Int32</span><span class="sxs-lookup"><span data-stu-id="1fbc7-119">Int32</span></span>|<span data-ttu-id="1fbc7-120">Porta.</span><span class="sxs-lookup"><span data-stu-id="1fbc7-120">Port.</span></span> <span data-ttu-id="1fbc7-121">0 a 65.535 os valores válidos</span><span class="sxs-lookup"><span data-stu-id="1fbc7-121">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="1fbc7-122">Relações</span><span class="sxs-lookup"><span data-stu-id="1fbc7-122">Relationships</span></span>
<span data-ttu-id="1fbc7-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1fbc7-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1fbc7-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1fbc7-124">JSON Representation</span></span>
<span data-ttu-id="1fbc7-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1fbc7-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024
}
```





