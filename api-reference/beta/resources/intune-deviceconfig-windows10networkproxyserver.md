---
title: Tipo de recurso windows10NetworkProxyServer
description: Política de Servidor Proxy de Rede.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 120eff89a01434803c1e2f4f5ba84d3f088e1022
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571958"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="b0e99-103">Tipo de recurso windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="b0e99-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="b0e99-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b0e99-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0e99-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0e99-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0e99-106">Política de Servidor Proxy de Rede.</span><span class="sxs-lookup"><span data-stu-id="b0e99-106">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="b0e99-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0e99-107">Properties</span></span>
|<span data-ttu-id="b0e99-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0e99-108">Property</span></span>|<span data-ttu-id="b0e99-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0e99-109">Type</span></span>|<span data-ttu-id="b0e99-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0e99-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0e99-111">address</span><span class="sxs-lookup"><span data-stu-id="b0e99-111">address</span></span>|<span data-ttu-id="b0e99-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0e99-112">String</span></span>|<span data-ttu-id="b0e99-113">Endereço para o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="b0e99-113">Address to the proxy server.</span></span> <span data-ttu-id="b0e99-114">Especifique um endereço no formato <server>\[“:”<port>\]</span><span class="sxs-lookup"><span data-stu-id="b0e99-114">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="b0e99-115">exceptions</span><span class="sxs-lookup"><span data-stu-id="b0e99-115">exceptions</span></span>|<span data-ttu-id="b0e99-116">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0e99-116">String collection</span></span>|<span data-ttu-id="b0e99-117">Endereços que não devem usar o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="b0e99-117">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="b0e99-118">O sistema não usará o servidor proxy para endereços que começam com o conteúdo especificado nesse nó.</span><span class="sxs-lookup"><span data-stu-id="b0e99-118">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="b0e99-119">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="b0e99-119">useForLocalAddresses</span></span>|<span data-ttu-id="b0e99-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0e99-120">Boolean</span></span>|<span data-ttu-id="b0e99-121">Especifica se o servidor proxy deve ser usado para endereços locais (intranet).</span><span class="sxs-lookup"><span data-stu-id="b0e99-121">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0e99-122">Relações</span><span class="sxs-lookup"><span data-stu-id="b0e99-122">Relationships</span></span>
<span data-ttu-id="b0e99-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b0e99-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0e99-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0e99-124">JSON Representation</span></span>
<span data-ttu-id="b0e99-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0e99-125">Here is a JSON representation of the resource.</span></span>
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





