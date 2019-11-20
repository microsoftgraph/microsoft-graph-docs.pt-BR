---
title: Tipo de recurso windows10NetworkProxyServer
description: Política de Servidor Proxy de Rede.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 88cf36813a6ed7102807917caf0bca3e46744f5f
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2019
ms.locfileid: "38748459"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="23235-103">Tipo de recurso windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="23235-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="23235-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="23235-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23235-105">Política de Servidor Proxy de Rede.</span><span class="sxs-lookup"><span data-stu-id="23235-105">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="23235-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23235-106">Properties</span></span>
|<span data-ttu-id="23235-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23235-107">Property</span></span>|<span data-ttu-id="23235-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="23235-108">Type</span></span>|<span data-ttu-id="23235-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="23235-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23235-110">address</span><span class="sxs-lookup"><span data-stu-id="23235-110">address</span></span>|<span data-ttu-id="23235-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23235-111">String</span></span>|<span data-ttu-id="23235-112">Endereço para o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="23235-112">Address to the proxy server.</span></span> <span data-ttu-id="23235-113">\<Especifique um endereço no servidor\>\[de formato:\<porta\>\]</span><span class="sxs-lookup"><span data-stu-id="23235-113">Specify an address in the format \<server\>\[:\<port\>\]</span></span>|
|<span data-ttu-id="23235-114">exceptions</span><span class="sxs-lookup"><span data-stu-id="23235-114">exceptions</span></span>|<span data-ttu-id="23235-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="23235-115">String collection</span></span>|<span data-ttu-id="23235-116">Endereços que não devem usar o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="23235-116">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="23235-117">O sistema não usará o servidor proxy para endereços que começam com o conteúdo especificado nesse nó.</span><span class="sxs-lookup"><span data-stu-id="23235-117">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="23235-118">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="23235-118">useForLocalAddresses</span></span>|<span data-ttu-id="23235-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="23235-119">Boolean</span></span>|<span data-ttu-id="23235-120">Especifica se o servidor proxy deve ser usado para endereços locais (intranet).</span><span class="sxs-lookup"><span data-stu-id="23235-120">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23235-121">Relações</span><span class="sxs-lookup"><span data-stu-id="23235-121">Relationships</span></span>
<span data-ttu-id="23235-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23235-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23235-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23235-123">JSON Representation</span></span>
<span data-ttu-id="23235-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23235-124">Here is a JSON representation of the resource.</span></span>
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




