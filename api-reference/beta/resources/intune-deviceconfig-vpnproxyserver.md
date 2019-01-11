---
title: tipo de recurso de vpnProxyServer
description: Servidor de Proxy VPN.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3b4842444bc248e51e1967fcbef4a863ed50498c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867673"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="cb10c-103">tipo de recurso de vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="cb10c-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="cb10c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cb10c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb10c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cb10c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cb10c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cb10c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb10c-107">Servidor de Proxy VPN.</span><span class="sxs-lookup"><span data-stu-id="cb10c-107">VPN Proxy Server.</span></span>
## <a name="properties"></a><span data-ttu-id="cb10c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cb10c-108">Properties</span></span>
|<span data-ttu-id="cb10c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb10c-109">Property</span></span>|<span data-ttu-id="cb10c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb10c-110">Type</span></span>|<span data-ttu-id="cb10c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb10c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb10c-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="cb10c-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="cb10c-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb10c-113">String</span></span>|<span data-ttu-id="cb10c-114">Url de script de configuração automática do proxy.</span><span class="sxs-lookup"><span data-stu-id="cb10c-114">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="cb10c-115">address</span><span class="sxs-lookup"><span data-stu-id="cb10c-115">address</span></span>|<span data-ttu-id="cb10c-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb10c-116">String</span></span>|<span data-ttu-id="cb10c-117">Endereço.</span><span class="sxs-lookup"><span data-stu-id="cb10c-117">Address.</span></span>|
|<span data-ttu-id="cb10c-118">porta</span><span class="sxs-lookup"><span data-stu-id="cb10c-118">port</span></span>|<span data-ttu-id="cb10c-119">Int32</span><span class="sxs-lookup"><span data-stu-id="cb10c-119">Int32</span></span>|<span data-ttu-id="cb10c-120">Porta.</span><span class="sxs-lookup"><span data-stu-id="cb10c-120">Port.</span></span> <span data-ttu-id="cb10c-121">0 a 65.535 os valores válidos</span><span class="sxs-lookup"><span data-stu-id="cb10c-121">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb10c-122">Relações</span><span class="sxs-lookup"><span data-stu-id="cb10c-122">Relationships</span></span>
<span data-ttu-id="cb10c-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cb10c-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cb10c-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cb10c-124">JSON Representation</span></span>
<span data-ttu-id="cb10c-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cb10c-125">Here is a JSON representation of the resource.</span></span>
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





