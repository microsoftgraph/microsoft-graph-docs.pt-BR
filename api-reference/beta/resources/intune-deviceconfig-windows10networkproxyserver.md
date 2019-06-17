---
title: Tipo de recurso windows10NetworkProxyServer
description: Política de Servidor Proxy de Rede.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b8424a31686605cd0c992d696e2db21350347c6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34982186"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="0d2aa-103">Tipo de recurso windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="0d2aa-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="0d2aa-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0d2aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d2aa-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0d2aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d2aa-106">Política de Servidor Proxy de Rede.</span><span class="sxs-lookup"><span data-stu-id="0d2aa-106">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="0d2aa-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0d2aa-107">Properties</span></span>
|<span data-ttu-id="0d2aa-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d2aa-108">Property</span></span>|<span data-ttu-id="0d2aa-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d2aa-109">Type</span></span>|<span data-ttu-id="0d2aa-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d2aa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d2aa-111">address</span><span class="sxs-lookup"><span data-stu-id="0d2aa-111">address</span></span>|<span data-ttu-id="0d2aa-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0d2aa-112">String</span></span>|<span data-ttu-id="0d2aa-113">Endereço para o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="0d2aa-113">Address to the proxy server.</span></span> <span data-ttu-id="0d2aa-114">Especifique um endereço no formato <server>\[“:”<port>\]</span><span class="sxs-lookup"><span data-stu-id="0d2aa-114">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="0d2aa-115">exceptions</span><span class="sxs-lookup"><span data-stu-id="0d2aa-115">exceptions</span></span>|<span data-ttu-id="0d2aa-116">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0d2aa-116">String collection</span></span>|<span data-ttu-id="0d2aa-117">Endereços que não devem usar o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="0d2aa-117">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="0d2aa-118">O sistema não usará o servidor proxy para endereços que começam com o conteúdo especificado nesse nó.</span><span class="sxs-lookup"><span data-stu-id="0d2aa-118">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="0d2aa-119">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="0d2aa-119">useForLocalAddresses</span></span>|<span data-ttu-id="0d2aa-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="0d2aa-120">Boolean</span></span>|<span data-ttu-id="0d2aa-121">Especifica se o servidor proxy deve ser usado para endereços locais (intranet).</span><span class="sxs-lookup"><span data-stu-id="0d2aa-121">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d2aa-122">Relações</span><span class="sxs-lookup"><span data-stu-id="0d2aa-122">Relationships</span></span>
<span data-ttu-id="0d2aa-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0d2aa-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d2aa-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0d2aa-124">JSON Representation</span></span>
<span data-ttu-id="0d2aa-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0d2aa-125">Here is a JSON representation of the resource.</span></span>
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





