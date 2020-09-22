---
title: Tipo de recurso windows10NetworkProxyServer
description: Política de Servidor Proxy de Rede.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 58fd5fb0e46b7458cf9c96c4f1b5d541ba60bf3b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091576"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="a068b-103">Tipo de recurso windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="a068b-103">windows10NetworkProxyServer resource type</span></span>

<span data-ttu-id="a068b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a068b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a068b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a068b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a068b-106">Política de Servidor Proxy de Rede.</span><span class="sxs-lookup"><span data-stu-id="a068b-106">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="a068b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a068b-107">Properties</span></span>
|<span data-ttu-id="a068b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a068b-108">Property</span></span>|<span data-ttu-id="a068b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a068b-109">Type</span></span>|<span data-ttu-id="a068b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a068b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a068b-111">address</span><span class="sxs-lookup"><span data-stu-id="a068b-111">address</span></span>|<span data-ttu-id="a068b-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a068b-112">String</span></span>|<span data-ttu-id="a068b-113">Endereço para o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="a068b-113">Address to the proxy server.</span></span> <span data-ttu-id="a068b-114">Especifique um endereço no formato \<server\> \[ :\<port\>\]</span><span class="sxs-lookup"><span data-stu-id="a068b-114">Specify an address in the format \<server\>\[:\<port\>\]</span></span>|
|<span data-ttu-id="a068b-115">exceptions</span><span class="sxs-lookup"><span data-stu-id="a068b-115">exceptions</span></span>|<span data-ttu-id="a068b-116">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a068b-116">String collection</span></span>|<span data-ttu-id="a068b-117">Endereços que não devem usar o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="a068b-117">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="a068b-118">O sistema não usará o servidor proxy para endereços que começam com o conteúdo especificado nesse nó.</span><span class="sxs-lookup"><span data-stu-id="a068b-118">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="a068b-119">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="a068b-119">useForLocalAddresses</span></span>|<span data-ttu-id="a068b-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="a068b-120">Boolean</span></span>|<span data-ttu-id="a068b-121">Especifica se o servidor proxy deve ser usado para endereços locais (intranet).</span><span class="sxs-lookup"><span data-stu-id="a068b-121">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a068b-122">Relações</span><span class="sxs-lookup"><span data-stu-id="a068b-122">Relationships</span></span>
<span data-ttu-id="a068b-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a068b-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a068b-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a068b-124">JSON Representation</span></span>
<span data-ttu-id="a068b-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a068b-125">Here is a JSON representation of the resource.</span></span>
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









