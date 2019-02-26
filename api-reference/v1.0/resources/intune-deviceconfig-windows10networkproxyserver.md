---
title: Tipo de recurso windows10NetworkProxyServer
description: Política de Servidor Proxy de Rede.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1dfe20e52ad63cf1d0d6a958f2ef5f4f89a53ad6
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260694"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="3a54b-103">Tipo de recurso windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="3a54b-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="3a54b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3a54b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a54b-105">Política de Servidor Proxy de Rede.</span><span class="sxs-lookup"><span data-stu-id="3a54b-105">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="3a54b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a54b-106">Properties</span></span>
|<span data-ttu-id="3a54b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a54b-107">Property</span></span>|<span data-ttu-id="3a54b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a54b-108">Type</span></span>|<span data-ttu-id="3a54b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a54b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a54b-110">address</span><span class="sxs-lookup"><span data-stu-id="3a54b-110">address</span></span>|<span data-ttu-id="3a54b-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a54b-111">String</span></span>|<span data-ttu-id="3a54b-112">Endereço para o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="3a54b-112">Address to the proxy server.</span></span> <span data-ttu-id="3a54b-113">Especifique um endereço no formato <server>\[“:”<port>\]</span><span class="sxs-lookup"><span data-stu-id="3a54b-113">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="3a54b-114">exceptions</span><span class="sxs-lookup"><span data-stu-id="3a54b-114">exceptions</span></span>|<span data-ttu-id="3a54b-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a54b-115">String collection</span></span>|<span data-ttu-id="3a54b-116">Endereços que não devem usar o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="3a54b-116">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="3a54b-117">O sistema não usará o servidor proxy para endereços que começam com o conteúdo especificado nesse nó.</span><span class="sxs-lookup"><span data-stu-id="3a54b-117">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="3a54b-118">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="3a54b-118">useForLocalAddresses</span></span>|<span data-ttu-id="3a54b-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="3a54b-119">Boolean</span></span>|<span data-ttu-id="3a54b-120">Especifica se o servidor proxy deve ser usado para endereços locais (intranet).</span><span class="sxs-lookup"><span data-stu-id="3a54b-120">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a54b-121">Relações</span><span class="sxs-lookup"><span data-stu-id="3a54b-121">Relationships</span></span>
<span data-ttu-id="3a54b-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3a54b-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a54b-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a54b-123">JSON Representation</span></span>
<span data-ttu-id="3a54b-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a54b-124">Here is a JSON representation of the resource.</span></span>
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



