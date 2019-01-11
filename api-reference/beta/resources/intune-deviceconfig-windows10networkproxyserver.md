---
title: Tipo de recurso windows10NetworkProxyServer
description: Política de Servidor Proxy de Rede.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7efe08c565aaeab109339c43e80225b6946299c3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876255"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="0e5e4-103">Tipo de recurso windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="0e5e4-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="0e5e4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0e5e4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e5e4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0e5e4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0e5e4-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0e5e4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e5e4-107">Política de Servidor Proxy de Rede.</span><span class="sxs-lookup"><span data-stu-id="0e5e4-107">Network Proxy Server Policy.</span></span>
## <a name="properties"></a><span data-ttu-id="0e5e4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0e5e4-108">Properties</span></span>
|<span data-ttu-id="0e5e4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e5e4-109">Property</span></span>|<span data-ttu-id="0e5e4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e5e4-110">Type</span></span>|<span data-ttu-id="0e5e4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e5e4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e5e4-112">address</span><span class="sxs-lookup"><span data-stu-id="0e5e4-112">address</span></span>|<span data-ttu-id="0e5e4-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e5e4-113">String</span></span>|<span data-ttu-id="0e5e4-114">Endereço para o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="0e5e4-114">Address to the proxy server.</span></span> <span data-ttu-id="0e5e4-115">Especifique um endereço no formato <server>\[“:”<port>\]</span><span class="sxs-lookup"><span data-stu-id="0e5e4-115">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="0e5e4-116">exceptions</span><span class="sxs-lookup"><span data-stu-id="0e5e4-116">exceptions</span></span>|<span data-ttu-id="0e5e4-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e5e4-117">String collection</span></span>|<span data-ttu-id="0e5e4-118">Endereços que não devem usar o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="0e5e4-118">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="0e5e4-119">O sistema não usará o servidor proxy para endereços que começam com o conteúdo especificado nesse nó.</span><span class="sxs-lookup"><span data-stu-id="0e5e4-119">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="0e5e4-120">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="0e5e4-120">useForLocalAddresses</span></span>|<span data-ttu-id="0e5e4-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="0e5e4-121">Boolean</span></span>|<span data-ttu-id="0e5e4-122">Especifica se o servidor proxy deve ser usado para endereços locais (intranet).</span><span class="sxs-lookup"><span data-stu-id="0e5e4-122">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e5e4-123">Relações</span><span class="sxs-lookup"><span data-stu-id="0e5e4-123">Relationships</span></span>
<span data-ttu-id="0e5e4-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0e5e4-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0e5e4-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0e5e4-125">JSON Representation</span></span>
<span data-ttu-id="0e5e4-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0e5e4-126">Here is a JSON representation of the resource.</span></span>
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





