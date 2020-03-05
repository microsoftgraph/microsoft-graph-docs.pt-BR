---
title: Tipo de recurso windows10NetworkProxyServer
description: Política de Servidor Proxy de Rede.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f2c8002423f394decbb2d52e9163581e4f254c92
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525639"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="1d974-103">Tipo de recurso windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="1d974-103">windows10NetworkProxyServer resource type</span></span>

<span data-ttu-id="1d974-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1d974-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d974-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1d974-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d974-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1d974-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d974-107">Política de Servidor Proxy de Rede.</span><span class="sxs-lookup"><span data-stu-id="1d974-107">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="1d974-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d974-108">Properties</span></span>
|<span data-ttu-id="1d974-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d974-109">Property</span></span>|<span data-ttu-id="1d974-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d974-110">Type</span></span>|<span data-ttu-id="1d974-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d974-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d974-112">address</span><span class="sxs-lookup"><span data-stu-id="1d974-112">address</span></span>|<span data-ttu-id="1d974-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d974-113">String</span></span>|<span data-ttu-id="1d974-114">Endereço para o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="1d974-114">Address to the proxy server.</span></span> <span data-ttu-id="1d974-115">Especifique um endereço no formato <server>\[“:”<port>\]</span><span class="sxs-lookup"><span data-stu-id="1d974-115">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="1d974-116">exceptions</span><span class="sxs-lookup"><span data-stu-id="1d974-116">exceptions</span></span>|<span data-ttu-id="1d974-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d974-117">String collection</span></span>|<span data-ttu-id="1d974-118">Endereços que não devem usar o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="1d974-118">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="1d974-119">O sistema não usará o servidor proxy para endereços que começam com o conteúdo especificado nesse nó.</span><span class="sxs-lookup"><span data-stu-id="1d974-119">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="1d974-120">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="1d974-120">useForLocalAddresses</span></span>|<span data-ttu-id="1d974-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d974-121">Boolean</span></span>|<span data-ttu-id="1d974-122">Especifica se o servidor proxy deve ser usado para endereços locais (intranet).</span><span class="sxs-lookup"><span data-stu-id="1d974-122">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d974-123">Relações</span><span class="sxs-lookup"><span data-stu-id="1d974-123">Relationships</span></span>
<span data-ttu-id="1d974-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1d974-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d974-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d974-125">JSON Representation</span></span>
<span data-ttu-id="1d974-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d974-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10NetworkProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10NetworkProxyServer",
  "address": "String",
  "exceptions": [
    "String"
  ],
  "useForLocalAddresses": true
}
```



