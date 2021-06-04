---
title: Tipo de recurso windows10NetworkProxyServer
description: Política de Servidor Proxy de Rede.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0c561787c74649c6628768de691510524165f43f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52742731"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="f1f9f-103">Tipo de recurso windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="f1f9f-103">windows10NetworkProxyServer resource type</span></span>

<span data-ttu-id="f1f9f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1f9f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1f9f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f1f9f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1f9f-106">Política de Servidor Proxy de Rede.</span><span class="sxs-lookup"><span data-stu-id="f1f9f-106">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="f1f9f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f1f9f-107">Properties</span></span>
|<span data-ttu-id="f1f9f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1f9f-108">Property</span></span>|<span data-ttu-id="f1f9f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1f9f-109">Type</span></span>|<span data-ttu-id="f1f9f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1f9f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1f9f-111">address</span><span class="sxs-lookup"><span data-stu-id="f1f9f-111">address</span></span>|<span data-ttu-id="f1f9f-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1f9f-112">String</span></span>|<span data-ttu-id="f1f9f-113">Endereço para o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="f1f9f-113">Address to the proxy server.</span></span> <span data-ttu-id="f1f9f-114">Especifique um endereço no formato <server>\[“:”<port>\]</span><span class="sxs-lookup"><span data-stu-id="f1f9f-114">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="f1f9f-115">exceptions</span><span class="sxs-lookup"><span data-stu-id="f1f9f-115">exceptions</span></span>|<span data-ttu-id="f1f9f-116">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1f9f-116">String collection</span></span>|<span data-ttu-id="f1f9f-117">Endereços que não devem usar o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="f1f9f-117">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="f1f9f-118">O sistema não usará o servidor proxy para endereços que começam com o conteúdo especificado nesse nó.</span><span class="sxs-lookup"><span data-stu-id="f1f9f-118">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="f1f9f-119">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="f1f9f-119">useForLocalAddresses</span></span>|<span data-ttu-id="f1f9f-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="f1f9f-120">Boolean</span></span>|<span data-ttu-id="f1f9f-121">Especifica se o servidor proxy deve ser usado para endereços locais (intranet).</span><span class="sxs-lookup"><span data-stu-id="f1f9f-121">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1f9f-122">Relações</span><span class="sxs-lookup"><span data-stu-id="f1f9f-122">Relationships</span></span>
<span data-ttu-id="f1f9f-123">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="f1f9f-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1f9f-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f1f9f-124">JSON Representation</span></span>
<span data-ttu-id="f1f9f-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f1f9f-125">Here is a JSON representation of the resource.</span></span>
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




