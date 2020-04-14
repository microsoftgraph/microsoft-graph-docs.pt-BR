---
title: Tipo de recurso windows10NetworkProxyServer
description: Política de Servidor Proxy de Rede.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 56c4b4bd526c69bf9992673aa8ae93d723a2d9bf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456950"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="46e5b-103">Tipo de recurso windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="46e5b-103">windows10NetworkProxyServer resource type</span></span>

<span data-ttu-id="46e5b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46e5b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46e5b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="46e5b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46e5b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="46e5b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46e5b-107">Política de Servidor Proxy de Rede.</span><span class="sxs-lookup"><span data-stu-id="46e5b-107">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="46e5b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="46e5b-108">Properties</span></span>
|<span data-ttu-id="46e5b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46e5b-109">Property</span></span>|<span data-ttu-id="46e5b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="46e5b-110">Type</span></span>|<span data-ttu-id="46e5b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="46e5b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46e5b-112">address</span><span class="sxs-lookup"><span data-stu-id="46e5b-112">address</span></span>|<span data-ttu-id="46e5b-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46e5b-113">String</span></span>|<span data-ttu-id="46e5b-114">Endereço para o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="46e5b-114">Address to the proxy server.</span></span> <span data-ttu-id="46e5b-115">Especifique um endereço no formato <server>\[“:”<port>\]</span><span class="sxs-lookup"><span data-stu-id="46e5b-115">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="46e5b-116">exceptions</span><span class="sxs-lookup"><span data-stu-id="46e5b-116">exceptions</span></span>|<span data-ttu-id="46e5b-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="46e5b-117">String collection</span></span>|<span data-ttu-id="46e5b-118">Endereços que não devem usar o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="46e5b-118">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="46e5b-119">O sistema não usará o servidor proxy para endereços que começam com o conteúdo especificado nesse nó.</span><span class="sxs-lookup"><span data-stu-id="46e5b-119">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="46e5b-120">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="46e5b-120">useForLocalAddresses</span></span>|<span data-ttu-id="46e5b-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="46e5b-121">Boolean</span></span>|<span data-ttu-id="46e5b-122">Especifica se o servidor proxy deve ser usado para endereços locais (intranet).</span><span class="sxs-lookup"><span data-stu-id="46e5b-122">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="46e5b-123">Relações</span><span class="sxs-lookup"><span data-stu-id="46e5b-123">Relationships</span></span>
<span data-ttu-id="46e5b-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="46e5b-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="46e5b-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="46e5b-125">JSON Representation</span></span>
<span data-ttu-id="46e5b-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="46e5b-126">Here is a JSON representation of the resource.</span></span>
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



