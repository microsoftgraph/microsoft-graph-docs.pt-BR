---
title: Tipo de recurso windows10NetworkProxyServer
description: Política de Servidor Proxy de Rede.
ms.openlocfilehash: 4e2e995c8d66249e5c742343f74e18e87337bfaa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038655"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="e08be-103">Tipo de recurso windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="e08be-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="e08be-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e08be-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e08be-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e08be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e08be-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e08be-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e08be-107">Política de Servidor Proxy de Rede.</span><span class="sxs-lookup"><span data-stu-id="e08be-107">Network Proxy Server Policy.</span></span>
## <a name="properties"></a><span data-ttu-id="e08be-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e08be-108">Properties</span></span>
|<span data-ttu-id="e08be-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e08be-109">Property</span></span>|<span data-ttu-id="e08be-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e08be-110">Type</span></span>|<span data-ttu-id="e08be-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e08be-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e08be-112">address</span><span class="sxs-lookup"><span data-stu-id="e08be-112">address</span></span>|<span data-ttu-id="e08be-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e08be-113">String</span></span>|<span data-ttu-id="e08be-114">Endereço para o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="e08be-114">Address to the proxy server.</span></span> <span data-ttu-id="e08be-115">Especifique um endereço no formato <server>\[“:”<port>\]</span><span class="sxs-lookup"><span data-stu-id="e08be-115">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="e08be-116">exceptions</span><span class="sxs-lookup"><span data-stu-id="e08be-116">exceptions</span></span>|<span data-ttu-id="e08be-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e08be-117">String collection</span></span>|<span data-ttu-id="e08be-118">Endereços que não devem usar o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="e08be-118">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="e08be-119">O sistema não usará o servidor proxy para endereços que começam com o conteúdo especificado nesse nó.</span><span class="sxs-lookup"><span data-stu-id="e08be-119">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="e08be-120">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="e08be-120">useForLocalAddresses</span></span>|<span data-ttu-id="e08be-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="e08be-121">Boolean</span></span>|<span data-ttu-id="e08be-122">Especifica se o servidor proxy deve ser usado para endereços locais (intranet).</span><span class="sxs-lookup"><span data-stu-id="e08be-122">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e08be-123">Relações</span><span class="sxs-lookup"><span data-stu-id="e08be-123">Relationships</span></span>
<span data-ttu-id="e08be-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e08be-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e08be-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e08be-125">JSON Representation</span></span>
<span data-ttu-id="e08be-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e08be-126">Here is a JSON representation of the resource.</span></span>
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





