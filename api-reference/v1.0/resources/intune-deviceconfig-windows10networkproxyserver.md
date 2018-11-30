---
title: Tipo de recurso windows10NetworkProxyServer
description: Política de Servidor Proxy de Rede.
ms.openlocfilehash: 2cd9d4ddc84733e3985f718fd2d3ef86481d762e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004140"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="3297c-103">Tipo de recurso windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="3297c-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="3297c-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3297c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3297c-105">Política de Servidor Proxy de Rede.</span><span class="sxs-lookup"><span data-stu-id="3297c-105">Network Proxy Server Policy.</span></span>
## <a name="properties"></a><span data-ttu-id="3297c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3297c-106">Properties</span></span>
|<span data-ttu-id="3297c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3297c-107">Property</span></span>|<span data-ttu-id="3297c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3297c-108">Type</span></span>|<span data-ttu-id="3297c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3297c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3297c-110">address</span><span class="sxs-lookup"><span data-stu-id="3297c-110">address</span></span>|<span data-ttu-id="3297c-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3297c-111">String</span></span>|<span data-ttu-id="3297c-112">Endereço para o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="3297c-112">Address to the proxy server.</span></span> <span data-ttu-id="3297c-113">Especifique um endereço no formato <server>\[“:”<port>\]</span><span class="sxs-lookup"><span data-stu-id="3297c-113">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="3297c-114">exceptions</span><span class="sxs-lookup"><span data-stu-id="3297c-114">exceptions</span></span>|<span data-ttu-id="3297c-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3297c-115">String collection</span></span>|<span data-ttu-id="3297c-116">Endereços que não devem usar o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="3297c-116">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="3297c-117">O sistema não usará o servidor proxy para endereços que começam com o conteúdo especificado nesse nó.</span><span class="sxs-lookup"><span data-stu-id="3297c-117">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="3297c-118">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="3297c-118">useForLocalAddresses</span></span>|<span data-ttu-id="3297c-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="3297c-119">Boolean</span></span>|<span data-ttu-id="3297c-120">Especifica se o servidor proxy deve ser usado para endereços locais (intranet).</span><span class="sxs-lookup"><span data-stu-id="3297c-120">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3297c-121">Relações</span><span class="sxs-lookup"><span data-stu-id="3297c-121">Relationships</span></span>
<span data-ttu-id="3297c-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3297c-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3297c-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3297c-123">JSON Representation</span></span>
<span data-ttu-id="3297c-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3297c-124">Here is a JSON representation of the resource.</span></span>
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



