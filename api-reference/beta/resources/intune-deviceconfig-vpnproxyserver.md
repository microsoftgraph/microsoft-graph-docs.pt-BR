---
title: tipo de recurso de vpnProxyServer
description: Servidor de Proxy VPN.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 676e56771f021a79179e268280f5e3190754eef2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425670"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="653e0-103">tipo de recurso de vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="653e0-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="653e0-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="653e0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="653e0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="653e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="653e0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="653e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="653e0-107">Servidor de Proxy VPN.</span><span class="sxs-lookup"><span data-stu-id="653e0-107">VPN Proxy Server.</span></span>

## <a name="properties"></a><span data-ttu-id="653e0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="653e0-108">Properties</span></span>
|<span data-ttu-id="653e0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="653e0-109">Property</span></span>|<span data-ttu-id="653e0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="653e0-110">Type</span></span>|<span data-ttu-id="653e0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="653e0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="653e0-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="653e0-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="653e0-113">String</span><span class="sxs-lookup"><span data-stu-id="653e0-113">String</span></span>|<span data-ttu-id="653e0-114">Url de script de configuração automática do proxy.</span><span class="sxs-lookup"><span data-stu-id="653e0-114">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="653e0-115">address</span><span class="sxs-lookup"><span data-stu-id="653e0-115">address</span></span>|<span data-ttu-id="653e0-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="653e0-116">String</span></span>|<span data-ttu-id="653e0-117">Endereço.</span><span class="sxs-lookup"><span data-stu-id="653e0-117">Address.</span></span>|
|<span data-ttu-id="653e0-118">porta</span><span class="sxs-lookup"><span data-stu-id="653e0-118">port</span></span>|<span data-ttu-id="653e0-119">Int32</span><span class="sxs-lookup"><span data-stu-id="653e0-119">Int32</span></span>|<span data-ttu-id="653e0-120">Porta.</span><span class="sxs-lookup"><span data-stu-id="653e0-120">Port.</span></span> <span data-ttu-id="653e0-121">0 a 65.535 os valores válidos</span><span class="sxs-lookup"><span data-stu-id="653e0-121">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="653e0-122">Relações</span><span class="sxs-lookup"><span data-stu-id="653e0-122">Relationships</span></span>
<span data-ttu-id="653e0-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="653e0-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="653e0-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="653e0-124">JSON Representation</span></span>
<span data-ttu-id="653e0-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="653e0-125">Here is a JSON representation of the resource.</span></span>
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




