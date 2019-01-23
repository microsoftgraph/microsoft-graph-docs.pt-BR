---
title: Tipo de recurso windows10NetworkProxyServer
description: Política de Servidor Proxy de Rede.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 673cfe99e9cafe1b57fde5c70b7059286a6cc554
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418579"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="cd71d-103">Tipo de recurso windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="cd71d-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="cd71d-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="cd71d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cd71d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cd71d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cd71d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="cd71d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd71d-107">Política de Servidor Proxy de Rede.</span><span class="sxs-lookup"><span data-stu-id="cd71d-107">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="cd71d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cd71d-108">Properties</span></span>
|<span data-ttu-id="cd71d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd71d-109">Property</span></span>|<span data-ttu-id="cd71d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd71d-110">Type</span></span>|<span data-ttu-id="cd71d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd71d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd71d-112">address</span><span class="sxs-lookup"><span data-stu-id="cd71d-112">address</span></span>|<span data-ttu-id="cd71d-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd71d-113">String</span></span>|<span data-ttu-id="cd71d-114">Endereço para o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="cd71d-114">Address to the proxy server.</span></span> <span data-ttu-id="cd71d-115">Especifique um endereço no formato <server>\[“:”<port>\]</span><span class="sxs-lookup"><span data-stu-id="cd71d-115">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="cd71d-116">exceptions</span><span class="sxs-lookup"><span data-stu-id="cd71d-116">exceptions</span></span>|<span data-ttu-id="cd71d-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd71d-117">String collection</span></span>|<span data-ttu-id="cd71d-118">Endereços que não devem usar o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="cd71d-118">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="cd71d-119">O sistema não usará o servidor proxy para endereços que começam com o conteúdo especificado nesse nó.</span><span class="sxs-lookup"><span data-stu-id="cd71d-119">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="cd71d-120">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="cd71d-120">useForLocalAddresses</span></span>|<span data-ttu-id="cd71d-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="cd71d-121">Boolean</span></span>|<span data-ttu-id="cd71d-122">Especifica se o servidor proxy deve ser usado para endereços locais (intranet).</span><span class="sxs-lookup"><span data-stu-id="cd71d-122">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd71d-123">Relações</span><span class="sxs-lookup"><span data-stu-id="cd71d-123">Relationships</span></span>
<span data-ttu-id="cd71d-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cd71d-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd71d-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cd71d-125">JSON Representation</span></span>
<span data-ttu-id="cd71d-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cd71d-126">Here is a JSON representation of the resource.</span></span>
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




